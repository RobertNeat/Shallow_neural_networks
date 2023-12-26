# Neural Network Creation and Parameter Optimization

---

## Neural Network Basics and Activation Functions

Activation functions are essential in neural networks for introducing non-linearity. Here are some commonly used ones:

- **Sigmoid**: Outputs values between 0 and 1.
- **Tanh (Hyperbolic Tangent)**: Similar to Sigmoid but ranges from -1 to 1.
- **Softsign**: A smooth variation of the sigmoid function.
- **ReLU (Rectified Linear Unit)**: Allows for faster training of deep neural architectures.
- **ELU (Exponential Linear Unit)**: Addresses vanishing gradient problems.
- **SELU (Scaled Exponential Linear Unit)**: Scaled version of ELU for better learning dynamics.
- **Softmax**: Used in multi-class classification to obtain probabilities.

## Grid Search for Hyperparameter Tuning

Grid search is a technique for systematically working through multiple combinations of hyperparameters to find the best configuration for a model. In cases where exhaustive search is impractical, randomized search offers a quicker alternative by randomly selecting combinations.

---

### Code Explanation

The provided code demonstrates the creation of dense neural networks using Keras for the MNIST dataset. It involves:

1. Defining activation functions and visualizing their behaviors.
2. Implementing a wrapper for Keras models to use with `GridSearchCV`.
3. Performing grid search for hyperparameters (`n_hidden`, `n_neurons`, `neural_optimizer`, `learning_rate`, `epochs`, `batch_size`).
4. Training a model based on the best parameters obtained from grid search and evaluating its performance on test data.
5. Plotting accuracy and loss over epochs to visualize model performance and potential overfitting.

### Steps to Use the Code

1. **Activation Functions Visualization**: Displaying the behavior of various activation functions.
2. **Grid Search**: Search for the best combination of hyperparameters.
3. **Training Model**: Training the model using the obtained best parameters.
4. **Model Evaluation**: Evaluate model performance on test data.
5. **Plotting Performance**: Visualize training and validation accuracy/loss.

### Overfitting Detection

Overfitting occurs when a model learns the training data too well but performs poorly on unseen data. Loss and accuracy plots over epochs can help identify overfitting. If the validation loss increases while the training loss decreases, it's a sign of overfitting.

### Randomized Search as an Alternative

For more complex scenarios, where grid search becomes time-consuming due to numerous parameters, randomized search offers an efficient way to explore a broader range of hyperparameter combinations randomly.

---

The code provides a structured approach to creating neural networks, optimizing hyperparameters, and evaluating model performance. Use it as a guide for implementing similar procedures in your projects.

## Launching Project

To run the project, you have a couple of options:

### Using Google Colab via Gist

Access the project through Google Colab using the Gist website. You can import the necessary data from the GitHub project resources. Use the following Gist link: [gist link here](https://gist.github.com/RobertNeat/5cabf823cb93a378fd36ccf2ffefde0f)

### Running Locally

If you prefer to run the project on your local machine, follow these steps:

1. **Clone the Repository**: Download the repository branch from GitHub.
2. **Local Environment**:
   - **DataSpell or PyCharm**: Open the project using DataSpell or PyCharm by JetBrains.
   - **Spyder IDE**: Alternatively, you can use Spyder IDE to work with the project.
3. **Dataset Requirements**:
   - Ensure that the dataset files are available and stored inside your project directory. This step is crucial to prevent any issues related to missing data.

Running the project locally allows you to explore the code and execute it in your preferred Python environment. If you encounter any problems, make sure to check the dataset's presence in your project directory.
