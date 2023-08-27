# Behneshan
First Persian Educational Software for Teaching Persian Sign Language to Deaf Children


## Brief explanation on what this software is basically is 
One of the main concerns today in the field of education is choosing the right learning method to increase the quality of learning in people, especially for children. Games and entertainment, especially computer games, can be an alternative and practical solution to motivate children's learning.
The need to use such new methods in education, especially in teaching sign language to deaf and hard of hearing children, is felt. Due to their disability, these children will need specialized and at the same time innovative training in order to motivate them and make them interested in education and a stronger presence in the society.
In this project, an attempt has been made to design a module for identifying and tracking pointing movements by using Mediapipe and OpenCV libraries and combining them with LSTM neural network, and finally with the benefit of pygame (Python language game engine) a platform game in In order to motivate deaf children, improve the quality and modernize the education system, especially education for the deaf and hard of hearing. The database collected in this research consists of 24 signs and 60 videos have been prepared for each of them as training and test data. The sample in this study was only one male, and of course, in future studies and in the process of product commercialization, samples with physical characteristics different from the requirements of the study will be considered.


&nbsp;
&nbsp;

## Statement of Purpose
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/8f3a3855-586e-4a6c-b39a-b2ff20e3141f)
&nbsp;
In our country, Iran, there is a population of more than half a million deaf and hard of hearing people, and about 7% of this population are children. Deaf children, like other deaf people, still learn this skill through traditional methods such as integrated teaching method and Farsi sign with the help of professors fluent in this language.
Teaching sign language based on traditional methods has some drawbacks, among the most important of which we can mention the lack of educational facilities and the way the teacher communicates with the deaf person.
In this research, by designing an educational game, we have taken a step towards eliminating the current educational limitations and modernizing the Persian sign language education system.

&nbsp;
&nbsp;
## Main Purpose
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/22f3adcc-729b-46f7-971a-d5677aefc4e9)
&nbsp;
The purpose of this research is to design a game to teach Persian sign language to children. Education in the form of games increases motivation in children, which will have a significant impact on better learning and increase productivity during their education. Also, education through computer games will have a great impact on reducing children's education costs, which can be very important in the implementation of this project in deprived areas and especially for low-income communities.

&nbsp;
&nbsp;
## Innovations
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/4d2c99e7-9f83-410d-b9c3-9968671c52a0)
&nbsp;
Among the innovations of this research, we can mention the reduction of physical and material limitations by removing motion sensors and replacing them with a combination of diagnostic algorithms and machine vision techniques.
On the other hand, by using the LSTM neural network and designing a model based on machine vision techniques, the final system will have the ability to accurately and real-time detect and track body movements when performing Persian sign language signs, and thus, according to the quality And the level of accuracy of the final model, it can be used as a software for teaching Persian sign language.

&nbsp;
&nbsp;
## Mediapipe
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/5c8ffba3-8e64-4b9f-ab17-902162da9e81)
&nbsp;
Mediapipe is a human movement detection algorithm with the help of which it will be possible to identify and track the human body using machine vision techniques. Among the capabilities of this algorithm, we can mention hand, body and face recognition. After identifying the body physics, this algorithm divides the user's anatomy into 33 separate points and allows the user to access the location of each of these points to apply commands in his program. After processing by this algorithm, the hand skeleton is divided into 21 separate points and the user has the possibility to display the connection lines of different joints in the webcam output window in addition to displaying these points.

&nbsp;
&nbsp;
## Holistic Algorithm
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/00926146-52f5-46ef-a7b6-b2e6a1617d1b)
&nbsp;
The holistic algorithm is another example of the detection algorithms of the Mediapipe library. This algorithm is created from the combination of hand, body and face recognition algorithms and finally gives the user access to all the marker points resulting from the combined algorithms. The output of this algorithm will include the location of 468 points indicating the face, 42 points indicating both hands and 33 points indicating the body's physique in all three horizontal, vertical and depth directions.

&nbsp;
&nbsp;
## Data Acquisition
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/f2dae986-5398-4f6a-91f9-3fead45e0547)
&nbsp;
The database collected in this research includes 24 signs of Persian sign language. For each badge, 60 videos are prepared as input data. Each video consists of 30 frames, and each frame will contain a list of locations of body markers by the holistic algorithm, which includes a total of 1662 key points.

