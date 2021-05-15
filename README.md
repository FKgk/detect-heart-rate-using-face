# detect-heart-rate-using-face

## Origin Code
1. [eulerian-remote-heartrate-detection](https://github.com/rohintangirala/eulerian-remote-heartrate-detection)
- using Cascade, Pyramid and heartrate-detection

2. [Heart-rate-measurement-using-camera](https://github.com/habom2310/Heart-rate-measurement-using-camera)
- using face detector

3. [QRS-detection](https://github.com/KChen89/QRS-detection)
- using QRS detector

## Dataset
### Emotion elicitation trials of [mahnob-db](https://mahnob-db.eu/hci-tagging/)
- Twenty of the entire videos were used, and were composed of 144980 frames
- The video was cut every 10 seconds and the remaining videos(Less than 10 seconds) were discarded.
- So we conducted the test with a total of 222 data.

### Results (using Cascade-Pyramid-eulerian)
- RMSE: 9.6
- MAE: 6.0

### Reference
- We test the video(about 8) of smartphone(Galaxy A8) using file of Dlib(fixed_position)-Pyramid-eulerian
- this best Result is following
- RMSE: 8.8
- MAE: 7.6

## How to run
```
git clone https://github.com/FKgk/detect-heart-rate-using-face.git
cd detect-heart-rate-using-face
conda create -n qrs python=3.8.1
conda activate qrs
pip install -r requirements.txt
```
OR
```
git clone https://github.com/FKgk/detect-heart-rate-using-face.git
cd detect-heart-rate-using-face
conda env create -f ./environment.yml
```
- Put your data to data folder
- Select the code in code folder
- You must adjust the input_path in the code
- Run this code

## Sub_code folder
- This is real subfiles
- Cut the video per 10 sec
- Change from bdf format to csv format
- Detecting QRS and get heartrate (using EXG2 signal)

## [Summary](https://github.com/FKgk/detect-heart-rate-using-face/blob/master/summary.md)
- If you are interested in this topic, I suggest to take a look at the link.
