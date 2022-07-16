# AILabProj-FaceRecognition
Files for AI Lab Project about Face Recognition. The final purpose should be to make an application which uses Face Recogniton as a form of user authentication, using custom inputs (obtained with a proper Face Detection algorithm).

The best choice to solve this problem is to work with face embeddings, obtained with a sort of hash function which maps a human face to a fixed-dimension vector.
Using a metric, for example the Euclidean one, the problem reduces to identity-based clustering of the images. 
This approach adapts very well to work on new face images, that is our desired behavior.
So the idea of the solution is mainly inspired by the model of FaceNet, developed by Google researchers in 2015.

Firstly, the application detects face using a MTCNN (Multi-Task Convolutional Neural Network). The output of this model is used to calculate embeddings for each image.
Embeddings are given to an Inception net: we will use a model which is pretrained on the large-scale dataset VGGFace2, testing the accuracy on LFW dataset.
Last, we will analyse how the accuracy of the model reacts to changes of pose and illumination of images.
