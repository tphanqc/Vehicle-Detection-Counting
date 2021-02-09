# Video Analytics : Vehicle-Detection-Counting

Welcome to the Video Analytic repository for the vehicle-Detection-Counting challenges . This repo contains the definition of the environment where your code submissions will run. 

 ----

### [Getting started](#0-getting-started)
 - [Prerequisites](#prerequisites)
 - [Quickstart](#quickstart)
### [Testing your submission.zip](#1-testing-your-submissionzip)
 - [Implement your solution](#implement-your-solution)
 - [How your submission will run](#how-your-submission-will-run)
 - [Test running your submission locally](#test-running-your-submission-locally)
   - [Making a submission](#making-a-submission)
   - [Reviewing the logs](#reviewing-the-logs)
### [Updating the runtime packages](#2-updating-the-runtime-packages)
 - [Adding new Python packages](#adding-dependencies-to-the-runtime)
 - [Testing new dependencies](#testing-new-dependencies)
 - [Submitting a PR](#opening-a-pull-request)



----

## (0) Getting started

### Environment

[comment]: <> (Make sure you have the prerequisites installed.)

[comment]: <> ( - A clone or fork of this repository)

[comment]: <> ( - [Docker]&#40;https://docs.docker.com/get-docker/&#41;)

[comment]: <> ( - At least ~10GB of free space for both the training images and the Docker container images)

[comment]: <> ( - GNU make &#40;optional, but useful for using the commands in the Makefile&#41;)

[comment]: <> ( - [AWS CLI]&#40;https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html&#41; &#40;Optional, but useful for the `make sample-images` command which downloads images from S3&#41;)

[comment]: <> (Additional requirements to run with GPU:)

[comment]: <> ( - [NVIDIA drivers]&#40;https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html#package-manager-installation&#41; &#40;we check whether you have `nvidia-smi` installed and enabled to automatically determine whether to build the cpu or gpu image&#41;)

[comment]: <> ( - [NVIDIA Docker container runtime]&#40;https://nvidia.github.io/nvidia-container-runtime/&#41;)
Libraries and versions with Python 3.8 have been identified to be used in order to ease the run of your submission to the challenge.

They are gathered in files <mark>py-cpu.yml</mark> or <mark>py-gpu.yml</mark> depending on whether you use a GPU for your work. These .yml files are available in the **_envs_** folder of this respository.

The conda environment can be created, then activated by:


```
conda env create -f /envs/py-gpu.yml
conda activate py-gpu
```
or
```
conda env create -f /envs/py-cpu.yml
conda activate py-cpu
```

## (1) Problem description

<mark>Traffic Counting is crucial for every traffic project. Traffic datas are collected from different sources : api, IoT, flat file, videos etc... They are transformed, analysed via differnt data process developed by our team. We're looking for a talented Data scentist to join our team to work for a new project video analytic. 
You have an excellent skill in this domain and have great experience in Deep Learning, Object Detection, Tracking and Counting, then we have a great place for you in this project. 

We want to learn more about you via the following topics. Please do not spend more than 1 day for each topic. We expect to have a small model runing for topic 1, topic 2 and 3 are bonus. 

</mark>

 - Topic 1: Object detection 
   
   - Useful folder for this topic: <mark>datasets/predict</mark>
   
   - The output of this topic is: 
     - a series of pictures with added drawing boxes identifying the cars and trucks detected;
   
     - a separate .txt file where you mention the number of cars and trucks detected in the pictures associated with the corresponding picture filename (cars count and associated image name on one line, as many lines in the file as the number of pictures you predicted on)
   
     - the python script for predicting on new images
   
 - Topic 2: Count number of car and truck appeared in videos
   
   - Useful folder for this topic: <mark>videos</mark>

   - The output of this topic is: 
     - a video with drawing boxes identifying the cars and trucks detected;
   
     - a separate .txt file where you mention the number of cars and trucks detected in the videos associated with the corresponding video filename (cars count and associated video name on one line, as many lines in the file as the number of videos you predicted on)
   
     - the python script for predicting on new videos
   
 - Topic 3: count number of cars in direction North bound after a right turn

   - Useful folder for this topic: <mark>videos</mark>

   - The output of this topic is: 
     - a video with drawing boxes identifying the cars and trucks detected going North after a right turn;
   
     - a separate .txt file where you mention the number of cars and trucks detected in the videos associated with the corresponding video filename (cars count and associated video name on one line, as many lines in the file as the number of videos you predicted on)
   
     - the python script for predicting on new videos

## (2) Data resources

Around <mark>thousand</mark> annotated pictures are provided in the **_datasets/train_** folder.

A set of pictures to predict on and provide the output as stated in "Topic 1".

3 videos for topics 2 and 3.

### Formats

 - Yolo format

<mark>lorem ipsum</mark>
   
 - CSV format

The **_train_annotations.csv_** contains the following information:

<mark>annotation_id - a unique identifier for each annotation</mark>

<mark>filename - the slide image corresponding to each annotation; each image contains multiple annotations</mark>

<mark>geometry - x, y coordinates of the annotation in WKT format; all geometries are closed rectangles. NOTE: x,y coordinates assume origin is bottom left corner of the image.</mark>

<mark>annotation_class - the class of the annotated tissue

### Classes description
<mark>c</mark>
