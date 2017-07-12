# Artificial Intelligence Engineer Nanodegree Term II
## Computer Vision Capstone Project
### Project: Facial Keypoint Detection and Real-time Filtering
## Overview

In this project, I combined my knowledge of computer vision techniques and deep
learning to build and end-to-end facial keypoint recognition system. Facial 
keypoints include points around the eyes, nose, and mouth on any face and are 
used in many applications, from facial tracking to emotion recognition. My code is 
able to take in any image containing faces and identify the location of each 
face and their facial keypoints, as shown below,

![Facial Keypoint Detection][image1]

## Getting Started

### Environment

1. Clone the repository, and navigate to the downloaded folder.
```
git clone https://github.com/JonathanKSullivan/Facial-Keypoint-Detection.git
cd AIND-CV-FacialKeypoints
```

2. Create (and activate) a new environment with Python 3.5 and the `numpy` package.

	- __Linux__ or __Mac__: 
	```
	conda create --name aind-cv python=3.5 numpy
	source activate aind-cv
	```
	- __Windows__: 
	```
	conda create --name aind-cv python=3.5 numpy scipy
	activate aind-cv
	```

3. Install/Update TensorFlow (for this project, you may use CPU only).
	- Option 1: __To install TensorFlow with GPU support__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.  If you are using the Udacity AMI, you can skip this step and only need to install the `tensorflow-gpu` package:
	```
	pip install tensorflow-gpu -U
	```
	- Option 2: __To install TensorFlow with CPU support only__:
	```
	pip install tensorflow -U
	```

4. Install/Update Keras.
 ```
pip install keras -U
```

5. Switch [Keras backend](https://keras.io/backend/) to TensorFlow.
	- __Linux__ or __Mac__: 
	```
	KERAS_BACKEND=tensorflow python -c "from keras import backend"
	```
	- __Windows__: 
	```
	set KERAS_BACKEND=tensorflow
	python -c "from keras import backend"
	```

6. Install a few required pip packages (including OpenCV).
```
pip install -r requirements.txt
```


### Data

All of the data you'll need to train a neural network is in the AIND-CV-FacialKeypoints repo, in the subdirectory `data`. In this folder are a zipped training and test set of data.

1. Navigate to the data directory
```
cd data
```

2. Unzip the training and test data (in that same location). If you are in Windows, you can download this data and unzip it by double-clicking the zipped files. In Mac, you can use the terminal commands below.
```
unzip training.zip
unzip test.zip
```

You should be left with two `.csv` files of the same name. You may delete the zipped files.

*Troubleshooting*: If you are having trouble unzipping this data, you can download that same training and test data on [Kaggle](https://www.kaggle.com/c/facial-keypoints-detection/data).

Now, with that data unzipped, you should have everything you need!


### Project files
Main project files:
- **mimic.js**: Javascript file with code that connects to the Affectiva API and processes results.
- **index.html**: Dynamic webpage that displays the video feed and results.
- **mimic.css**: Stylesheet file that defines the layout and presentation for HTML elements.

There are two additional files provided for serving the project as a local web application: 

- **serve.py**: A lightweight Python webserver required to serve the webpage over HTTPS, so that we can access the webcam feed.
- **generate-pemfile.sh**: A shell script you’ll need to run once to generate an SSL certificate for the webserver.

## Deployment


1. Navigate back to the repo. (Also your source environment should still be activated at this point)
```shell
cd
cd AIND-CV-FacialKeypoints
```

2. Open the notebook and follow the instructions.
```shell
jupyter notebook CV_project.ipynb
```

## Built With
## Authors
* **Udacity** - *Initial work* - [AIND-CV-FacialKeypoints](https://github.com/udacity/AIND-CV-FacialKeypoints)
* **Jonathan Sulivan**

## Acknowledgments
* Hackbright Academy
* Udacity


<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>. Please refer to [Udacity Terms of Service](https://www.udacity.com/legal) for further information.
