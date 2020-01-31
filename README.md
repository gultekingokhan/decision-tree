# Decision Tree
Example code and own notes while taking the course "Intro to Machine Learning" on Udacity.

## Entropy
Controls how a decision tree where to split the data.

**Definition:** Measure of impurity in a bunch of examples.

![Entropy](resources/entropy-formula.png)

> Pi: Fraction of examples in class

### Tips

⭐️ All examples are same class 👉 Entropy = 0

⭐️ Examples are evenly split between classes 👉Entropy = 1.0

## Information Gain

```Information gain = entropy(parent) - [weighted average] * entropy(children)```

> The question is: Where to make that split?

Decision tree algorithm : **MAXIMIZE INFORMATION GAIN**

This is how we will choose the feature that split on.

## Bias - Variance Trade-Off

High bias is not so good. There should be a sweet balance between bias and variance.

High bias practically ignores the data. Almost no capacity to learn anything.

## Pros & Cons of Decision Tree

### Pros
- You can build bigger classifiers out of decision trees in something called ensemble methods.

### Cons
- Prone to overfitting. 
If you have data that lots and lots of features and a complicated decision tree it can overfit tha data. Have to be careful with the parameter tunes that you're picking.

