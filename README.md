# Two-Input Perceptrons Learning Project

This repository contains Python code for learning two-input perceptrons, specifically implementing the AND gate and OR gate.

## Introduction

This project provides a hands-on learning experience with perceptrons, a fundamental building block of artificial neural networks. Perceptrons are simple models capable of learning binary classification tasks, and understanding their functionality is crucial for grasping the basics of neural network operations.

The implemented perceptrons in this project learn to mimic the behavior of logical AND gate and logical OR gate, which are essential components in digital logic circuits and serve as foundational examples in neural network tutorials.

## Implementation Details

The project includes Python scripts to create, train, and test two-input perceptrons for the AND gate and OR gate logic operations. The code is structured to facilitate understanding and experimentation, making it suitable for educational purposes and beginner-level understanding of neural networks.

## How to Use

### Running Locally

1. **Clone the Repository:**
   - Clone this repository to your local machine using the following command:

        ```bash
        git clone <repository_url>
        ```

2. **Navigate to the Project Directory:**
   - Enter the cloned repository directory:

        ```bash
        cd <repository_directory>
        ```

3. **Install Dependencies:**
   - Ensure you have Python 3.x installed on your system.
   - Install the required dependencies using pip:

        ```bash
        pip install -r requirements.txt
        ```

4. **Run the Perceptron Learning Scripts:**
   - Execute the Python scripts for learning AND gate and OR gate perceptrons:

        ```bash
        python and_gate_perceptron.py
        python or_gate_perceptron.py
        ```

   - These scripts will train the perceptrons and display the learned weights and biases.

5. **Test the Perceptrons:**
   - You can test the trained perceptrons with different input combinations to observe their behavior.

### Running on AWS EC2 Instance

If you prefer running the code on an AWS EC2 instance, you can follow similar steps outlined in the [Running on AWS EC2 Instance](#running-on-aws-ec2-instance) section of the README file.

## Example Usage

Below is an example of how you can use the perceptrons in your Python code:

```python
from perceptrons import Perceptron
from inputs import AND_inputs, OR_inputs

# Create an AND gate perceptron
and_perceptron = Perceptron()
and_perceptron.train(AND_inputs)

# Test the AND gate perceptron
input_data = (1, 0)
output = and_perceptron.predict(input_data)
print(f"AND gate output for {input_data}: {output}")

# Create an OR gate perceptron
or_perceptron = Perceptron()
or_perceptron.train(OR_inputs)

# Test the OR gate perceptron
input_data = (1, 0)
output = or_perceptron.predict(input_data)
print(f"OR gate output for {input_data}: {output}")
