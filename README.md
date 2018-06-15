# Transfer_Learning_VGG-16

This repo contains the program for Transfer learning the VGG-16 model.

We use the state of art architecture VGG-16 to increase the image classification accuracy. 
To know more about VGG-16 architecture please refer this urls:
    
    1.https://arxiv.org/abs/1409.1556
    2.https://medium.com/@siddharthdas_32104/cnns-architectures-lenet-alexnet-vgg-googlenet-resnet-and-more-666091488df5
    3.https://www.pyimagesearch.com/2017/03/20/imagenet-vggnet-resnet-inception-xception-keras/

To know about Transfer learning please refer this urls:

    1.http://cs231n.github.io/transfer-learning/
    2.https://machinelearningmastery.com/transfer-learning-for-deep-learning/
    3.https://www.analyticsvidhya.com/blog/2017/06/transfer-learning-the-art-of-fine-tuning-a-pre-trained-model/
    4.http://ruder.io/transfer-learning/
    5.https://www.pyimagesearch.com/2017/03/20/imagenet-vggnet-resnet-inception-xception-keras/
    6.https://medium.com/@siddharthdas_32104/cnns-architectures-lenet-alexnet-vgg-googlenet-resnet-and-more-666091488df5


This is the program written for classifcation of elephant and non-elephant images (Basically binary classification).If you want to perform multiclass classification simply use categorical_crossentropy or some other loss functions.
  
1. Training our model:
    
        Use the train.py for training our model.
   
2. Classify the test images:
    
        Use the class.py for testing our model.
       


Notes: 
----------
   * This is made in reference with,
            https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html
            https://www.codesofinterest.com/2017/08/bottleneck-features-multi-class-classification-keras.html
            
   * For the first time running train.py,it will search for Pre-trained weight file of the VGG-16 (without top layer), if it doesn't find it, it will automatically download from internet.
   
   * Pre-trained file is mandatory to perform any kinf of transfer learning.
   * To classify the Images, we must do trainning followed by classification.
   * My dataset folder (named "data") will look like this.
        
                  data/
                      train/
                          elephant/
                              ele001.jpg
                              ele002.jpg
                              ...
                          others/
                              other001.jpg
                              other002.jpg
                              ...
                      validation/
                          elephant/
                              ele801.jpg
                              ele802.jpg
                              ...
                          others/
                              other801.jpg
                              other802.jpg
                              ...
        
