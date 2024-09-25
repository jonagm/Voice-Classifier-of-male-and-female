# Voice Classifier of male and female (Trees and KNN)
This is a Voice classifier in WAV files that can identify whether the voice in the audio file belongs to a man or a woman (MATLAB)

The small model was trained using _19 voice files, where 10 belong to a male and 9 to a female_. The **Fourier Transform** is employed to decompose a signal and extract information about its composition, specifically from all our audio files to gather relevant details.

The signal is _normalized_ to ensure that there are no peaks. 
Among the features (feature vector) selected for training, three were chosen:

1. **Mean Absolute Value**: This is an average of the characteristics.
2. **Variance**: This represents the variability of the dataset concerning its mean.
3. **Maximum Peak**: It is important to identify the maximum values of our variables.
Based on this feature vector, similarities or differences within our database are _identified_.

With all this in place, training begins using the **"Classification Learner"** for supervised training. The feature vector is loaded, and we define the target prediction, which in this case is “male” or “female.” We select the **"All Quick-To-Train"** option, which chooses a variety of classifiers (_decision trees and K-Nearest Neighbors_) that can be trained quickly.

Finally, upon exporting the model, it provides us with a **function** that will assist in making classifications for the test.

## **Original dataset:**
![1](https://github.com/user-attachments/assets/1d30e010-86f4-40b3-ac07-3d0399d5905f)

## **Training variety:**
### Trees:
![training-trees](https://github.com/user-attachments/assets/7e25dbda-9d4f-4145-b10a-3b0ac5f2cfca)
### KNN:
![training-KNN](https://github.com/user-attachments/assets/436ce3b0-7e03-4f05-a5eb-db30d73813f6)

## **Function:**
![final-function](https://github.com/user-attachments/assets/2be4738b-f547-4f01-8452-12563ed0e9cd)

## **Test:**
![test](https://github.com/user-attachments/assets/7369b930-91f9-46d2-9cc3-43e56fa71564)





