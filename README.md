# Flower

## Introduction 
Flower is a Streamlit application for a specific client that needs a machine learning model to identify patterns between healthy cherry leaves and powdery mildew-infected leaves. With Flower, our client will be able to examine cherry leaves and understand the infection better, which will help us understand the world we live in.

## Project descirption 
Flower is a Streamlit app powered by machine learning.


## User demographic 
* Flower is created for a specific client interested in conducting a study to visually differentiate a healthy cherry leaf from one infected with powdery mildew.
* The client is also interested in predicting if a cherry leaf is healthy or contains powdery mildew.

## Functions 

The project has a machine learning model suited to the client's needs.

# We have 4 diffrent apps inside our streamlit application 
## Qucik project Summery
 On this page, we describe the project and provide general information about the fungal disease "Powdery Mildew." We also explain where we obtained the samples for the machine to learn from. 
![img of landingsite](img/leaf%20detector%20landning.png)
## Leaf Detector 
 In Leaf Detector, the client can drop a PNG file that will be scanned by the machine to determine if the leaf is infected with mildew or not. The client will also receive a graph.
![img of detector site](img/leaf%20detector%20detect.png)
## Project Hypothesis 
 In "Project Hypothesis," the client can read our hypothesis and validation about the project. We also added pictures from the Jupyter notebook showing the average image for healthy and infected leaves, with an explanation at the end.
![img of hypo site1](img/project%20hyp1.png)
![img of hypo site2](img/project%20hyp2.png)
## ML Performance Metrics 
 On this page, the client can see how the machine learned and its performance. We also added a graph showing how we divided all pictures from the dataset into "training," "validation," and "test" sets.
In the end, you will also see the Generalized Performance test where we have an accuracy of 99.29%, which is something we are very proud of and stand behind. 
![img of ML performance metrics](img/ml%20performance.png)


## How we created the ML 


* We used Jupyter notebooks to create an ML model. We started by downloading the dataset from Kaggle: https://www.kaggle.com/datasets/codeinstitute/cherry-leaves. We cleaned the dataset by removing objects and files that weren't image files.

* Data Visualization: In the second Jupyter notebook, we started to learn more about the dataset's images. We looked at the average image size.

* Modeling and Evaluation: We divided the images into training, validation, and test sets. After that, we trained the model and evaluated it to see if the machine found any patterns. After analyzing the learning curve for the ML model, we concluded that it was ready.



## Deployment 
We deployed our project to heroku. 
1. log in to heroku
2. Create a new app
3. Set Europe as the region and choose a name 
4. Change the stack from Heroku-22 to Heroku-20 
5. In the terminal, use the "Git push heroku main" command.
6. Deployed: https://blooming-garden-64545-53ac3eb0c98d.herokuapp.com/

## Bugs 
When we tried to deploy to Heroku, we got an error that told us to downgrade our protobuf to 3.20.0 or below, so we did that. Because we downgraded our protobuf, all the other programs were incompatible, so we referred to the walkthrough project with malaria-infected blood cells and took the requirements.txt from there. Then it worked to deploy to Heroku.

After we changed the requirements.txt file, we encountered another bug with the Leaf Detector. Because we changed the version of TensorFlow in the requirements.txt, this bug appeared. We used another version of TensorFlow when we created the machine learning model inside the Jupyter notebook, which I believe caused this bug.
![alt](img/leaf%20error.png)

## Credit 
I used the method for the ML model from the malaria walkthrough but adapted it to match my needs, so I have to give credit to the Malaria walkthrough.
I also give credit to the dataset from Kaggle: https://www.kaggle.com/datasets/codeinstitute/cherry-leaves.

Thanks to Heroku's website, which is very helpful when you need help deploying to Heroku.

