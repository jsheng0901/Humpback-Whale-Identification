## Learning Algorithm

CNNs are regularized versions of multilayer perceptrons. Multilayer perceptrons usually mean fully connected networks, that is, 
each neuron in one layer is connected to all neurons in the next layer. 
The "fully-connectedness" of these networks makes them prone to overfitting data. 
Typical ways of regularization include adding some form of magnitude measurement of weights to the loss function. 
However, CNNs take a different approach towards regularization: 
they take advantage of the hierarchical pattern in data and assemble more complex patterns using smaller and simpler patterns. 
Therefore, on the scale of connectedness and complexity, CNNs are on the lower extreme.

Convolutional networks may include local or global pooling layers to streamline the underlying computation. 
Pooling layers reduce the dimensions of the data by combining the outputs of neuron clusters at one layer into a single neuron in 
the next layer. Local pooling combines small clusters, typically 2 x 2.
Global pooling acts on all the neurons of the convolutional layer.
In addition, pooling may compute a max or an average. 
Max pooling uses the maximum value from each of a cluster of neurons at the prior layer.

Transfer learning is a research problem in machine learning that focuses on storing knowledge gained while solving one problem 
and applying it to a different but related problem. 
For example, knowledge gained while learning to recognize cars could apply when trying to recognize trucks. 

## Model Summary

The first and second model use basic CNN model depends on conv, pooling and dropout. The average accuracy is near 0.67.
The rest model I use Resnet50 and Mobilenet combine ImageDataGenerator method when fitting. The average accuracy improve to 0.72.

*  Hyperparameters
   conv unit, pooling size, drop put rate, activation funtion, padding type, batch size, epochs
   
*  Data Augmentation

   rotation_range = 40
   
   width_shift_range = 0.2
   
   height_shift_range = 0.2
   
   shear_range = 0.2
   
   zoom_range = 0.2
   
   horizontal_flip = True
   
For more details about the model summary, please see the Output file. 


#  Future Improvements and Plans

*  Data Augmentation --- This project has very limit data on some categories. Thus try some other data augmentation method is most
   efficient way to improve train accuracy. Also combine other trnasfer learning model maybe will improve some accuracy.  
