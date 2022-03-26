# Xilinx Package Detection using Tensorflow

This set of Notebooks was taken from https://github.com/nicknochnack/TFODCourse by following the [Youtube Tutorial](https://youtu.be/yqkISICHH-U) from 
Nicholas Renotte's [YouTube channel](https://www.youtube.com/c/nicholasrenotte). The differences are the training dataset was modified to detect packages instead of hand signs and the virtual environment was renamed from tfod to xpd. Also there is a slight modification in the jupyter notebook 2. Training and Detection.ipynb to detect package theft when the package moves upwards in 10 successive frames.

## Getting started
**Step 1.** Clone this repository: https://github.com/nicknochnack/TFODCourse  
 
**Step 2.** Create a new virtual environment

python3 -m venv xpd

  
**Step 3.** Activate your virtual environment

source xpd/bin/activate # Linux

  
**Step 4.** Install dependencies and add virtual environment to the Python Kernel

python3 -m pip install --upgrade pip
pip install ipykernel
python3 -m ipykernel install --user --name=xpd

  
**Step 5.** Collect images using the Notebook 1\. Image Collection.ipynb - ensure you change the kernel to the virtual environment xpd

**Step 6.** Manually divide collected images into two folders train and test. So now all folders and annotations should be split between the following two folders.  
./Tensorflow/workspace/images/train  
./Tensorflow/workspace/images/test  
  
**Step 7.** Begin training process by opening [2\. Training and Detection.ipynb] this notebook will walk you through installing Tensorflow Object Detection, making detections, saving and exporting your model.  
