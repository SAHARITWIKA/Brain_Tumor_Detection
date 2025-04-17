pred
prediction:
read the image and classify that tumor is there or not.

dataset
2sub part yes and no 
classified images stored . 

mainTrain
keras is a api , used for solving ml algo .

1. directory set up.
2. os reader made that is yes_tumor, no_tumor . to seggregate yes and no tumors. 
3. by default image size 64 bits . we take it as 64 bit has better clarity over 32 bit image.  
4. train_test_split use for training the module , testing the module and splitting them into 2 sub directory . 
5. random_state=0 state 0 means the model is not trained yet .
6. relu -> rectified linear unit , used to activate artificial neural network and helps to learn model which use cnn (keras) .
7. kernel_initializer='he_uniform'    -> use to get a uniformly splitted image .(keras)
8. softmax  -> when we want to find specific data from within an image or dataset without using it as a whole (keras) .
9. cross_entropy-softmax -> a measure of the difference between two probability distributions.
10. adam ->optimizer
11. verbose=1 ->gives realtime feedback of module performance 
12. epochs=10 ->cutoff , used to determine how many time trainning continue.
 


mainTest
output 0 mean no tumor 
output 1 mean tumor 

-> mainTrain line 32,40 that is label.append we classify that .


BrainTumor10EpochsCategorical.h5

h5 heirerchial dataformat 5 
used for store large amount of data  in the form of multi dimensional heirerchy or arrays .

model:
In Keras, a Sequential model is a linear stack of layers, where each layer's output is fed as input to the next. It's suitable for simple, single-input, single-output architectures.


argmax:
np.argmax()
Returns the indices of the maximum values along an axis.
-> to get sequential data in a specific axis in a multi dimentional array.