# Audio_classification

## Table of Contents
1. [Introduction](#introduction)
2. [System Requirements](#system-requirements)
3. [Installation](#installation)
4. [Data](#data)
5. [Usage](#usage)
6. [Results](#results)
7. [License](#license)

## Introduction
This project uses CNN models for audio classification. The goal is to classify audios which come from different sources.

## System Requirements
- Python 3.8+
- Jupyter Notebook
- Kaggle (for running the notebook)

## Installation
The Jupyter notebook can be run on Kaggle. Follow these steps to get started:
1. Upload the notebook to Kaggle.
2. Add Urbansound8k dataset to your uploaded notebook. (if needed)
3. Run the notebook with GPU accelerator. (Should use GPU P100)

## Data
- **Source**: Urbansound8k.
- **Description**: This dataset contains 8732 labeled sound excerpts (<=4s) of urban sounds from 10 classes: air_conditioner, car_horn, children_playing, dog_bark, drilling, enginge_idling, gun_shot, jackhammer, siren, and street_music.

## Usage
To use the notebook:
1. Open the .ipynb file in Kaggle.
2. If you want to perform with MelSpectrogram transform, change the line 41 at 7th code cell with this code:
``sgram = AudioUtil.LFCC(shift_aud, n_lfcc=64, n_fft=1024, hop_len=None)``
3. Run each cell consecutively from top to bottom.

## Results
![image](https://imgur.com/a/libPEgs)
