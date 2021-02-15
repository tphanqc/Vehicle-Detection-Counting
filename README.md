# Video Analytics : Vehicle-Detection-Counting

Welcome to the Video Analytic repository for the vehicle-Detection-Counting challenges . This repo contains the definition of the environment where your code submissions will run. 

 ----

### [Getting started](#0-getting-started)
 - [Environnement](#environment)
 - [Problem description](#1-problem-description)
 - [Data resources](#2-data-resources)
### [Submission](#submission)
   - [Making a submission](#making-a-submission)
 
----

## (0) Getting started

### Environment

Libraries and versions with Python 3.8 have been identified to be used in order to ease the run of your submission to the challenge.

They are gathered in files py-cpu.yml or py-gpu.yml depending on whether you use a GPU for your work. These .yml files are available in the **_envs_** folder of this respository.

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

Traffic Counting is crucial for every traffic project. Traffic datas are collected from different sources : api, IoT, flat file, videos etc... They are transformed, analysed via differnt data process developed by our team. We're looking for a talented Data scentist to join our team to work for a new project video analytic. 
You have an excellent skill in this domain and have great experience in Deep Learning, Object Detection, Tracking and Counting, then we have a great place for you in this project. 

We want to learn more about you via the following topics. Please do not spend more than 1 day for each topic. 



 - Topic 1: Object detection (Required)
   
   - Useful folder for this topic: datasets/predict
   
   - The output expected for this topic is: 
     - a series of pictures with added drawing boxes identifying the cars, trucks and bus detected;
   
     - a separate .txt file where you mention the number of cars, truck and buses detected in the pictures associated with the corresponding picture filename (cars, trucks and buses counted and associated video name on one line, as many lines in the file as the number of videos you predicted on)
   
     - a script (ex : python) used for detecting number of cars, trucks and bus
   
 - Topic 2 (optional): Counting number of cars, bus and trucks appeared in videos
   
   - Useful folder for this topic: videos

   - The output expected of this topic is: 
     - a video with drawing boxes identifying cars, bus and trucks;
   
     - a separate .txt file where you mention the number of cars and trucks detected in the videos associated with the corresponding video filename (cars, trucks and buses counted and associated video name on one line, as many lines in the file as the number of videos you predicted on)
   
     - a python script for predicting on new videos
   
 - Topic 3 (optional): count number of cars in North Bound direction and right turn at the intersection ( you can assign a direction in each leg by yourself)

   - Useful folder for this topic: videos

   - The output of this topic is: 
     - a video with drawing trajectories identifying the cars and trucks detected going North Bound direction and turning right at the intersection;
   
     - a separate .txt file where you mention a number of cars, trucks and bus detected in the videos associated with the corresponding video filename (cars, trucks and buses counted and associated video name on one line, as many lines in the file as the number of videos you predicted on)
   
     - a python script for predicting on new videos

## (2) Data resources

Hundreds annotated pictures are provided in the "datasets/annotation" folder.

A set of pictures that you can use to test model in "datasets/predict". We'll use a similar set of picture to test your submission. 

A set of 3 videos (/videos) provided for testing your model of topic 2 and 3. The topics are optional/bonus for the submission. For the topics, we expect a minium description of your approach to creat a model for the topic.


### Formats

 - Yolo format : zip file contains the annotated files associated with the images.
   
 - CSV format : annotated csv of the images. 


### Vehicule Classification description

Motorcycles – All two or three-wheeled motorized vehicles. Typical vehicles in this category have saddle type seats and are steered by handlebars rather than steering wheels. This category includes motorcycles, motor scooters, mopeds, motor-powered bicycles, and three-wheel motorcycles.

Passenger Cars – All sedans, coupes, and station wagons manufactured primarily for the purpose of carrying passengers and including those passenger cars pulling recreational or other light trailers.

Other Two-Axle, Four-Tire Single Unit Vehicles – All two-axle, four-tire, vehicles, other than passenger cars. Included in this classification are pickups, panels, vans, and other vehicles such as campers, motor homes, ambulances, hearses, carryalls, and minibuses. Other two-axle, four-tire single-unit vehicles pulling recreational or other light trailers are included in this classification. Because automatic vehicle classifiers have difficulty distinguishing class 3 from class 2, these two classes may be combined into class 2.

Buses – All vehicles manufactured as traditional passenger-carrying buses with two axles and six tires or three or more axles. This category includes only traditional buses (including school buses) functioning as passenger-carrying vehicles. Modified buses should be considered to be a truck and should be appropriately classified.
## Submission your solution
- Topic 1 : Please submit all instructions and your script so we can test them locally. 
- Topic 2,3 : If you complete these topics, please submit all instructions and your script. We expect a description of your approach to do the topics if you don't have time to finish finish them.
- Under /submission folder create a folder with your name and push all your submission there : 
  - ex : Thomas_phan/
    - /topic1
    - /topic2
    - /topic3      

To submit your solution, please follow these steps to submit your code : 

 - Fork this repository
 - Make your changes
 - Test them and commit using git
 - Open a pull request to this repository

