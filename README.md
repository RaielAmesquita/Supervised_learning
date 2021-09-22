# Supervised_learning
 Understand the fundamentals of neural networks and how they are trained to make accurate predictions. 

The Problem - The neural network will be given a sequence of three numbers that can only be a zero or a one. In the table we have the patterns
with their correct outputs listed for each pattern. The answer to the pattern is that the first digit in the pattern is always the output. 
Now that we can see the pattern. The challenge is to design a neural network that can learn this for itself. (The image file provided the situation)

Execution - Since there are 3 input connections with a single output connection, this problem will only require a single neuron. Now lets's discuss 
how to apply the weights to the inputs.

Weights - The neural network will use memory that will allow it to learn. We have three weights in the problem, one for each input.
Each connection will have its own weight which will be a number between -1 and 1. If the number is close to 1 it will increase the strength of the signal 
and if the number is closer to 0 it will decrease the strength of the signal. If the weight is negative it will completely inhibit the neuron from firing. 

Theory - Based on how the weights are designed the derived equation takes the input value and multiplies it by the weight and then adds them all together
to produce the output. Incoming signal to the neuron=input1*weight1+input2*weight2+input3*weight3 

Activation function - I will also use an activation function that will take the incoming signal and translate it to the output. We will be using the sigmoid
function. Euler’s number is e=2.71828. I will use this is in the sigmoid function. One reason sigmoid is used in neural networks is because neural networks
are used to estimate probabilities. Probabilities range between zero and one so the sigmoid function takes the input signal and puts it in-between zero and
one so the output can be seen as a probability.

Training process- This neural network is trained by adjusting the weights to minimize the error between the predicted values made by the known network 
and the target practice provided by the training set. First I assigned random weights between minus one and plus one. Then the neural network will predict 
the output using the activation function. Then it will take the output that was given and compare it to the correct answer. In doing this, it will reveal 
the error within the neural network and it will adjust the weights and start to learn. It will repeat this step 10,000 times. By the end, the neural network 
will be able to guess the correct output by adjusting the weights. With this we can input a new similar pattern and the neural network will be more accurate 
at predicting the output.

How to adjust the weights- Use the error cost function and gradient descent.

Error cost function gradient= input*error in output*sigmoid curve gradient

Sigmoid gradient= neuron output*(1-neuronoutput) 


Results-  The neural network was given a new pattern of 1,0,0. As we know the correct answer is 1. After 10,000 executions, the neural network gave an output 
of 0.9999.  This output  was an extremely accurate result given by the neural network. 
