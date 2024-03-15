**Introduction/Context:**
- The YT video for this material : https://www.youtube.com/watch?v=VMj-3S1tku0&t=6249s

- The video is called "The spelled-out intro to neural networks (NN) and backpropagation: building micrograd".

- And he builds something called a micrograd - what does it mean?

- Micrograd is a small automatic-gradient, or autograd engine. It implements backpropagation.

- What is backpropagation? It is an algorithm used for training neural networks. More on this later.

- BPN, or backpropagation, helps to evaluate gradients (differentitation) of a mathematical function

- In a neural network, BPN is used to calculate the gradients of loss function (of the NN).

- BPN is at the core of modern deep neural network libraries like PyTorch, JAX, etc.

- He then goes on to explain the usage of micrograd engine -we shall come to that at the last - when we have already understood the whole video.

**Derivative of a simple function with one input:**
- This section includes code - find it in the jupyter notebook (in a section with the same name)

- A function `f(x) = 3x^2 - 4x + 5` is used for demo. It is evaluated for a data point (3.0) and also plotted.

- From the plot of the function, we start thinking about derivative of the function - at different points (on the x-axis) of the graph.

- From the definition of differentiability, the value of a limit if it exists, is given by the equation:`(f(a+h) - f(a)) / h`, where `h` is the slight bump  made to the value of `a` (input variable). 

- This limit value is the amount by which the functon responds, i.e., the slope at that point.

- How much does the function go up or down? What is the sensitivity of the function the change `h` made to input `a`?
- This, in fact, can help to calculate the derivative of the function. Taking `h = 0.0000001` for `a = 3.0`, we get `f(x + h) - f(x) = 0.00140003000` and `(f(x + h) - f(x))/h = 14.00030000`.

- From the graph we can see, at `x = 3.0`, the value of `f(x)` is approx. `14` and a slight nudge to the positive x-axis shifts the function `f(x)` higher! This positive slope is the value of the derivative.

- Two more examples are provided. With a negative `h`, we see the function `f(x)` also falls down - negative slope, hence negative derivative!

- At `x = 2/3`, function `f(x)` becomes zero. And very small nudges don't cause any change to the function `f(x)`, and thereby the derivative.
