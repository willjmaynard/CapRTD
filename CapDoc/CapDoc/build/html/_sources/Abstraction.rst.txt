Abstraction
===========

There are many medical slide images that contain artifacts, hence our group is implementing an artifact detection tool which is used to detect artifacts in Whole Slide Images (WSIs) and classifies detected artifacts areas, such as out-of-focus, blurry, not blurry, or in-focus areas. This project focuses on blur detection in WSIs, calculating the accuracy of each image, performing classification methods, and providing complete documentation in the readthedocs. The aim of this project is to develop the artifact detection tool which is based on a deep learning concept. For blur detection, we used a tool based on the DeepFocus model. This tool is a form of classification that scans the image, patch-by-patch, and returns the classified image data. Additionally, we performed additional classification methods on WSIs, such as Laplacian and Image Variance. In this project, the following steps were performed:

•	Whole slide scanners (WSSs) are used to scan all the whole slide images (WSIs) and use binary classification to divide them into small patches of pixels. These patches are classified as containing artifacts or not by using patch classification.

•	Patch classification will take super pixel regions and scan them instead of detecting the entire image at once.

•	For these regions, we tried to achieve 80% or more accuracy on each detected image.

•	Show a data visualization on accuracy that describes the accuracy results.

•	For super-pixel regions, we have used binary classifications to label what regions have been identified as containing an artifact.