&nbsp;
&nbsp;
## Methodology
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/d50ab061-fe2f-46e3-9a59-43fee592ec84)
&nbsp;
The process of designing the model is that first, training data in the form of points indicating the position of the body's body are collected through the Mediapipe algorithm and sent as input data to the LSTM neural network. The selected neural network trains the final model by placing 85% of the data in the database as training data and 15% as test data after 2000 iterations and identifies the person's actions through it. . The selected neural network consists of 3 LSTM layers and 3 dense layers. The number of units placed in the last layer is determined by the number of signs in the research and finally after training the model, about 600 thousand parameters are obtained in the form of training parameters, which is much less than the number of parameters obtained from training through convolutional neural network and There have been other neural networks, which is why the speed of the final model in diagnosis is much higher than other algorithms.

&nbsp;
&nbsp;
## Software 
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/a62d8787-f3c6-4102-a0e3-10904d41057e)
&nbsp;
In this slide, there are pictures of the program's main menu and its training section. There are 5 options in the main menu, which include 3 keys and 2 labels. The keys are for entering the training section, entering the game section and exiting the program, respectively. The first label shows the highest score of the child from the game and the second label shows the learning rate of the marks determined in the database of this research by the child.
After entering the education section, pictures of the correct implementation of the signs learned by the child are placed next to their written equivalent.
After entering the training section and selecting the webcam option, the user's webcam is activated and an image is displayed in its output window through which the child can see the correct implementation of the gesture equivalent to the Persian word written in the same image and after The correct implementation of that next sign will appear for him.
After leaving the education section, an e-mail indicating the child's educational status will be sent to his parents.

&nbsp;
&nbsp;
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/d4d740bc-52cb-4662-aa8a-cae47c148317)
&nbsp;
In this slide, there are pictures of the game environment. The challenges in the game scene have gradually increased and this will make the game more attractive for children. If the game character collides with the enemy or lava while passing the stage, the character will be destroyed and the start screen will be displayed again, and if the restart option is selected, the stage will be reloaded. If the stage ends, meaning the character reaches the exit gate, the webcam is activated and an image is displayed. If the gesture corresponding to that image is executed correctly, the next stage of the game will be loaded.
Finally, after exiting the game, an email will be sent to his parents about the status of the game played by the child, in which the number of words learned, which means the number of steps passed, are attached along with the duration of his game.

&nbsp;
&nbsp;
## Convergence charts
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/ee28313c-420f-4154-85ba-4c8656ae6919)
&nbsp;
In this slide, the convergence diagrams resulting from model training on the LSTM neural network are displayed. As can be seen in Figure 19 a, the model has reached 96.8% accuracy after 2000 repetitions during the training process, which shows the proper performance of the model during training.
The cost function, which indicates the correctness of the model's performance, finally reached the value of 0.08 after 2000 repetitions, which is an acceptable figure for a model with this amount of training data, and it can be said that the performance of the model in the training process is somewhat It will be perfect and the implemented logo will be recognized correctly.

&nbsp;
&nbsp;
## Future Suggestions
![image](https://github.com/Yazdan-Ghanavati/Behneshan/assets/137007531/f9f96f03-ebbe-413c-ac0a-66b6a59b653b)
&nbsp;
In future researches, it is possible to increase the child's understanding of how to correctly perform each sign by replacing the educational images with videos of the correct execution of each sign.
Recording the training data in an environment with complex backgrounds and in different locations can avoid the disturbance during the recognition of user-implemented badges.
Using child samples while recording training data can have a significant impact on the final performance of the model.
Finally, designing more stages and adding new challenges in the game scene can have a great impact on the level of fun and attractiveness of educational software for children.

&nbsp;
&nbsp;
## Notes
Hey Guys,
I am glad to say that this project which at the time was my B.Sc. Capstone Project, is now updated in a new level which can detect more efficiently and is currently being reviewed by some sponsers for a demo version.
About the database, I have to say that I would be more than happy to share it with you but please understand that because of the copyright rules I cannot share it online, though, I would be more than happy to share it with you if it would help you to maybe challenge or test your trained neural network, so feel free to contact me via email for more informations.
