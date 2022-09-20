# Basic_Perceptron
This repo explores the basics of Perceptron from scratch. Enjoy!

### Software, Tools, and prerequisits
1. Access to Google Colab or some Jupyter Notebook.
2. Basic python programing.
3. Basic arithmetic & calculus knowledge

### Intro: What is a Perceptron?
A superviced learning algorithm for binary classifiers. Also reffered to as the single unit of a neural network with a step activation function. This can learn only linearly seperable patterns.

The single layer perceptron is imspired by biological neuron and simulates it.

<img
  src="neuron.png"
  alt="Alt text"
  title="Optional title"
  style="display: block; align: center; margin: 0 auto; max-width: 150px">

Given the following equations,
1. A linear model:

$$ f(x) = w^{T}x + b $$

2. The unit step function (serving as activation function):

$$ U(z)=   \left\{
\begin{array}{ll}
      1 & if z \geq \theta \\
      0 & otherwise \\
\end{array} 
\right.  $$

3. The resulting approximation of the output combining the above equations.

$$ \hat{y} = U(f(x)) = U(w^{T}x + b) $$

4. The Perceptron update rule, where $\alpha$ is the learning rate. Note the calculation below is done as vectors for optimization:

$$ w = w + (\alpha * \Sigma ({y}- \hat{y})) * x $$
$$ b = b + (\alpha * \Sigma ({y}- \hat{y})) $$

### Steps to completing the project
1. Import the necessary modules/ packages needed for this project.
2. Generate your dataset and split them into train & test sets.
3. Plot your dataset for visualization.
4. Implement the perceptron algorithm using np arrays $fit(X,y)$ & $predict(X)$:
    * Initialize your weight vector as random vectors.
    * initialize your bias.
5. Test your classifier & evaluate the error using any accuracy calculation method.
