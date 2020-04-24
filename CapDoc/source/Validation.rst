Validation
==========

Firstly, worked on smaller image files before testing our python code on the WSIs and as the size of WSIs is ~5GB. For training, the slide is scanned by lines (pixels) i.e., patch by patch classification. To train the model, first 150,000 images were used from the dataset and the remaining 15,000 images of the dataset were used for testing throughout the training. Moreover, the rest of the images were used for validation datasets and this image samples are classified as an image tile which results in in-focus or blurry.
This method selects focus points of the image tiles whose offset values are in between -0.5 micron to +0.5 micron. In this model, image tiles are placed with labels and labels with assigned 4,5,6 are considered “in focus” and all others are considered “out of focus”. For a binary classification problem, this model is based on a convolutional neural network named as DeepFocus model.
