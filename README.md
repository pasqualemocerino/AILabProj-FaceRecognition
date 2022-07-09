# AILabProj-FaceRecognition
Files for AI Lab Project about Face Recognition. The final purpose is to make an application which uses Face Recogniton as a form of user authentication, using custom inputs obtained with a proper Face Detection algorithm.

The best choice to solve this problem is to work with face embeddings, obtained with a sort of hash function which maps a human face to a fixed-dimension vector.
Using a metric, for example the Euclidean one, the problem reduces to identity-based clustering of the images, that could be done using different approaches.
So the idea of the solution is inspired by the model of FaceNet, developed by Google researchers in 2015.
