# Final_Project_2040
This repo created for final project DATA2040 at Brown University

This project is motion recognition using HMDB, a large human motion dataset create by brown univeristy (https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/). The dataset contain 51 classes video clips with intotal 6849 clips such as smile, laugh, talk, smoke etc. Our goal is to build a model that can predict given video's class from these 51 classes.
We split data into train test split, and train test validation split, which test is for ensemble models. Using bi-directional LSTM boost our model performance. Ensemble method boost our model performance from accuracy 0.68 to 0.74. Due to the time and computing resources, we tried from 4 classes, 9 classes, 16 classes, 25 classes and finally trained on 51 classes. 4 classes model can have a accuracy as high as 0.91 without overfitting issue. Although witht class increase, overfitting issue appear, our method is using data augmentation to increase input variety.
The future work can be writing data into TFRecord files for easier loading and faster training, train more models for ensemble methods as it is efficient.
