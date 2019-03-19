# Python-source-code-generation-using-LSTM

What if our model generates code for us ?? Isn't that interesting ?

Yes ! We gonna build a LSTM model to generate python code for us !

# Steps in Generating Code :

1. Importing the 'txt' source code file into the environment
2. Reading each line in the file and converting them into lowercase
3. Tokenizing them into characters and finding the total number of characters and number of unique characters
4. Mapping the unique characters to integers, since we cant feed the characters to our model
5. Creating semi-redundant sequences and splitting them into X and Y(labels)
6. One-hot encoding the Y(labels)
7. Building a LSTM model with 2-LSTM layers and a fully-connected layer
8. Training and predicting to generate source code.

Prediction results after running 10 Epochs :

![alt-text](https://github.com/SaravananJaichandar/Python-source-code-generation-using-LSTM/blob/master/code_generator.png)

As you can see, our model predicted a "function" starting with "def", and with correct indendations. We can improvise this by building a bigger model with 4 LSTM layers containing 500 or 700 neurons in each layer, but this could be computationally expensive and time-consuming if trained on CPU.
