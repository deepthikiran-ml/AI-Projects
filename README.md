# AI-Projects
Our proposal is to recommend yoga exercises and come up with a yoga schedule based on the symptoms observed.
The application takes the symptom parameters as input and map this to the problem such as sinusitis, 
thyroid, ergonomic pain (pain caused due to bad posture), heart problem, allergy, sports injury etc. 
It  then proposes suitable yoga postures and exercise schedule to help heal the situation.


Dataset 
comprises of symptoms of common diseases. 
Each disease can have multiple symptoms.
Dataset consists of 5000 samples which spans around 35 diseases which is mapped to 233 symptoms 
The sources for these dataset are form the popular medical websites 
https://www.mayoclinic.org/
 https://www.webmd.com/ 
Dataset is in the form of a csv file.

Model   
Multinomial Naïve Bayes classifier is used for model training.
 Bayes theorem is 


Accuracy of 99.99% is achieved in the model.
Tried training the dataset on multiple models like Logistic Regression & chose the best fit.

To get effective results from this trained model, the below decision tree is enabled
If the confidence level ( of matching symptoms) is below 20%, then no disease can be inferred
If the confidence level is greater than 70%, then one disease can be perfectly diagnosed.
If the confidence level is between 20 to 70%, then more than one disease can be diagnosed.
A dictionary mapping of the disease to asanas is creating which will predict the yoga schedule for the diseased.
