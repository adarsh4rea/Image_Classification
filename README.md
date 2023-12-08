MODEL ARCHITECTURE:
The model that was selected is a basic fully connected neural network that was built with the Keras library. Three dense layers make up the architecture:
Input layer with 512 neurons and ReLU activation.
Dropout layer with a dropout rate of 0.5 to prevent overfitting.
Hidden layer with 256 neurons and ReLU activation.
Another Dropout layer with a dropout rate of 0.5.
Output layer with the number of neurons equal to the number of unique classes (celebrities) and softmax activation for multiclass classification.

TRAINING PROCESS:
Sparse categorical cross-entropy loss and the Adam optimizer are used to train the model. HOG (Histogram of Oriented Gradients) features taken from pictures of famous people make up the training set. 
Fitting the model to the feature vectors (X) and their corresponding labels (y_encoded) is the process of training the model. With a batch size of 32, the training takes place over 25 epochs, and 20% of the data is used for validation.

CRITICAL FINDINGS:
The model's architecture is relatively simple, consisting of fully connected layers, which may limit its ability to capture complex patterns in images.
The use of HOG features for image representation may have limitations compared to more modern feature extraction techniques or convolutional neural networks (CNNs).
The model's effectiveness in predicting celebrities would depend on the quality and diversity of the training data, as well as the chosen features.
