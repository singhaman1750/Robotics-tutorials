# Installation of Softwares

## Anaconda
### What is Anaconda 
Anaconda is a free and open-source distribution of the Python and R programming languages for scientific computing, data science, and machine learning. It includes many popular data science packages and tools such as Jupyter Notebook, Spyder, NumPy, Pandas, Matplotlib, Scikit-learn, and many others.

Anaconda provides a convenient way to manage Python and R environments, allowing you to create isolated environments with specific versions of packages and dependencies. This makes it easy to switch between different projects or collaborate with others without worrying about version conflicts or dependencies.

Anaconda also includes a package manager called conda, which makes it easy to install, update, and manage packages and dependencies from the command line.

Overall, Anaconda is a powerful and convenient tool for data scientists, researchers, and developers who need a reliable and easy-to-use platform for scientific computing and data analysis.

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
### What is Pybullet
PyBullet is a physics engine and simulation environment for robotics, machine learning, and computer graphics research. It provides accurate and efficient physics simulation, including rigid body dynamics, collision detection and response, contact forces, and friction. PyBullet supports a wide range of robots and objects, and provides a range of built-in controllers and optimization algorithms for controlling them. It is designed to be easy to use and integrate with popular programming languages and frameworks, and is available under the permissive zlib license. Overall, PyBullet is a powerful tool for simulating complex dynamic systems and testing algorithms and controllers in a virtual environment.

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

## Mujoco
### What is Mujoco
MuJoCo (Multi-Joint dynamics with Contact) is a physics engine for simulating dynamic environments with complex robots and other articulated bodies. It is widely used in robotics, biomechanics, and computer graphics research for modeling and simulating systems with complex dynamics, including human and animal movements, industrial robots, and other multi-body systems.

MuJoCo uses a rigid body dynamics engine to simulate the physics of articulated bodies, including collisions, contact forces, friction, and joint constraints. It also provides a range of built-in controllers and optimization algorithms for controlling robots and other dynamic systems.

MuJoCo has a user-friendly interface and can be easily integrated with popular programming languages and robotics frameworks, such as Python, MATLAB, ROS, and OpenAI Gym. It is available under a proprietary license and requires a license fee for commercial use. However, academic and personal licenses are available for free.

Overall, MuJoCo is a powerful and flexible physics engine that enables researchers and developers to simulate complex dynamic systems and test their algorithms and controllers in a virtual environment.

### Installation
Here are the basic steps to install MuJoCo on your system:

1. **Download MuJoCo**: Go to the MuJoCo website (www.mujoco.org) and download the version of MuJoCo that matches your operating system (Windows, Linux, or macOS) and the version of Python you are using. Note that MuJoCo requires a license key for commercial use, but academic and personal licenses are available for free.

2. **Install MuJoCo**: Unzip the MuJoCo package to a location of your choice (e.g., ~/mujoco/mujoco200 for MuJoCo version 2.0.0). Add the path to the MuJoCo binaries and libraries to your system's environment variable. For example, on Linux, you can add the following line to your .bashrc file:
```
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/path/to/mujoco200/bin:/path/to/mujoco200/bin
```
3. **Install MuJoCo Python bindings**: Install the MuJoCo Python bindings using pip by running the following command:
```
pip install mujoco-py
```
This will download and install the Python bindings for MuJoCo.

4. **Test the installation**: To verify that MuJoCo is installed correctly, you can run the following Python code to open a MuJoCo environment and render it:
```
import mujoco_py
import os

model_path = os.path.join(os.path.dirname(mujoco_py.__file__), 'xmls', 'humanoid.xml')
model = mujoco_py.load_model_from_path(model_path)
sim = mujoco_py.MjSim(model)

while True:
    sim.step()
    viewer.render()
```
This code will load the "humanoid" MuJoCo model and simulate it in a window.

These are the basic steps for installing MuJoCo on your system. MuJoCo can be a powerful tool for simulating complex dynamics in robotics and other fields, and it is widely used in research and development.
