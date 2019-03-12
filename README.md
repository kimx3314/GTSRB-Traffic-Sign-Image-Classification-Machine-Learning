# Advanced Machine Learning
### GTSRB Traffic Sign Image Multi-class Classification
with Python

by Sean Sungil Kim

Jupyter notebook coming soon, March 19th

Computer Vision is utilized in many fields that deploy IoT devices. The purpose of Computer Vision would include but not only be limited to many image detection and recognition aspects. For example, successfully classifying traffic signs given image data of traffic signs could benefit vehicle companies tremendously. To be able to classify traffic signs with significant performance, finding the optimal model with corresponding hyperparameters is important. Therefore, implementing machine learning algorithms in addition to analytical algorithms is necessary. Algorithms such as Random Forest, ADAboost, Neural Networks, XGBoost and other classifiers will be used to compare model performances in this project.

The goal of this traffic sign image multi-class classification analysis is to explore the effectiveness of different classifiers on lower quality (both in dimension size and color), non-centered traffic sign image (researched and provided by INI Benchmark, which can be downloaded here: http://benchmark.ini.rub.de/?section=gtsrb&subsection=dataset). Image data are heavy both in terms of size and processing time required. It is also difficult to obtain carefully cenetered image data (regardless of what the images are of) in the real world. Having high quality, colored and perfectly centered images can enhance the effectiveness of machine learning and statistical algorithms. However, this requires a significant amount of time, both in the front and the back end. Utilizing lower quality image data is extremely beneficial when computing power is very limited. In addition, being able to use not-so-perfectly cenetered images can save a lot of time. Combining these two factors together, the lower quality and non-centered image data can excel in extremely time sensitive and limited computing power environments, which are not hard to find in the real world.

The original GTSRB data is in fact not low quality. Each image is clear and decently sized (which explains the file size of the training and testing dataset provided on the INI website). It also provides the location of the actual traffic signs within each image in the annotation csv file. Since the goal of this project is to classify low quality traffic signs, each image is resized (downsized) to 16 x 16 pixels and the annotation csv file was not used. Original images are not the same size (sizes vary between 15x15 to 250x250 pixels); however, it did not affect this project since all of them were downsized to 16x16. Because of this size inconsistency, some images with bigger dimensions may have more information than the smaller images post downsizing. The INI Benchmark also provides HOG and haar-like precomputed features. These were not utilized in this project. Everything was started from scratch. Due to my personal limited computing power and time, only the GTSRB training set was used in this project. In the training data alone, there are 39,209 images and total 43 classes.
