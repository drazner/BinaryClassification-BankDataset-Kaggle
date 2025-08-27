I have included the Jupyter Notebook that I used to construct a binary classification artifical neural network using tensorflow. 

First I cleaned the incoming data and then evaluated scatterplots, histograms and heatmaps to determine general relationships. 

Then I separated the input features into two separate lists: one for categorical data and one for numerical data. 

I applied a standard scaler to the numerical data and OneHotEncoding for the categorical data.

I created an ANN model with an input layer that uses batch normalization, three hidden layers using the ReLU activation function and an output layer using the sigmoid function.
I used adam for the optimizer, and binary-crossentropy for the loss function, and I added an early-stopping callback because without it the model was overfitting.

After training, I was able to create a model with 93.20% binary-accuracy 

<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/c8d21894-d7c0-4356-afe9-398906322a75" />

![Uploading image.png…]()
