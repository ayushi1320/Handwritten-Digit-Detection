# Handwritten-Digit-Detection
IMPORT DATASET :
 Tensorflowand Kerasallow us to import and download the MNIST dataset(Modified National Institute of Standards and Technology) directly from their API
 The MNIST database contains 60,000 training images 
 10,000 testing images 
PREPROCESS DATA:
 Reshaping the array to 4-dims so that it can work with the KerasAPI(greyscale image ) 
 Need to normalize our data as it is always required in neural network models, by dividing the RGB codes to 255
 So initially will be converting data to float as we are dividing
BUILDING THE CONVOLUTIONAL NEURAL NETWORK:
 Sequential model allows you to build a model layer by layer.
 model.add(Conv2D(28, kernel_size=(3,3), input_shape=input_shape))
 #28 number of layers
Max pooling is a pooling operation that selects the maximum element from the region of the feature map covered by the filter. Flattening involves transforming the entire pooled feature map matrix into a single column which is then fed to the neural network for processing.DENSE LAYER , A linear operation in which every input is connected to every output by a weight . It connects neurons in one layer to neurons in another layer. It is used to classify images between different category by training.DROPOUT : A Simple Way to Prevent Neural Networks from OverfittingSOFTMAX  LAYER is the last layer of CNN. It resides at the end of FC layer, softmaxis for multi-classification.Flattening involves transforming the entire pooled feature map matrix into a single column which is then fed to the neural network for processing.DENSE LAYER , A linear operation in which every input is connected to every output by a weight . It connects neurons in one layer to neurons in another layer. It is used to classify images between different category by training.DROPOUT : A Simple Way to Prevent Neural Networks from OverfittingSOFTMAX  LAYER is the last layer of CNN. It resides at the end of FC layer, softmaxis for multi-classification.Thus, the output after max-pooling layer would be a feature map containing the most prominent features of the previous feature map
Flattening involves transforming the entire pooled feature map matrix into a single column which is then fed to the neural network for processing.
DENSE LAYER , A linear operation in which every input is connected to every output by a weight . It connects neurons in one layer to neurons in another layer. It is used to classify images between different category by training.
DROPOUT : A Simple Way to Prevent Neural Networks from Overfitting
SOFTMAX  LAYER is the last layer of CNN. It resides at the end of FC layer, softmaxis for multi-classification.
COMPILING AND TRAINING THE MODEL : Compiling the model takes three parameters: optimizer, loss and metrics.
optimizer : controls the learning rate. We will be using ‘adam’ as our optmizer. Adam is generally a good optimizer to use for many cases. The adam optimizer adjusts the learning rate throughout training
Loss: that can be used to estimate the loss of the model so that the weights can be updated to reduce the loss on the next evaluation.We use fit method then training starts 
EVALUATING THE MODEL :With a simple evaluate function to know the accuracy.
