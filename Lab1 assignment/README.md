# Lab 1: Neural Network Design Space Exploration

This lab uses PyTorch to build and train fully connected neural
networks on MNIST and compare implementation cost with accuracy drop.

## Files
- MNIST_Task1.ipynb: Network generator, training, evaluation and Pareto analysis.
- pareto_front.png: Cost versus accuracy drop plot.

## Requirements
Python 3, PyTorch (torch), torchvision and matplotlib.

## How to run
1. Download MNIST_Task1.ipynb.
2. Open Google Colab and upload the notebook.
3. Run all cells in order from top to bottom.
4. MNIST is downloaded automatically.
5. The notebook trains and evaluates the configurations and saves
   the plot as pareto_front.png.

## Experiment settings
- Hidden layers: 1, 2 or 3.
- Nodes per hidden layer: 10, 20, 40, 80, 160 or 200.
- Search method: Exhaustive search over 18 configurations.
- Training: 5 epochs, Adam optimizer, learning rate 0.001, batch size 128.
- Cost: Total parameters, including weights and biases.
- Accuracy drop (%): 100 - test accuracy (%).

Results may vary between runs because of random initialization
and shuffled training data.
