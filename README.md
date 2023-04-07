# Installation of Softwares

## Anaconda
### Installation
To install Anaconda on your computer, follow these steps:

1. **Go to the Anaconda download page**: Visit the official Anaconda website at https://www.anaconda.com/products/individual and click on the "Download" button for the Python version you want to use.

2. **Choose the appropriate installer**: Select the installer for your operating system (Windows, macOS, or Linux) and the version of Python you want to use (Python 2.7 or 3.x).

3. **Download the installer**: Once you have chosen the appropriate installer, click on the "Download" button to download the installer file.

4. **Run the installer**: Once the installer has finished downloading, run the installer by double-clicking on the file. Follow the instructions provided by the installer.

5. **Agree to the license terms**: During the installation process, you will be asked to agree to the Anaconda license terms. Read the license terms and click on the "I Agree" button if you agree.

6. **Choose the installation location**: The installer will prompt you to choose the installation location. The default location is usually fine, but you can choose a different location if you prefer.

7. **Choose whether to add Anaconda to your PATH environment variable**: The installer will also ask you whether you want to add Anaconda to your system's PATH environment variable. This is usually a good idea, as it makes it easier to use Anaconda from the command line.

8. **Wait for the installation to finish**: Once you have made all the necessary choices, the installation will begin. Wait for the installation to finish.

Test the installation: Once the installation is complete, open a terminal or command prompt and type "conda list". If everything is installed correctly, you should see a list of installed packages and their versions.

Congratulations, you have now installed Anaconda on your computer! You can now start using it to work with Python, Jupyter Notebook, and other data science tools.

### How to use Anaconda
Conda environments are a powerful feature of the Anaconda distribution that allow you to create isolated Python environments with specific versions of packages and dependencies. This makes it easy to switch between different projects or collaborate with others without worrying about version conflicts or dependencies.

Here are the basic steps to create and use conda environments:

1. **Create a new environment**: Open a terminal or Anaconda prompt and run the following command to create a new environment with a specific version of Python:
```
conda create --name myenv python=3.9
```
This will create a new environment called "myenv" with Python 3.9 installed. You can replace "myenv" with any name you like, and you can also specify a different version of Python if you prefer.

2. **Activate the environment**: Once the environment is created, you can activate it by running the following command:
```
conda activate myenv
```
This will activate the "myenv" environment and any packages you install or run will use the Python version and packages installed in this environment.

3. **Install packages**: You can now install packages or dependencies in the new environment using the "conda install" command. For example:
```
conda install numpy matplotlib pandas
```
This will install the NumPy, Matplotlib, and Pandas packages in the "myenv" environment.

4. **Deactivate the environment**: When you're done working in the environment, you can deactivate it by running the following command:
```
conda deactivate
```
This will deactivate the "myenv" environment and return you to the base environment.

5. **Remove the environment**: If you no longer need the environment, you can remove it using the following command:
```
conda remove --name myenv --all
```
This will remove the "myenv" environment and all the packages installed in it.

These are the basic steps for creating and using conda environments. With conda environments, you can easily manage your Python projects and dependencies and ensure that your code works consistently across different systems.

## Pybullet
### Installation

You can install PyBullet on your PC by following these steps:

1. **Install Python**: If you don't already have Python installed on your PC, you can download it from the official website https://www.python.org/downloads/. Make sure to select the version that matches your operating system.

2. **Install pip**: pip is a package manager for Python that makes it easy to install and manage Python packages. If you have a recent version of Python, pip should already be installed. You can check if pip is installed by running the command `pip --version` in a terminal or command prompt.

3. **Install PyBullet**: Once you have Python and pip installed, you can install PyBullet by running the command `pip install pybullet` in a terminal or command prompt. This will download and install the latest version of PyBullet and any necessary dependencies.

4. **Verify the installation**: To verify that PyBullet is installed correctly, you can run the following code in a Python console or a script:

```
import pybullet as p

# Create a PyBullet physics simulation
p.connect(p.GUI)
p.setGravity(0, 0, -9.81)
planeId = p.loadURDF("plane.urdf")

# Close the PyBullet simulation
p.disconnect()
```
If the installation was successful, you should see a PyBullet simulation window pop up, showing a simple plane. If you see any error messages, double-check that you have installed PyBullet correctly and that your system meets the requirements.
