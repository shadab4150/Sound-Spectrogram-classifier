# Sound Spectrogram classifier

## Dataset: " 50 enviromental sound dataset"

* There are 50 types sounds in each fold, each type contains 8 files 

  * I will use fold 1,2,3,4 for training, **total train spectrogram:** **1600** 

  * fold 5 for validation, **total test spectrogram:**  **400**

* **In this project I have build a classifier that distinguises between 50 different types of sound.**

* First I pre-processed the **.wav** audio files to **spectrograms** to train a deep learning model.

* I have used **resnet50** pretrained model.  *A Deep Residual Learning for Image Recognition.*

 *I have used a **pretrained model** because **learned features are often transferable to different data**. For **example**, a model trained on a large dataset of bird images will contain learned features like edges or horizontal lines that would be transferable to my data.*


[**Notebook sound to spectrogram pre-processing**](https://nbviewer.jupyter.org/github/shadab4150/Sound-Spectrogram-classifier/blob/master/sound_to_image_pre_processing.ipynb)


* **spectrogram** of clapping sound:


* Matplotlib **specgram**


![kd](https://i.ibb.co/xXWpCSd/downloczczczad.png)


* librosa specgram


![kd](https://i.ibb.co/Wn2WzGB/1-15689-A-4-4.png)


[**Spectrogram classification notebook**](https://nbviewer.jupyter.org/github/shadab4150/Sound-Spectrogram-classifier/blob/master/environmental_sound_spectrogram_classification.ipynb)


* **Spectrogram Datablock:**

![kd](https://i.ibb.co/qn415xm/downzczczcload.png)

### Confusion matrix:

![kd](https://i.ibb.co/QbWnSwk/downloczczczczcad.png)

#### Most confused:

![kd](https://i.ibb.co/JCsWZ4B/downloazczczczczzd.png)


* As we can see from the above confusion matrix it gets most confused between:

  * between **clapping** and **rain** is **3** times
  * between **helicopter** and **airplane** is **3** times
  * between **wind** and  **siren** is **3** times

## Final accuracy is **78%**
