# Time series prediction and text generation

## Quick start

It is recommended you run this project on a GPU enabled system. If you have access to a GPU, you should follow the Keras instructions for [running Keras on GPU](https://keras.io/getting-started/faq/#how-can-i-run-keras-on-gpu). 

1. Clone the repository, and navigate to the downloaded folder.
```
git clone https://github.com/ysharc/text-generation.git
cd text-generation
```

2. Create (and activate) a new environment with Python 3.6 and the `numpy` package.

	- __Linux__ or __Mac__: 
	```
	conda create --name text-generation python=3.6 numpy
	source activate text-generation
	```
	- __Windows__: 
	```
	conda create --name text-generation python=3.6 numpy scipy
	activate text-generation
	```

3. Install/Update TensorFlow (for this project, you may use CPU only).
	- Option 1: __To install TensorFlow with GPU support__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.
	```
	pip install tensorflow-gpu==1.3.0
	```
	- Option 2: __To install TensorFlow with CPU support only__:
	```
	pip install tensorflow==1.3.0
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

7. Run the notebook and follow instructions
```
jupyter notebook RNN_project.ipynb
```