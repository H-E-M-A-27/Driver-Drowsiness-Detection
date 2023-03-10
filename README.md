# Driver-Drowsiness-Detection
Driver Drowsiness detection using CNN and OpenCV
### Abstract:
<p align="justify"> 
Image classification and object detection are some of the most researched digital image analysis problems. Some of the image classification models using AI-based deep learning models have already surpassed humans in terms of data processing and accuracy. A cornerstone of these types of problems is the Drowsiness Detection problem. But what is often overlooked in the development of deep learning models for image classification and object detection test cases is the effect of optimizers. Most models use the Adam optimizer as a standard due to faster computation speed and it requiring fewer parameters for tuning. In this study, we compare the performance of different optimizers for the drowsiness detection test case. We use a dataset from the Medical Research Lab (MRL) with 48,000 images split into training and testing datasets. This dataset has infrared images of drivers’ eyes in different settings. We propose a CNN model given its advantage with image data feature extraction using the pooling and convolutional layers. The optimizers we use for this study are Adam, Adagrad, RMSProp, SGD, Adamax, and Nadam. Werunthemodelforasetnumberofepochsacrossalloptimizerstogetanideaofthe trends given our limited GPU capability. Training and validation losses are plotted for the models across optimizers using the categorical cross-entropy metric. Finally, we use the model selected in concurrence with OpenCV to employ our Drowsiness Detection System. This system increments a score variable for each second that the driver’s eyes are closed. When the score reaches a particular threshold, the system rings an alarm.
</p>

### Introduction:
<p align="justify">
Statistical surveys have relayed that in the past few years drowsiness-related accidents have remained constant even with the increase in information and countermeasures put in place. According to the National Highway Traffic Safety Administration, there are over 100,000 Police reported crashes and over 1,500 deaths due to drowsy driving. More than 40% of drivers have admitted that they have fallen asleep behind the wheel. Drowsiness can result in symptoms that significantly affect how well activities are performed, such as decreased response time or brief loss of consciousness. These symptoms are highly dangerous when driving since they greatly increase the likelihood of drivers crashing their cars and getting into accidents. This is the problem we propose to tackle with the help of an optimized deep-learning CNN model.
Good drowsiness detection is an essential first step in lowering the cost of road accidents to society. By implementing an effective drowsiness detection system in every vehicle, we will be able to prevent up to 274 accidents every day, which means we will be able to avoid 11 accidents every hour.
Our work has a research objective and a real-world application objective. The research objective is to analyze the performance of the model with different optimizers using validation accuracy and categorical cross-entropy loss. The real-world application objective is to develop a functioning drowsiness detection system with the best model achieved through the research objective. We will achieve the objectives by implementing a CNN model and training it on the available dataset using different optimizers for model compilation. Finally, we will select the model which gives the best performance and produces the lowest loss. With the selected model, we create a python file for drowsiness or fatigue detection. If the driver is drowsy, we ring an alarm to avoid any mishaps. There is also an attribute ‘score’ which is used to track the length of time a person closes his eyes in real-time. It is incremented when both eyes are closed and decremented when either or both eyes are open.
In comparison to other approaches, CNN models are highly efficient in preprocessing images without loss of information. This is why CNNs are used majorly for image classification use cases. We can also use supervised machine-learning algorithms for multiclass classification, such as SVM, Bayesian, and KNN Classifier. Since there are many classes when we are involved with real-time audio-visual data, these supervised machine algorithms fail to produce results with much accuracy or speed.
So, to summarize, we develop a CNN model and train it on a large corpus of images. Next, The trained model is compiled using different optimizers. We plot training loss, validation loss, and finally, implement the best model for the drowsiness detection system. Some of the limitations we encountered were low GPU capability and time-consuming training operations due to image preprocessing and input size.
</p>

### Optimizers used:
<ol>
<li>Adam</li>
<li>Nadam</li>
<li>Adagrad</li>
<li>Adamax</li>
<li>RMSProp</li>
</ol>

### Conclusion:
<p align="justify">
  In this work, we have obtained results for image classification of driver drowsiness based on the most prevalent optimizers used in CNN. The optimizer analysis was done using the exact same CNN model. The accuracy obtained by Adagrad was the highest with a validation accuracy of 80.53%, followed by Adamax with 79.57%, then Adam with 73.56%, followed by Nadam with 71.39%, and SGD with 68.27% and finally, RMSProp having the worst performance with 56.49%.
When it comes to categorical cross-entropy loss, the best performance was given by Adagrad with a validation loss of 5.5562, followed by SGD with 18.6988, then Adamax with 35.2122, then Adam with 38.6224, next being Nadam with 87.5950 and finally, RMSProp with 167.9985. We also implemented the drowsiness detection algorithm which performed well. We used the CNN model with Adagrad optimizer.
</p>

#### The dataset is in:
https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new
