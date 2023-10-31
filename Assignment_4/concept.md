Kernal:

“Kernel” is used due to a set of mathematical functions used in Support Vector Machine providing the window to manipulate the data. So, Kernel Function generally transforms the training set of data so that a non-linear decision surface is able to transform to a linear equation in a higher number of dimension spaces.

Different Types of kernal functions:


            1. Polynomial Kernal
            
            2. RBF Kernal
            
            3. Sigmoid Kernal

Polynomial Kernal:


It represents the similarity of vectors in the training set of data in a feature space over polynomials of the original variables used in the kernel.
![image](https://github.com/Astik-Gorai/ML-Lab/assets/81304561/aebe0e39-c6b2-454d-a6e7-fb2b1e2df864)


Sigmoid Kernal:
this function is equivalent to a two-layer, perceptron model of the neural network, which is used as an activation function for artificial neurons.
![image](https://github.com/Astik-Gorai/ML-Lab/assets/81304561/92fdc534-7b68-468d-bc0f-b3f4601ed9ff)

RBF Kernal:
Improvement of Gaussian Kernal.
![image](https://github.com/Astik-Gorai/ML-Lab/assets/81304561/beaf4686-77e8-4e4a-8783-047a0446a242)

'C' Parameter in SVM :
The C parameter tells the SVM optimization how much you want to avoid misclassifying each training example. For large values of C, the optimization will choose a smaller-margin hyperplane if that hyperplane does a better job of getting all the training points classified correctly.
It controls the level of misclassification that can be tolerated in the training dataset.

Gamma Parameter in SVM:
The gamma parameter in SVMs is a hyperparameter that controls the shape of the decision boundary. It determines the flexibility of the model and the level of overfitting or underfitting of the training data.

Difference between C parameter and Gamma Parameter:
The C parameter controls the trade-off between margin maximization and classification error, with high C values leading to potential overfitting, and low C values emphasizing better generalization. On the other hand, the gamma parameter shapes the complexity and flexibility of the decision boundary when a non-linear kernel is used, with high gamma values leading to potential overfitting and low gamma values potentially causing underfitting. Both parameters should be carefully tuned to find the right balance for a given problem and dataset.


