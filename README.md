# Fire-and-Smoke-Classification-Transfer-Learning

Special thanks to Adrian Rosebrock as his [article](https://www.pyimagesearch.com/2019/11/18/fire-and-smoke-detection-with-keras-and-deep-learning/)  has provided the basic tutorial for the implementaion of model to detect fire. 

In addition to guidance from above, I have incorporated the concept of Transfer Learning, details of which can be leared from [here](https://keras.io/guides/transfer_learning/). 

In this project, the base model from Xception Net is employed with custom top layers. The base model has been frozen and only the top layers are trained on Classification of Fire/Smoke and Non-Fire Images. Then during the fine-tune run, whole model is unfrozen and trained with very small learning rate. 


## Dataset 
The dataset used in this project has been collected from various sources which include:
* https://github.com/cair/Fire-Detection-Image-Dataset
* http://smoke.ustc.edu.cn/datasets.htm
* https://www.kaggle.com/phylake1337/fire-dataset
* https://github.com/breed2137/fire_dataset

The final dataset is provided below:
* [Training-FireImages](https://drive.google.com/file/d/19cDIEM0E9HA0raoPSzg0dpyeQRSHy9vz/view?usp=sharing)
* [Training-NonFireImages](https://drive.google.com/file/d/1NG2Eo8rBdSvyITl0Xrud7NXV-TyJFHc6/view?usp=sharing)
* [TestData](https://drive.google.com/file/d/1yfylkft_Dw2Yayn2gbhtELjq0awYYnV9/view?usp=sharing)

## Training
![image](https://user-images.githubusercontent.com/61320147/116779300-ee003100-aa8e-11eb-90ca-9de7c3bffe62.png)

## Results
Train accuracy=98% \
Cross-Validation accuracy=97% \
Test accuracy=97-96% 

Results on Test Dataset: \
![image](https://user-images.githubusercontent.com/61320147/116779511-002e9f00-aa90-11eb-8f4b-e3003b525ab1.png)
