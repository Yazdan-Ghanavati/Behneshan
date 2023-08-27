# Behneshan
First Persian Educational Software for Teaching Persian Sign Language to Deaf Children


## Abstract 
One of the main concerns today in the field of education is choosing the right learning method to increase the quality of learning in people, especially for children. Games and entertainment, especially computer games, can be an alternative and practical solution to motivate children's learning.
The need to use such new methods in education, especially in teaching sign language to deaf and hard of hearing children, is felt. Due to their disability, these children will need specialized and at the same time innovative training in order to motivate them and make them interested in education and a stronger presence in the society.
In this project, an attempt has been made to design a module for identifying and tracking pointing movements by using Mediapipe and OpenCV libraries and combining them with LSTM neural network, and finally with the benefit of pygame (Python language game engine) a platform game in In order to motivate deaf children, improve the quality and modernize the education system, especially education for the deaf and hard of hearing. The database collected in this research consists of 24 signs and 60 videos have been prepared for each of them as training and test data. The sample in this study was only one male, and of course, in future studies and in the process of product commercialization, samples with physical characteristics different from the requirements of the study will be considered.


&nbsp;
&nbsp;

## Data Acquisition
In this section, the goal is to create a database in the form of a list of arrays containing key points obtained from the Holistic algorithm. All identified points are added to the final list in the form of an array, and if the points are not visible, an array of zeros is recorded as the location of that point. In this way, the output array will have a value for each of the body pointer points. The arrays stored using the flatten() command will all have dimensions of 1*n, where n indicates the points of the indicator extracted from the special algorithm multiplied by the dimensions of each of the points.
&nbsp;

The final array is the joining of four arrays for detecting the body, face, right hand and left hand. Since this algorithm divides the body into 33 separate points with four characteristics, the body array will have dimensions equal to 1* (33*4). The facial recognition algorithm identifies 468 points, each of which has three characteristics. Therefore, the dimensions of this array will be equal to 1* (3*468). Each of the hands contains 21 points and each of these points has dimensions in three horizontal, vertical and depth axes; As a result, the final array obtained from each hand will have dimensions equal to 1* (3*21). The final array has dimensions equal to 1662x1. The figure below shows the implementation of the selected signs, in order to collect a database of a group of signs determined by the researcher


![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/50b29e56-2ca5-4f54-b5c1-aa4104df299e)

![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/17d267e3-2588-48d0-80a0-20ab51279c7f)

&nbsp;
&nbsp;
