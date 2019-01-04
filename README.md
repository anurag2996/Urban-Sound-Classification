# Urban-Sound-Classification
## Dataset and its structure
1. We can use Urban Sound Classification ( https://urbansounddataset.weebly.com/ ) dataset which is quite popular.

2. Whichever dataset you are using, it is important to understand its structure and how to extract required features out of them.

3. For UrbanSound8K dataset, it can be downloaded using the following link ( https://goo.gl/8hY5ER ). It downloads a compressed tar file of size around 6GB.

4. On extracting it, it contains two folders named 'audio' and 'metadata'.

5. Audio folder contains 10 folders with name fold1, fold2 and so on, each having approximately 800 audio files of 4s each.

6. Metadata folder contains a .csv file having various columns such as file_id, label, class_id corresponding to label, salience etc.

7. Complete description can be found here https://urbansounddataset.weebly.com/urbansound8k.html

# Library To Use
We can use librosa library which can be installed using

pip install librosa

It uses ffmpeg as backend to convert and read some of the audio files. So to install ffmpeg, you can use

apt-get install ffmpeg

Librosa library can read audio files and convert them to there amplitude values for each sample of audio. Let us say there is an audio file of 4s and sampling rate of audio file is 22050 Hz. This means that audio file is made using amplitude samples such that 22050 samples of amplitudes are recorded in each second. Hence a 4s audio file with sampling rate 22050 can be expressed as an array of 4*22050=88200 size


