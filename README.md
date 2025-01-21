# 100-sports-classification
## overview
This project uses deep learning to classify images of 100 different sports. It is built using PyTorch and employs Convolutional Neural Networks (CNNs) for image classification. The model is trained on a custom dataset and achieves high accuracy in identifying sports based on visual features.
## dataset
The [dataset](https://www.kaggle.com/datasets/gpiosenka/sports-classification) consists of images from 100 different sports. Each image is labeled with the corresponding sport. The folder structure is:
/dataset
  /train
  /test
  /val
## training
To train the model, I first preprocessed the dataset by resizing the images to 232 and applying data augmentation techniques such as random rotations and flips to increase model generalization. I then chose resnet50 model as the base and fine-tuned it on the dataset using transfer learning. I utilized PyTorch for model implementation and training, and the training process was executed on a GPU for faster computation. During training, the model was optimized using the Adam optimizer, and the performance was monitored using accuracy and loss metrics. After training, the model's performance was evaluated using a test set, and the best-performing weights were saved for inference.

##Results
The trained model achieved an accuracy of 92% on the test set, demonstrating strong performance in classifying images across 100 different sports categories. During evaluation, the model was tested using metrics such confusion matrix, and classification report, which highlighted the model’s ability to accurately identify sports and differentiate between similar categories. The model performed well overall.
