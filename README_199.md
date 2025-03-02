Deep Learning Assignment 1 - CIFAR-10 Classification

Overview:
This project implements a Feedforward Neural Network (FNN) to classify images from the CIFAR-10 dataset. The model is trained using different optimizers and hyperparameters, following the requirements of Deep Learning Assignment 1.

Dataset Details:
- Dataset Used: CIFAR-10
- Number of Classes: 10 (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
- Training Set: 50,000 images
- Test Set: 10,000 images
- Image Size: 32 × 32 pixels

Model Implementation:
- Model Type: Feedforward Neural Network (FNN)
- Hidden Layers: Configurable (3, 4, 5 layers)
- Activation Functions: ReLU, Sigmoid
- Optimizers Tested: SGD, Adam, RMSprop, Momentum-based SGD, Nesterov Accelerated Gradient Descent
- Loss Functions: Cross-Entropy Loss and Mean Squared Error (MSE)
- Batch Sizes Tested: 16, 32, 64
- Learning Rates: 0.001, 0.0005
- Weight Initialization: Random, Xavier

Training and Evaluation:
- The model is trained for multiple epochs using different configurations.
- Training and validation losses were observed for model performance.
- Cross-Entropy Loss and Mean Squared Error Loss were compared.
- A confusion matrix was generated to visualize classification performance.

Results and Best Model Selection:
The model was trained with different hyperparameter settings, and the accuracy results are as follows:

- For hidden layers [64, 128, 256] with a learning rate of 0.001 and batch size of 32 using Adam optimizer, the test accuracy was 52.17%.
- For hidden layers [128, 256, 512] with a learning rate of 0.0005 and batch size of 64 using SGD optimizer, the test accuracy was 33.68%.
- For hidden layers [32, 64, 128] with a learning rate of 0.001 and batch size of 16 using RMSprop optimizer, the test accuracy was 46.34%.

Based on these results, the best configuration chosen for CIFAR-10 classification was:
- Hidden Layers: [64, 128, 256]
- Optimizer: Adam
- Batch Size: 32
- Learning Rate: 0.001

Loss Function Comparison:
The comparison between Cross-Entropy Loss and Mean Squared Error (MSE) Loss showed the following:
- Cross-Entropy Loss: 1.4042
- Mean Squared Error (MSE) Loss: 9.7332

It was observed that Cross-Entropy Loss performed significantly better than MSE Loss, confirming that it is more suitable for multi-class classification tasks.

How to Run the Code:
1. Clone the repository:
   ```
   git clone <your-github-repo-link>
   cd <repo-folder>
   ```
2. Open the `199dlassignment.ipynb` file in Google Colab or Jupyter Notebook.
3. Run all the cells in order.
4. Check the model accuracy, loss values, and confusion matrix at the end.

Submission Details:
- GitHub Repository: `<your-github-repo-link>`
- Google Form Submission Link: [Submit Here](https://forms.gle/Xdn6qYDDQpGg77Aw5)
