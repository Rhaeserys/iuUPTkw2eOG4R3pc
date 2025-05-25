Project Setup Guide
This document outlines the necessary steps to prepare your environment before running the project code. These steps ensure that you have the correct Python environment and all required packages installed. This project was developed and tested using Visual Studio.

1. Environment Creation
Before installing any packages, it's crucial to create an isolated Python environment. This prevents conflicts between project dependencies and your global Python installation.

Using Visual Studio:

Open your project in Visual Studio.

Go to View > Other Windows > Python Environments.

Click on "+ Add Environment...".

Choose to create a Virtual environment (venv) or a Conda environment.

Name: Give your environment a descriptive name (e.g., .venv, myproject-env).

Location: It's good practice to create it within your project folder.

Base interpreter: Select your desired Python interpreter (e.g., Python 3.9, 3.10, etc.).

Click "Create".

Once created, ensure this new environment is activated for your project. You can usually do this by right-clicking the environment in the "Python Environments" window or setting it in your project's properties.

(For users not using Visual Studio, they can create a virtual environment using commands like python -m venv .venv and then activate it.)

2. Package Installation
Once your environment is created and activated, you need to install the necessary Python packages. The following packages were used in this project:

pip: The Python package installer. The version used during development was 25.1.1. Your environment should come with pip pre-installed. You can upgrade it if needed using python -m pip install --upgrade pip.

Pandas: For data manipulation and analysis. Version 2.2.3 was used.

pip install pandas==2.2.3

Scikit-learn: For machine learning algorithms and tools.

pip install scikit-learn

Matplotlib: For creating static, animated, and interactive visualizations.

pip install matplotlib

Seaborn: A data visualization library based on Matplotlib, providing a high-level interface for drawing attractive and informative statistical graphics.

pip install seaborn

gdown: For downloading files from Google Drive.

pip install gdown

TensorFlow: An end-to-end open-source platform for machine learning.

pip install tensorflow

NumPy: Fundamental package for numerical computation in Python. (Note: NumPy is often installed as a dependency of Pandas, Scikit-learn, or TensorFlow, but it's good to be aware of it.)

pip install numpy

Installation Command Summary:

You can typically install these using pip from your activated environment's terminal. The command python -m pip is a way to ensure you are using the pip associated with your currently active Python interpreter.

# Ensure pip is up-to-date (optional, but good practice)
python -m pip install --upgrade pip

# Install the required packages
python -m pip install pandas==2.2.3 scikit-learn matplotlib seaborn gdown tensorflow numpy

Alternatively, if a requirements.txt file is provided with the project, you can install all dependencies at once using:

python -m pip install -r requirements.txt

(You might want to create a requirements.txt file for your project by running pip freeze > requirements.txt from your activated environment after installing all packages. This makes it easier for others.)

Next Steps
Once the environment is set up and all packages are installed, you should be able to run the project code as described in the subsequent sections of this README or other project documentation.

This setup guide assumes you have Python installed on your system and are familiar with basic command-line or terminal operations.
