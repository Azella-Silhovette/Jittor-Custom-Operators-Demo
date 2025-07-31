# Jittor-Custom-Operators-Demo
Custom operator implementations (Linear, ReLU, Sigmoid, Softmax, MSE/CrossEntropy Loss) using Jittor framework. Includes MLP regression for function fitting and classification on MNIST with training visualizations.

## 1. Environment Requirements

* **Operating System:** Windows
* **Python Version:** 3.7.5
* **Hardware:** CPU (for local testing, run inside a VS Code container with CPU only; no GPU)
* **Memory:** At least 8 GB

## 2. Installation Steps

1. **Create and Activate a Virtual Environment (Recommended)**

   ```bash
   # Using conda
   conda create -n jittor_env python=3.7.5 -y
   conda activate jittor_env

   # Or using venv
   python -m venv jittor_env
   source jittor_env/bin/activate   # On Windows: jittor_env\Scripts\activate
   ```

2. **Install Jittor**

   * **CPU-only version:**

     ```bash
     pip install jittor==1.2.2.59
     ```

3. **Install Other Dependencies**

   ```bash
   pip install numpy matplotlib
   ```

## 3. Data Preparation

* The MNIST dataset will be downloaded automatically via `jittor.dataset.mnist.MNIST`; no manual download is required.
* For the regression task, synthetic data is generated within the script—no additional data files are needed.

## 4. Common Issues

1. **Error: `ModuleNotFoundError: No module named 'jittor'`**

   * Ensure you have installed Jittor in and activated your virtual environment; then retry:

     ```bash
     pip install jittor==1.2.2.59
     ```
2. **Plot Window Does Not Appear**

   * Verify that `matplotlib` is installed, run from a terminal environment, or enable plotting support in your IDE.
