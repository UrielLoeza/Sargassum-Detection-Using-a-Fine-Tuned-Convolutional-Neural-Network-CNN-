# Sargassum Detection Using a Fine-Tuned Convolutional Neural Network (CNN)

This project was developed as part of the "Neural Networks" course and participated in a Kaggle competition titled "Clasifica el sargazo 24B", where the dataset is publicly available. The objective was to predict the level of sargassum presence on various beaches, categorized into five distinct rating levels.

A DenseNet201 model was fine-tuned for this task. Initially, the original classification head of the model was removed, as the dataset contains only five classes compared to the 1000 classes in the original ImageNet-trained model. Additional layers were then added to reduce the number of features and adapt the architecture to the target classes. These newly added layers were fully trained, after which the entire model was unfrozen and fine-tuned using a smaller learning rate to optimize performance.
