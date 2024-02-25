# Pan-card-tampering-detector
## Detect potential tampering or alterations in PAN card images using machine learning and image processing techniques.

This project is an example of how one can use machine learning and image processing techniques to identify any potential tampering or alterations in PAN (Permanent Account Number) cards issued by the Income Tax Department of India. This project provides a simple and efficient way to analyze PAN card images and flag any suspicious modifications.

**Basic Understanding of code**
* Collect two different Pan card images - orginal & tampered
* Resize and change format if required
* Convert the images into gray scale
* Check for structural similarity index (SSI)- High SSI(Authentic card), Low SSI(Tampered Card)
* Apply Thresholding to the images (separate objects from the background in an image) for identify alterations between two images.
* Find and extract contours in the thresholded image to identify and extract the boundaries of regions that have changed or differ significantly from the reference image.
* Create blue rectangle boxes in both images to the parts which have been tampered making it easier to analyze the differences between the two images.

**Dependencies**
* Python
* Google Colab
* Libraries: skimage.metrics, imutils, PIL, requests, NumPy, OpenCV

**Data Sources**
* Publicly available PAN card images (e.g., government websites, online repositories)
* Personal PAN card dataset
