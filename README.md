# Humpback-Whale-Identification

## 1. Introduction

This project is focus on identify 5005 different categories whale based on their tail images. 

After centuries of intense whaling, recovering whale populations still have a hard time adapting to warming oceans and struggle to compete every day with the industrial fishing industry for food.

To aid whale conservation efforts, scientists use photo surveillance systems to monitor ocean activity. 
They use the shape of whales’ tails and unique markings found in footage to identify what species of whale they’re analyzing and meticulously log whale pod dynamics and movements. 
For the past 40 years, most of this work has been done manually by individual scientists, leaving a huge trove of data untapped and underutilized.

In this project, some of the categories picture with only several number. 

In the model, I try to fix data insufficient problem also as to overcome overfitting. 
Furthermore, to transfer this model in some business area overcome data insufficient problem.


## 2. Enviorment and Packages

This project use following packages:

*  numpy
*  pandas
*  matplotlib
*  sklearn
*  keras

## 3. Significance and Approach

Import the image as pixal data and reshape the data. 

First build 2 layers CNN model, each layer with conv, pooling and activation.

Second build 3 layers CNN model, each layer with 2 convs, pooling, dropout and activation. 

Further, build transfer learning model based on Resnet50 and MobileNet. Applyed ImageDataGenerator for data augmentation. 


## 4. Repository Structure

*  Input Data
*  Output Result
*  Source Code
*  Report
