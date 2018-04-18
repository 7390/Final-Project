# Billboard Chart Prediction
The Portfolio of INFO7390
## Introduction

## Getting Start

### Prerequisites
You should install Spotipy, billboard api , and Tensorflow and download the dataset on(https://drive.google.com/file/d/1RXsMtwsQRs_kPpgHB2uxJzspAhTPcPx8/view?usp=sharing)

### Installation
1.spotipy api
```bash
pip install spotipy
```
You can see this api at [spotipy github](https://github.com/plamere/spotipy).

2.billboard api(Unofficial)
```bash
pip install billboard.py
```
you can see all documents at[Allen Guo](https://github.com/guoguo12/billboard-charts)

3.Tensorflow
```bash
pip install --ignore-installed --upgrade tensorflow-gpu 
```
you must install GPU version of TensorFlow,and all the documents are at[Tensorflow](https://www.tensorflow.org/?hl=zh-cn)

### Get Billboad Chart by using Billboard API
you should run getdata.py with the data1.csv to get 100000 songs rank in billboard chart,if you run getdata.py and get about 100000 songs data which were saved in data.csv.

### Use the Spotify API to get Audio Feature
1.run regetdata.py to get the Artist id, Track id and audio feature of each track, then you will get all data which we have saved in new_data.csv. 

2.run aa_append_artists.py to get each artist popularity and followers, and we save in the pop_follower.csv

3.run read.Json.py to get each track's audio analysis, and we save all data into Data_Json folder.

Use Mysql to combine all these data into one csv file which we saved as Full_data.csv



Data

The datasets are obtained from Billboard API, Spotify API and web scraper; the first is a dataset in which the host took the weekly Top 100 Billboard charts and scraped song lyrics websites. The second is year-end Billboard charts range from 1964 to 2017 and song lyrics scraped from three websites.

Methods

A. Preprocess the data
   1. Data cleaning
   2. Changing the column['Rank']: If the rank is higher than 30(<30), the added colomn Hit will be Yes or "1"; If the rank is lower than 30(>30), the added colomn Hit will be No or "0".
   
B. Analyze the data
   1. Find out the linear relation between the features of the song
   2. Find out the lyrics trending in Billboard
   
C. Modeling
   1. 
   
D. Computing Platform


Results
A. 
