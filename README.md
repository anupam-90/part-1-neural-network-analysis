## Part 1: Neural Network Analysis - Customer Churn
DATASET link:https://drive.google.com/drive/folders/1Aihn49cUYMjCgeCTFBTyprjrgZO3UY6r?usp=drive_link
## Project Overview
This repositary contains a basic feed-forward neural network trained on past customer data to predict customer churn.

## Task 6: Final Reflection
### Q1:
Wieght represetnthe importance or strength between each neuron, features like 'monthly_charges' influence the likelihood of churn. Biases shift the activation either to the left or right, making the model to fit data which may not pass through the origin. 
During the training phase, model uses backpropagation, on basis of it, the network updates these weights and biases respectively to minimize the loss function. 

### Q2:
Without activation functions, a neural network is nothing but a series of linear mathematical transformations, Activation functions like ReLu or Tanh inroduce non-linearity into the network.
It is crucial bevause it allows the network to learn and model complex real world patterns which would not be possible with a simple linear regrsssion. 

### Q3:
**Too High:** The weight updates in the model would be too drastic, it would possibly overshoot the optimal minimum of the loss the function, causing the training loss to jump erratically or even increase(diverge).
**Too Low:** In this case, the model will take very tiny steps, it would learn very slowly, requiring way more epochs to conclude to a solution.
It would also risk getting stuck on the 'optimal minimum' rather than finding the best overall solution. 

### Q4:
**Yes, the experiments demonstrated both the phenomena of overfitting and underfitting.**

Experiment 1 shows signs of overfitting, since when we increased the complexity of the model to 3 hidden layers and 64 neurons, the training accuracy jumped up to 1 or 100% which is a textbook
example of overfitting, which means the model memorized every single data point in the training set, testing accuracy stagnated around 0.98 or 98.25% which shows that the model failed to generalize new unseen data due to the highly specific rules. The testing accuracy score also proves that the model memorized every single data point. 
Conversely, the base model, experiment 2, and experiment 3 suffered from structural underfitting due to a class imbalance, instead of learning true predictive patterns,
these simpler models simply defaulted to predicting the majority class(retained customers) for everyone which inflated their accuracy to 98.2%

