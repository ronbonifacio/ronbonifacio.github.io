# Learning About Loss Functions
Probably the hardest concept for me to wrap my head around in this project was what the loss function is and what it is actually doing in neural nets. Accompanied with the fact that I'm currently studying COMP4702 Machine Learning as well as ELEC4630, it is rather important that I learn about this core concept. Now that I've finally dug into them, I actually understand what it is the loss function is doing.

In simple dot point terms, for classifiers:

-Predictions are values that take outputs from the neural net and with an activation function. For binary classifiers this is the sigmoid(), for multiclass this is the softmax().
-The loss function is a function that takes predictions from the neural net and scales them to create a value for the loss of a prediction.
  -Often times the loss function is created to minimise the scaling factor near when predictions are accurate (Loss=0 when Pred=1) and largely scale inccorect predictions such as the -log(y) loss function
-Loss is then used in the next batch in training to adjust weightings using gradient descent.
