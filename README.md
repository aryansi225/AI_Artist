# AI_Artist

In this project a base video and style reference image is taken. The base video is decomposed into frames by using opencv and each frame is passed through a trained deep convolutional neural network over a dataset to repaint base image based on the style of another style reference image. Then the repainted image spitted out of the neural network is again joined to form the output video using opencv

# Examples

![blue moon lake](https://cloud.githubusercontent.com/assets/16362957/20453699/2ce3621c-ae53-11e6-8aea-100934576fc0.gif)

<img src="https://cloud.githubusercontent.com/assets/16362957/20453729/0b5f885e-ae54-11e6-89b8-5e3063d50369.jpg" width="250" height="250"><img src="https://cloud.githubusercontent.com/assets/16362957/20453731/0daa968a-ae54-11e6-823e-cf00edd891dc.png" width="250" height="250">

<img src="https://cloud.githubusercontent.com/assets/16362957/20453732/11700746-ae54-11e6-9962-eb990e817c59.jpg" width="250" height="250"> <img src="https://cloud.githubusercontent.com/assets/16362957/20453733/140639e4-ae54-11e6-9f33-432327685bb3.png" width="250" height="250">

# Dependencies

* Numpy (http://www.numpy.org/)
* Keras (http://keras.io/#installation)
* Scipy (https://www.scipy.org/install.html)
* Theano (http://deeplearning.net/software/theano/install.html#install)
* h5py (http://docs.h5py.org/en/latest/build.html)
* sklearn (http://scikit-learn.org/stable/install.html)
* Pillow (https://pillow.readthedocs.io/en/latest/installation.html)
* CUDA (GPU) (http://docs.nvidia.com/cuda/cuda-getting-started-guide-for-mac-os-x/)
* CUDNN (GPU) (https://developer.nvidia.com/cudnn)
* VGG16 file https://drive.google.com/file/d/0Bz7KyqmuGsilT0J5dmRCM0ROVHc/view?usp=sharing
