**Recyclable and Household Waste Classification Agent**



*Group Members*



Aleksander Murati - Research regarding the dataset, data preprocessing.

Era Malaj - Worked on the CNN Model and the rule-based agent, worked on the powerpoint and assembling results, comparison.

Emi Brahaj - Worked on the Random Forest and Decision Tree models alongside assistance with showing the CNN graphs, QA.



***Project Overview***



This project implements an intelligent waste classification agent that automatically identifies household waste items from images and recommends the correct disposal bin.

The system combines statistical learning and neural network–based perception, satisfying the course requirement of integrating multiple AI techniques.



The agent first classifies waste images into one of 30 waste categories and then applies rule-based reasoning to map each predicted class to an appropriate disposal bin (Plastic, Paper, Glass, Metal, Organic, or Trash).



***Dataset***



Dataset Name: Recyclable and Household Waste Classification (https://www.kaggle.com/datasets/alistairking/recyclable-and-household-waste-classification/data)



Source: Kaggle



Size: 15,000 images



Classes: 30 waste categories



Structure: Images organized into class-based folders



Images were resized to 64×64 RGB, normalized to \[0,1], and split into training and testing sets using stratified sampling.



***AI Techniques Used***



1\. Statistical Learning



Random Forest Classifier



Decision Tree Classifier



These models operate on flattened image features and provide strong baselines for multi-class classification.



2\. Neural Networks



Convolutional Neural Network (CNN)



The CNN learns spatial features directly from image pixels using convolution and pooling layers, followed by fully connected layers for classification.



3\. Rule-Based Reasoning



A rule-based module maps predicted waste classes to disposal bins, simulating an intelligent agent that combines perception and action.



***Model Evaluation***



Models were evaluated using:



Accuracy



Precision, Recall, and F1-score



Confusion matrices



The CNN achieved approximately 60% test accuracy, while the Random Forest achieved approximately 63% accuracy, highlighting the trade-off between classical machine learning and deep learning approaches on limited-resolution images.



***Ethical and Societal Considerations***



This system can contribute to improved waste sorting and recycling efficiency, reducing environmental impact.

However, incorrect classifications may lead to improper disposal, emphasizing the need for human oversight in real-world deployment.





***Installation and Dependencies***



Python Version = Python 3.10.3

Jupyter Notebook was used to run the code.



***Required Libraries***



***Main dependencies:***



numpy



scikit-learn



tensorflow



pillow



matplotlib



seaborn



***Running the Project***


Ensure the dataset(the subfolders, such as aerosol, trash, etc) is placed in the images/ directory, which is then placed in a folder with the ipynb file. (Please make sure only ONE images folder is present. It should be one images folder, which leads directly to the data.)


Activate the virtual environment.



Run the notebook or Python scripts.



Models will train, evaluate, and output classification results and confusion matrices.



***Reproducibility***



All experiments can be reproduced by running the provided code with the same dataset and dependencies listed above.


