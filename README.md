# Blur Detection with opencv-python
This blur detection python script is the implementation result of this [tutorial](https://www.pyimagesearch.com/2015/09/07/blur-detection-with-opencv/) by Adrian Rosebrock. Using the calculation of Laplacian's variance method, you can detect the amount of blurring.

## Prerequisites
* [Python](https://www.python.org/)
* [opencv-python](https://pypi.python.org/pypi/opencv-python)
* [imutils](https://pypi.python.org/pypi/imutils)

## How to use
Make sure python and pip is installed. Then, install imutils and cv2.
```bash
# install opencv-python
pip install cv2
# install imutils
pip install imutils
```

Place all your images sample in `images` folder (you can change the folder path later). After that, run this on your project folder. 
```bash
python blur-detection.py --images images
```

The output will be like these
```bash
images/good_5.jpg - Not Blurry: 2710.411224406914
images/blur_6.jpg - Not Blurry: 234.53143074452882
images/blur_7.jpg - Not Blurry: 387.4177703388444
images/good_4.jpg - Not Blurry: 514.4024536712872
images/good_6.jpg - Not Blurry: 1130.655860980799
images/blur_5.jpg - Not Blurry: 495.3206078451865
images/blur_4.jpg - Not Blurry: 324.83960554053556
images/good_7.jpg - Not Blurry: 327.8921565864165
images/good_3.jpg - Not Blurry: 1698.3861949567324
images/blur_1.jpg - Not Blurry: 314.23002861170755
images/good_2.jpg - Not Blurry: 442.25663961896294
images/blur_3.jpg - Not Blurry: 1709.9848988757813
images/blur_2.jpg - Not Blurry: 211.84270219774743
images/good_1.jpg - Not Blurry: 867.844288393801
images/good_10.jpg - Not Blurry: 795.8420091234544
images/blur_10.jpg - Not Blurry: 197.06995360732373
images/blur_9.jpg - Not Blurry: 127.99090228522351
images/blur_8.jpg - Not Blurry: 1242.7135491667214
images/good_9.jpg - Not Blurry: 2784.3464001240054
images/good_8.jpg - Blurry: 86.070335876096
```

The default threshold is 100, which you can define by self by adding more parameter just like this
```bash
python blur-detection.py --images images --threshold 1000
```
