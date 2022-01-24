# EEG_audio

link to raw data: Cejnek, Matouš (2017): dataset.zip. figshare. Dataset. https://doi.org/10.6084/m9.figshare.5450293.v1 

## Summary
Data consists of EEG recordings of restings state activity obtained from people with Alzheimer's disease (AD), mild cognitive impairment (MCI) and healthy controls. More information about the experiment can be found in the paper:

https://link.springer.com/article/10.1007/s11517-021-02427-6

The goal of this project was to develop a machine learning algorithm that could predict the diagnosis of the people with AD. The secondary goal was to extract features from the signal that contribute to the prediction of Alzheimer's disease. The signals were converted to audio to be used as sound for the film, *Promenade nocturne* by Ryan Mckenna (in production).

## Project structure
*Note.* In this project, people with MCI were not considered due to the imbalance of the dataset. 

1. Exploratory Analysis
2. Preprocessing: equalize session
3. Preprocessing: filtering and rereferencing
4. Preprocessing: creating epochs, standardizing, and performing ICA
5. Classification using CNN
6. Converting signal to audio using librosa

## Requirements
It is strongly recommended to create a separate environment for the project.
Preprocessing was conducted using MNE-Python, and the classification was performed using tensorflow. Sonification was performed using librosa.
dependencies needed can be found in "requirements.txt"

