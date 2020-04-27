# Create-ChatBot

        
Here are the 5 steps to create a chatbot in Python from scratch:
                           
**1.Import and load the data file:**
 
Data.json file contains patterns and responses for our chatbot 

**2.Process data **

3.Create Training and testing data 

**4.Build the model **

In order to create a deep neural network model with three layers i.e Input layer with 128 neurons, Hidden layer with 64 neurons and Output layer. Keras Sequential API is being used where a sequential model is a linear stack of layers. A parameter called input.shape is passed in the first layer which denotes the tuple shape. The following layers can automatically perform shape inference. In this project, the input.shape will be equal to the length of our training data. The next parameter is the Activation Function which is used to determine the output of a neural network like yes or no.

The project uses ‘ReLU(rectified linear unit)’ activation function represented as :
 					R(z)=max(0,z) 
The project uses ‘Softmax’ activation function for the final layer that maps the final output as [0,1] range and sums up to 1.

Large neural nets trained on relatively small datasets can overfit the training data. Therefore, probabilistically dropping out nodes in the network is a simple and effective regularization method.
Compilation - Before training a model, you need to configure the learning process, which is done via the compile method. 
Stochastic Gradient Descent (SGD): it uses only a single sample, i.e., a batch size of one, to perform each iteration. The sample is randomly shuffled and selected for performing the iteration.

**5.Predict the response **

Loading the trained model and then use a graphical user interface that will predict the response from the bot. The model will only tell us the class it belongs to, so we will implement some functions which will identify the class and then retrieve us a random response from the list of responses.



