# AI_Artist

In this project a base video and style reference image is taken. The base video is decomposed into frames by using opencv and each frame is passed through a trained deep convolutional neural network over a dataset to repaint base image based on the style of another style reference image. Then the repainted image spitted out of the neural network is again joined to form the output video using opencv. This is the implementation of Neural Style Transfer from the paper [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576) in Keras 1.0.2.

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

# Basic Usage

There are 3 parts to identify when we run the script

1. Your base video (to artify)
2. Your reference image (the art to learn from)
3. Your generated video
Run the following comand to generate an image in your chosen style

python aistist.py --base_video_path /path/to/your/video --style_reference_image_path /path/to/your/painting --result_prefix /path/to/generated/file/you/create

Other optional commands are
* --image_size: Size of your output frame
* --content_weight: How much to weigh the content
* --style_weight: How much to weigh the style
* --style_scale: How much to scale the style
* --total_variation_weight: Uniformity of the generated frame
* --num_iter: Nmber of iterations
* --rescale_image: to rescale or not to rescale
* --rescale_method: rescale algorithm
* --maintain_aspect_ratio: to maintain aspect ratio or not
* --content_layer: which layer to focus on for content generation

# References

Credits to [Somsubra Majumdar](https://github.com/titu1994/Neural-Style-Transfer), [Siraj Raval](https://github.com/llSourcell/AI_Artist) for vast majority of code. 

