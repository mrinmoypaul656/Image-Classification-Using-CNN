# Image-Classification-Using-CNN
Step by Step Analysis
1.	Loading Data
2.	Pre-processing
3.	Build Model
4.	Evaluate Model
5.	Predict
Next, I imported different Libraries like pandas, numpy, keras, matplotlib, tensorflow. Loading the data was done by importing the dataset cifar10 from keras module
Next I crosschecked the different shapes of x_train, y_train, x_test, y_test..
Next I tried to show some basic datas which were present in the dataset
Next a bit of preprocessing of the model is done
Then I started building the model,
In the model,  I used 2 Conv2D laeyrs and 2 Maxpool2D laeyrs to have better accuracy and also to check whether the model doesn’t overfit the data, In the next layer I added a Flatten and used 3 activation function of Relu and the final Activation function as softmax as we have multiple classes in the data. In Each of the dense Layers, I used the Dropout of 0.2
Here in this model I went for loss function of Categorical_crossentropy and optimizer as adam considering the facts that these will fit the model perfectly
In the model I went for an earlystopping for the parameters being val_loss and patience=3.
Next I used an epoch of 20 and batch size of 128 and fitted the model with data’s present of the testing set.
What I noticed is that with each epoch that both the loss and validate_loss was decreasing and the accuracy and the val_accuracy was increasing which I also plotted in the graph.
