# Flower

## Introduction 
Flower is a streamlit application for a specific client that is in need of an Machine learning model that can see patterns between healthy cherry leafs and powdery mildew infected leafs. With Flower our client will be able to examinate cherry leafs and understand the infection better wich will help us to understand the world we live in. 

## Project descirption 
Flower is a streamlit app that is empowerd by ML 

## User demographic 
* Flower is created for a specific client that is intrested in conducting a study ti visually differentiate a cherry leaf that is healthy from one that contains powdery mildew
* The client is also intrested in predicting if a cherry leaf is healthy or contains powdery mildew. 

## Functions 

The project has a machine learning model suited for the clients need. 

# We have 4 diffrent apps inside our streamlit application 
## Qucik project Summery
 On this Page we describe the project where we talk about general information about the fungal disease "Powdery mildew". We also explain where we got the sampels for the machine to learn from. 
![img of landingsite](img/leaf%20detector%20landning.png)
## Leaf Detector 
 In leaf detector the client is able to drop a PNG file that will be scanned by the machine and try to figure out if the leaf is infected with mildew or not. The Client will also get a graph.
![img of detector site](img/leaf%20detector%20detect.png)
## Project Hypothesis 
 In "Project Hypothesis" the client will be able to read our hypothesis and validation about the project. We also added pictures from the Jupyter notebook we got back where the machine found the avg image for healthy and infected leafs with an explanation in the end. 
![img of hypo site1](img/project%20hyp1.png)
![img of hypo site2](img/project%20hyp2.png)
## ML Performance Metrics 
 On this side the client will be able to see how the machine learned and the preformence. We also added the graph of how we devided all pictures from the dataset for "training, validation and test". 
In the end you will also see the Generalised Performance test where we have an accuracy of 0.9929% wich is something we are very proud of and can stand behind. 
![img of ML performance metrics](img/ml%20performance.png)


## How we created the ML 


* We used Jupyer notebooks to create an ML. We started with downloading the Dataset we got from Kaggle https://www.kaggle.com/datasets/codeinstitute/cherry-leaves. We cleaned the Dataset from objectivs and files that weren't image files. 

* DataVisualization: In the second Jupyter notebook we started to learn more about the datasets images. We started to look at the average img size. 

* Modelling and evalutation: Here we devided the images in to train, validation and test set. After that we trained the model and looked at the evalutation to see if the machine found any patterns. After we saw the learning curv for the ml we concluded that the ml is ready.



## Deployment 
We deployed our project to heroku. 
1. log in to heroku
2. Create new app
3. Set europe and a name 
4. Change the stack from Heroku-22 to Heroku-20 
5. Then we went back in the terminal used the "Git push heroku main" command.
6. Deployed.

## Bugs 
When we were going to deploy to heroku we got an error that told us to downgrade our protobuf to 3.20.0 or belov so we did that. Because we downgraded our protobuf all the other programs were incompatible so we went in to the walkthrough project with the malaria infected blood cells and took the req.txt from there and then it worked to deploy it to heroku. 

After we changed the req.txt file we stombeld upon an another bug with the Leaf detector... Because we changed the version for the tensorflow in the req.txt we get this bug. We used another version of tensorflow when we created the machine learning model inside the jupyter notebook wich i belive create this bug.
![alt](img/leaf%20error.png)

## Credit 
I used the method for the ml from the malaria walkthrough but to match my needs so I have to give credit to the Malaria walkthrough. 
I also give credit for the Dataset from Kaggle https://www.kaggle.com/datasets/codeinstitute/cherry-leaves.

Thanks to Heroku's website wich is alot of help when you are in need of help when deploying to heroku. 