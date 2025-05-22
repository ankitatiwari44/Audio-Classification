# Audio-Classification using Machine Learning

Audio classification is the process of analyzing and identifying any type of audio, sound, noise, musical notes, or any other similar type of data to classify them accordingly. The audio data that is available to us can occur in numerous forms, such as sound from acoustic devices, musical chords from instruments, human speech, or even naturally occurring sounds like the chirping of birds in the environment. Modern machine learning techniques allow us to achieve state-of-the-art results for tasks and projects related to audio signal processing.

dataset is taken from Link = https://urbansounddataset.weebly.com/download-urbansound8k.html

Part 1 -> Exploratory data analysis
In this part we have learned about audio signal processing where audio are of form .wav here using sound file we have displayed it in wave using librosa and scipy.
Librosa has much more advantages here :

1. librosa normlize the audio signals data between -1 to +1
2. This library used for audio signal processing it helps to converge audio signal into mono-one.
3. it can represent audio signal it normalized manner from -1 to +1 so that the regular pattern can be observed from all audio signals
4. It also sees the sample rate and by deault it converts to 22050

Scipy is not mono it has multiple signals i.e more than one channel also they are not in normalized form.

Part 2 -> Extract Features
Here we will be using Mel-Frequency Cepstral Coefficients(MFCC) from the audio samples. The MFCC summarises the frequency distribution across the window size, so it is possible to analyse both the frequency and time characteristics of the sound. These audio representations will allow us to identify features for classification.
Followed by creating dataframe of extracted_feature and getting dependent and independent features then spliting data using train test split.

Part 3-> Model Creation 
In this part we are craeting our model ANN input layer followed by hidden layers with activation function relu then output layer which will give model predicted output i.e classification of audio.

Part 4 -> Testing Model for new test data
We performed label encoding to y i.e class then testing ANN model finding whether class predicted is correct .

