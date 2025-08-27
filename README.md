# General Summary
I have included the Jupyter Notebook that I used to construct a binary classification artifical neural network using tensorflow. 

## Data Cleaning
First I cleaned the incoming data and then evaluated scatterplots, histograms and heatmaps to determine general relationships. 
Here are some samlpes from that process: 
<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/7cec0f15-7cf0-448b-adc8-d751bf3ae2dc" />

<img width="1376" height="1489" alt="image" src="https://github.com/user-attachments/assets/afec5d6d-153b-4a75-bfa6-e0520ce45efe" />
Note: the data was already fairly clean given that it was given from a Kaggle playground competition (i.e. there were no nulls or duplicates found)

## Pre Processing
Then I separated the input features into two separate lists: one for categorical data and one for numerical data. 

I applied a **standard scaler** to the numerical data and **OneHotEncoding** for the categorical data.

## ANN Model
I created an ANN model with: 
1) an input layer that uses **batch normalization**,
2) three hidden layers using the **ReLU activation function** and
3) an output layer using the **sigmoid function**

   
I used **adam** for the **optimizer**, and **binary-crossentropy** for the **loss function**, and I added an **early-stopping callback** because without it the model was **overfitting**.


<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/db1d03d5-d91d-4b2e-86e6-d7b8879d9ee0" />


## Results
After training, I was able to create a model with **93.20% binary-accuracy** on training data and **92.97% validation-binary-accuracy** with early stopping during the 9th Epoch. 

<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/c8d21894-d7c0-4356-afe9-398906322a75" />

<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/0654b7b5-bfc6-4df6-b8b4-c4a356343e46" />

