# FoodVisor-TMM
Food classification using UPMC Food-101 dataset
## 1. The dataset
A dataset containing almost 100,000 images of 101 dishes collected from recipes websites on Internet. The dataset also contains the textual data from these website. For more information, please have a look at : <br />
http://visiir.lip6.fr/explore
## 2. Methods used
We try to classify the different dishes by fine-tuning the pre-trained models : **VGG16**, **Resnet18**, **InceptionV3**.<br />
We also try to classify the dishes by the textual features collected from the websites, we then do a fusion of the image classification and textual classification.
## 3. Results
After using several methods of data processing (data augmentation, rescale), we obtain the following results :<br />
- VGG16 :  **0.5242**
- Resnet18 : **0.6667** 
- InceptionV3 : **0.7217**

For the textual classification, we obtain an accuracy of **0.81** for a neuron network, **0.83** for the SVC Linear. <br />
The result after combining image and texutal features : **0.8637**.
