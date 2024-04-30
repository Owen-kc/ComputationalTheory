# Computational Theory

In this project, we solve the [numbers round](https://en.wikipedia.org/wiki/Countdown_(game_show)#Numbers_Round) of the popular TV show, [Countdown](https://en.wikipedia.org/wiki/Countdown_(game_show)), through the use of Python in this Jupyter notebook.

By *Owen Casey*

# Topic & Context

In the numbers round of countdown, contestants choose six numbers from a predefined set (two sets of integers 1-10, one set of 25, 50, 75, 100), and use these given numbers to add, subtract, divide and multiply to achieve a result based on a randomly generated three digit number between 101-999. Each number can onlt be used once, and the operations must result in whole numbers, meaning there can't be any fractions, decimals or negative numbers at any point in the calculation process. The contestants are timed, and must complete their answer within 30 seconds.

![Countdown Numbers Game](https://coolbutuseless.github.io/img/8-out-of-10-cats/left.jpg)


# Prerequisites
The main content of this repository is contained in a Jupyter notebook. To run the notebook, you will need the following:

**Python**: Downloading the most recent version of Python is recommended. You can download python from the official Python site [here](https://www.python.org/downloads/). However, I recommend installing Python through [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/) or [Anaconda](https://www.anaconda.com/download), as it provides an all in one installation and management for Python. 
- Miniconda (Recommended): Minimal installer, low storage usage
- Anaconda: Full installer, high storage usage 

**Jupyter Notebook**: Jupyter Notebook support should come with Anaconda/Miniconda, but you can also install it through a VSCode extension.

**Required Libraries**: Any required libraries will be mentioned in the relevant section they are used in the notebooks. 

**VSCode**: If you intend to execute code in your own environment, VSCode is recommended, as it's the standard.

# Anaconda and Miniconda
The use of Anaconda or Miniconda is *heavily* encouraged for this repository. Anaconda is a **full** installer while Miniconda is a **minimal** installer. They both have an easy to follow installation process, which you can use to set up your environment. However, there are some things I'd like to mention. 

- When you install Anaconda/Miniconda, ensure that you have the correct environment set up in the interpreter for VSCode. To do this, you can:
    - Open VSCode
    - Install Python extension (if not already installed)
    - Open the command palette (Ctrl+Shift+P on windows / Cmd+Shift+P on Mac)
    - Enter "Python:Select Interpreter" and select it
    - Choose the correct Anaconda/Miniconda environment

-  If you haven't be sure to activate your environment through the command line. To do this, open the Anaconda/Miniconda command line and enter the following command:

```
conda activate myenv
```

Ensure that you replace "myenv" with your environment name.

- If you wish to install packages, extensions, etc, directly to your environment, you can use the following command:

```
conda install *package name*
```

- If required, ensure that you read any relevant documentation needed for [Anaconda](https://docs.anaconda.com/index.html) or [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/).

# Libraries Used
Depending on how your base Python environment is set up, you may already have the required libraries installed. However, for clarity, the following libraries are used in the notebook:

- **Pandas (`pandas`)**: Used for data manipulation and analysis.
- **Matplotlib (`matplotlib`)** and **Seaborn (`seaborn`)**: Utilized for generating visualizations to better understand data and results visually.
- **NumPy (`numpy`)**: Provides support mathematical operations.
- **Random (`random`)**: Used for generating random numbers.
- **Operator (`operator`)**: Facilitates the mapping of arithmetic operations.
- **Itertools (`itertools`)**: Used to create permutations and combinations, critical for evaluating all possible operations sequences that could potentially solve the Countdown numbers game.
- **Functools (`functools`)**: The `reduce` function is used to apply functions cumulatively in the Reverse Polish Notation functions.


# How to run

This section provides a step-by-step guide on how to set up and run the Jupyter notebooks

### Step 1: Install Python
Ensure you have Python installed on your system. You can install it through the methods I outlined above.

### Step 2: Clone the Repository
Clone this repository to your local machine using Git. You can do this by running the following command in your terminal:
```
git clone https://github.com/Owen-kc/ComputationalTheory.git
```

### Step 3: Run Jupyter Notebook
If you have installed Anaconda or Miniconda, Jupyter Notebook should already be installed. Otherwise, install it using the following command:

```
pip install notebook
```
or you can install it through the VSCode extension.

### Step 4: Start Jupyter notebook

You can start the jupyter notebook you can run the following command:
```
jupyter notebook
```
You can use this command to open a navigation tree where you can select a specific notebook. **Note**: Depending on your own install, you may need to run this from your Anaconda/Miniconda terminal. If you are encountering errors launching the notebook in something like VSCode, you should open the Anaconda/Miniconda terminal, navigate to the repository using the following code command:

```
cd *path to repo on your system*
```

By following these steps, you should be able to run the contents of the repository.

# Project Overview

### Introduction
This project implements the Countdown numbers game from the TV show "Countdown," where contestants use arithmetic operations to reach a target number using six chosen numbers. The project is built in Python, focusing on computational theories and algorithm design.

### Objective
The main goals of the project are to:

- Identify computationl challenges in simple games.
- Apply different computational models to solve the game.
- Design the solve_numbers function using an efficient approach, particularly utilizing Reverse Polish Notation (RPA) and functional programming paradigms where possible.
- Analyze the efficiency and complexity of the algorithm.
- Visualize the output of the function and analyze it.

### Game Description and Rules
- Number Selection: Players choose six numbers from a set that includes large numbers (25, 50, 75, 100) and small numbers (1-10).
- Target Number: A random target between 101 and 999 is generated.
- Allowed Operations: Addition, subtraction, multiplication, and division, with the constraint that each operation must result in whole numbers and each number can be used only once.

### Strategy and Methodology
- Algorithm Design: The solve_numbers function simulates the game, enforcing rules about number usage and operations.
- Reverse Polish Notation (RPN): Employed for efficient expression evaluation, simplifying the computational logic by eliminating the need for operation precedence and parantheses.
- Functional Programming: The project utilizes immutable data structures and higher-order functions where possible to enhance the modularity and maintainability.

### Implementation Details
- `solve_numbers` Function: This method executes and outputs the result of the solution process, detailing each step taken by the functions and the entire solution. If there is more than one solution, the function outputs each solution and returns a total number of solutions at the end. 
- Random Number Generation: Method defined to mimic the games number selection process
- Validation and Optimization: Ensure all operations comply with the Countdown number game's rules and is optimized and efficient in the calculation process.

