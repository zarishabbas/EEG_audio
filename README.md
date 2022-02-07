# EEG_audio

link to raw data: Cejnek, Matouš (2017): dataset.zip. figshare. Dataset. https://doi.org/10.6084/m9.figshare.5450293.v1 

## Summary
Data consists of EEG recordings of resting-state activity obtained from people with Alzheimer's disease (AD), mild cognitive impairment (MCI) and healthy controls. More information about the experiment can be found in the paper:

https://link.springer.com/article/10.1007/s11517-021-02427-6

The goal of this project was to develop a machine learning algorithm that could predict the diagnosis of people with AD. The secondary goal was to extract features from the signal that contribute to the prediction of Alzheimer's disease. The signals were converted to audio to be used as sound for the film, *Promenade nocturne* by Ryan Mckenna (in production).

## Project structure
*Note.* In this project, people with MCI were not considered to avoid an imbalanced dataset. 

1. Preprocessing: equalize session
2. Preprocessing: filtering and rereferencing
3. Preprocessing: creating epochs, standardizing, and performing ICA
4. Classification using CNN
5. Converting signal to audio using librosa

## Requirements
It is strongly recommended to create a separate environment for the project.
Preprocessing was conducted using MNE-Python, and the classification was performed using tensorflow. Sonification was performed using librosa.
dependencies needed can be found in "requirements.txt"

