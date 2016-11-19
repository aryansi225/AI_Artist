# AI_Artist

In this project a base video and style reference image is taken. The base video is decomposed into frames by using opencv and each frame is passed through a trained deep convolutional neural network over a dataset to repaint base image based on the style of another style reference image. Then the repainted image spitted out of the neural network is again joined to form the output video using opencv

