# Task1---CV-AI
experimenting with custom datasets and training your model
For this experiment I built a image classification model using CNN in Tensorflow :
Classes made :
 - Cups (25 images)
 - Uno Flip Cards (26 images)
 - Hand gestures (26 images)

There were a total of 77 images, which i realize now is a very microscopic number to train your model with. The model was divided into training (62 images) and validation (15 images) set and the testing set was created later, not uploaded directly with the others. 

I also had to use softmax function (activation) as there were more than 2 classes.

In my first experiment with no dropouts and epoch=10, I recieved good response on some new images quite similar to the ones in dataset, but as soon as they started to differ, the model started predicting wrong answers. I realize this is probably due to overfitting and that my model simply memorized the images instead of understanding.

In the second experiment with dropouts and epoch = 20, the model is predicting wrong answers again but the accuracy percentage is nearly the same for all three classes so the model is basically guessing

In the third experiment with no dropouts and epoch=20, it becomes even more confidently wrong about the predictions

Training accuracy was 72% and Validation accuracy was 66%

<img width="1727" height="612" alt="image" src="https://github.com/user-attachments/assets/597926ea-0add-4080-adae-2c06f252eb20" />

Blue  (exp1, epochs=10, no dropout)
 training accuracy goes up steadily 
 validation accuracy (dashed) bounces around wildly 

Red   (exp2, epochs=20, WITH dropout)
 training accuracy slowly increases
 validation accuracy unstable, bouncing around
 dropout making training noisy

Green (exp3, epochs=20, NO dropout)
 training accuracy shoots to nearly 100%
 validation accuracy stays low ~60%
 HUGE gap = severe overfitting


Failed and Confusing experiments :
so I really didn't understand why increasing the epochs had no positive effect on the data or doing dropouts, maybe because the dataset was too small but that part confused me. Next thing i didn't understand how to fix the overfitting problem.

What i Learnt: 
from training this model i learnt a lot on what all stuff i would need to do differently to train a good model. 
Through this i also undestood 
- basic tensorflow framework
- loss functions
- backpropogation
- dropouts
- epochs
- different activation functions, softmax etc
- normalization
- batch size
- learning rate
- regularization


