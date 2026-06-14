# Task1---CV-AI
experimenting with custom datasets and training your model
For this experiment I built a image classification model using CNN in Tensorflow :
Classes made :
 - Cups (25 images)
 - Uno Flip Cards (26 images)
 - Hand gestures (26 images)

There were a total of 77 images, which i realize now is a very microscopic number to train your model with. The model was divided into training (62 images) and validation (15 images) set and the testing set was created later, not uploaded directly with the others. 
In my first experiment with no dropouts and epoch=10, I recieved good response on some new images quite similar to the ones in dataset, but as soon as they started to differ, the model started predicting wrong answers. I realize this is probably due to overfitting and that my model simply memorized the images instead of understanding.
In the second experiment with dropouts and epoch = 20, the model is predicting wrong answers again but the accuracy percentage is nearly the same for all three classes so the model is basically guessing
In the third experiment

