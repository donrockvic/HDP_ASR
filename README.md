# ASR
This is my first ASR project.
Basic Audio to Speech Recognition



## Content

Dataset Used: speech_commands
[Data Page](https://www.tensorflow.org/datasets/catalog/speech_commands)
[Data download link](http://download.tensorflow.org/data/speech_commands_v0.02.tar.gz)

After converting the data to numpy, i sored them on [Drive](https://drive.google.com/drive/folders/1q0JfWZ4eUmAX-luQ44tU9lppXdkiJQfw?usp=sharing).

## Project Description
* [ASR_DATA.ipynb]: Notebook to convert Audion data from wav file to numpy array and visualization.
* [ASR.ipynb]: Jupyter notebook which is used to create model for our SR model. We have used CNN model with 5 hidden layer.
* [app.py]: Main python script which trigger the Project. 
* [record.py]: Python file which is using [Sounddevice](https://pypi.org/project/sounddevice/) and [scipy]() to record the sound.
* [split.py]: We are using [pydub](https://github.com/jiaaro/pydub/tree/master/pydub) for spliting the speech.Breaking down the 
word can be done by looking at the pause in the waveform, but to save time I have used pydub.


## Result
Since the data set is small, and there is not enough words, the performance of my model is as below

loss: 0.9303 - accuracy: 0.7407 - val_loss: 0.8464 - val_accuracy: 0.7622


## More libs
* [Librosa]: creating numpy array from audio file
* [Tensorflow]: For creating CNN  model
* [Scikit Lib]: For train_test_split
* [matplot lib]: for visualization
