# Speech-Emotion-Recognition
A Speech Emotion Recognition model that classifies an audio into the 7 types of emotions taking an audio recording as the input.

Algorithm Applied: Recurrent Neural Networks (RNN) using LSTM

Dataset: RAVDESS 

Platform Used: Jupyter (using Anaconda)

**Pre-Requistes**
1. Python 3.0
2. Ravdess Dataset
3. Creating a new python env (optional)
4. Installing these Libraries

    *Libraries*

    Tensorflow v2.1.0\
    h5py v2.10.0\
    Scikit-learn v0.23.2\
    Librosa v0.8.0\
    Numba v0.48.0\
    Numpy v1.18.5\
    Pandas v1.1.1\
    Matplotlib v3.1.3
    
5. Your Mic should be working in order to test out the model. (Real Time Audio Recording) (Still A Work in Progress)

***Details about the Dataset Used***
| Corpus |  RAVDESS |
| :--- | :--- |
| Full Name | Ryerson Audio-Visual Database of Emotional Speech and Song |
| Origin | Ryerson University, Toronto, CA |
| Home URL | https://smartlaboratory.org/ravdess/ |
| License | Creative Commmons |
| Type | Multimodal |
| Speech Files | 1440 |
| Emotion Classes | 8 |
| Sentences | 2 |
| Male Actors | 12 |
| Female Actors | 12 |
| Total Actors | 24 |
| Age | 21 to 33 years |

*Filename Identifiers*:\
•	Modality (01 = full-AV, 02 = video-only, 03 = audio-only).\
•	Vocal channel (01 = speech, 02 = song).\
•	Emotion (01 = neutral, 02 = calm, 03 = happy, 04 = sad, 05 = angry, 06 = fearful, 07 = disgust, 08 = surprised).\
•	Emotional intensity (01 = normal, 02 = strong). NOTE: There is no strong intensity for the 'neutral' emotion.\
•	Statement (01 = "Kids are talking by the door", 02 = "Dogs are sitting by the door").\
•	Repetition (01 = 1st repetition, 02 = 2nd repetition).\
•	Actor (01 to 24. Odd numbered actors are male, even numbered actors are female).

**Execution of the Project**

Step 1: Download/ clone the repo into a folder and download the RAVDESS dataset into the same folder.

Step 2: Run Feature_Extraction.ipynb (cell by cell). Output Files: RAVDESS_Librosa_RNN.csv 

Step 3: Execute Main.ipynb cell by cell. Output Files:
                                                      1. RNN_RAVDESS.h5
                                                      2. mean_X.npy
                                                      3. std_X.npy

Step 4: Execute Deployment.ipynb cell by cell and record audio by running the last cell (wait for 'Recording!' and then speak into your mic) and enjoy the Prediction!

**OUTPUT**

![op1](https://user-images.githubusercontent.com/75331607/174962466-d9b77cb6-47f2-4cbb-8bb5-f28a59f81e0b.jpg)
![op2](https://user-images.githubusercontent.com/75331607/174962455-f0a9a1ab-8e44-4024-b7e8-2325eb2ca87e.jpg)
