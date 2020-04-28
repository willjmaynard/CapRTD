Evaluation
==========

We used the following steps:

  •	Created a python code that analyzes whole slide image files and returns the location of artifacts.
  •	Used whole slide scanners (WSSs) to scan the entire images, produce digital images with out-of-focus or blurry areas.
  •	A binary classification for whole slide images (WSIs) which are divided into small patches of pixels and these patches will be classified as containing artifacts or not.
  •	For this project, the most challenging part for super-pixel regions is to achieve 80% or more accuracy on each detected image and show a data visualization on accuracy that describes the accuracy results.
  •	For super-pixel regions, we have used classifications, such as the variance of the Laplacian method and image variance to achieve more accurate results on each detected image.
  •	To evaluate the proposed method i.e., deep learning algorithm, we measured the accuracy for blurry images if WSSs found a blurry image tile.

Accuracy= TP+TN/P+N
Where TP, TN, P, and N are the numbers of correctly classified in-focus and blurry image tiles, the number of in-focus image tiles, and the number of blurry image tiles.

In the figure below, the two bar graphs compare the accuracy and F1 Scores of our classification techniques on the same validation set.

.. image:: ../images/class_validation.png
