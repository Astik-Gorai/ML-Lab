# Gradient Descent:

A gradient is nothing but a derivative that defines the effects on outputs of the function with a little bit of variation in inputs.

Gradient Descent (GD) is a widely used optimization algorithm in deep learning that is used to minimize the cost function of a neural network model during training. It works by iteratively adjusting the weights or parameters of the model in the direction of the negative gradient of the cost function until the minimum of the cost function is reached.

## Vanishing and Exploding gradients:

Vanishing and exploding gradients are common problems that can occur during the training of deep neural networks. These problems can significantly slow down the training process or even prevent the network from learning altogether.

 The vanishing gradient problem occurs when gradients become too small during backpropagation. The weights of the network are not considerably changed as a result, and the network is unable to discover the underlying patterns in the data. Many-layered deep neural networks are especially prone to this issue. The gradient values fall exponentially as they move backward through the layers, making it challenging to efficiently update the weights in the earlier layers.

The exploding gradient problem, on the other hand, occurs when gradients become too large during backpropagation. When this happens, the weights are updated by a large amount, which can cause the network to diverge or oscillate, making it difficult to converge to a good solution.

To address these problems the following technique can be used:

        1. Weights Regularzations: The initialization of weights can be adjusted to ensure that they are in an appropriate range. Using a different activation   
                                function, such as the Rectified Linear Unit (ReLU), can also help to mitigate the vanishing gradient problem.
                                
        2. Gradient clipping: It involves limiting the maximum and minimum values of the gradient during backpropagation. This can prevent the gradients from     
                           becoming too large or too small and can help to stabilize the training process.
                           
        3.  Batch normalization: It can also help to address these problems by normalizing the input to each layer, which can prevent the activation function   from saturating and help to reduce the vanishing and exploding gradient problems.

Types Of Gradient Descent:

          1. Batch Gradient Descent:  In batch gradient descent, To update the model parameter values like weight and bias, the entire training dataset is used to compute the gradient and update the parameters at each iteration. This can be slow for large datasets but may lead to a more accurate model. It is effective for convex or relatively smooth error manifolds because it moves directly toward an optimal solution by taking a large step in the direction of the negative gradient of the cost function. However, it can be slow for large datasets because it computes the gradient and updates the parameters using the entire training dataset at each iteration. This can result in longer training times and higher computational costs.
          2. Stocastic Gradient Descent:In SGD, only one training example is used to compute the gradient and update the parameters at each iteration. This can be faster than batch gradient descent but may lead to more noise in the updates.
          3. Mini-Batch Gradient Descent: In Mini-batch gradient descent a small batch of training examples is used to compute the gradient and update the parameters at each iteration. This can be a good compromise between batch gradient descent and Stochastic Gradient Descent, as it can be faster than batch gradient descent and less noisy than Stochastic Gradient Descent


 Internal Covariate Shift: Internal Covariate Shift refers to a phenomenon in deep neural networks where the distribution of the activations within each layer of the network changes during training. This change in distribution can have a detrimental effect on training convergence and network performance.
 Fixed distribution of inputs to a sub-network would have positive consequences for the layers outside the subnetwork, as well.
 
