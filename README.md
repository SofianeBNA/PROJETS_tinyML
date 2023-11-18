# PROJETS_tinyML

This project goal was to create a model which will be able to recognize vibrations coming from a washing machine on. To create my dataset, I used my arduino for collecting datas. 3 labels were produced : Off, light load and heavy load. I simulated those vibrations by putting my arduino on a table and I hit the table with different strengths to produce theses vibrations. I put my dataset on Edge Impulse for the model creation. I collected datas coming from the gyroscope and the accelerometer and that was on the 3 axes (x,y,z). About the split, I took 1 minutes for each label for the training and only 20s for each label and that was for the test. I thought that was a bit short, I'll recommend someone to add more datas for the test set and also the training set. 


I put a spectral analysis to see those datas and tried to understand them. I also added a anomaly detection (k-means) and a classifier for my model and I trained it. 

The anomaly detection gave me pretty good results and the classifier gave me 100% of accuracy. I thought at this moment that the model was overfitting (Thats why I considered that adding datas will improve my model).
Then I tested the model and I got around 90% for the accuracy. That is why I deployed it into my arduino and I tested the program, the results were good and the model worked well.


Here's the arduino code and the arduino library containing my model.
