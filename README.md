# Speech Denoising Deep Learning Model

File Structure:
```
Speech Denoising Model Code
├── Dataset
│   ├──Clean
│   └──Noisy
├── Demucs
│   ├── Inference and Metrics Basic
│   ├── Metrics Advanced
│   └── Training 
└── FullSubNet
    ├── Metrics Basic
    ├── Metrics Advanced
    ├── Training
    └── Inference
```
TAPLoss, a novel differentiable loss function that allows for training deep learning denoiser model, is attached to Demucs and FullSubNet, the state of the art of denosing models to improve those models.

# Dataset 
- Data included in the dataset directory includes 150 pairs of test clean and noisy audio files. These data are added for convenience for the users to test scripts in this repo.
- Testing as well as training data are be downloaded in the code in the Demucs/FSN trianing notebook.

# How to Use this Repo
1. Metrics notebook require a pair of clean and noisy dataset. The pair is used to output various speech evaluation matrics. Basic metrics notebook utilizes python packages (librosa, pysepm,pystoi and speechmetrics). The metrics advanced notebook utilizes open smile package and it requires clean audio files, original noisy audio files and enhanced noisy auido files to run. Metrics advanced notebook in Demucs and FullSubNet are the same and duplicated for convenience.

2. Inference notebook downloads currently the best FSN and Demucs models and runs inference on noisy data. Enhanced audio files are outputted from the inference.

3. Training notebook includes the code for data download, model configurations and deploying training python scripts. Specific data can selected by only including paths to certain data. Configuations can be changed by altering the configuration file. 






