Download Link: https://assignmentchef.com/product/solved-cs145-homework-3-knn-and-neural-networks
<br>
Code of HW3 has been tested to be compatible with python version 3.6 (it may work with other versions of 3.X, but we won’t be officially supporting them.). You will need to make sure that during your virtual environment setup that the correct version of <sub>python</sub> is used. If you would like to use Python 2.7, it is also OK but keep in mind that you may have problems or errors, which may take extra efforts.

Set up Python 3 (For Mac OS/Linux)

Most of you have already installed Python 3 for previous assignments. If you have done that, you can skip this step. It is recommended to install <a href="https://www.anaconda.com/download/#macos">Anaconda</a> to manage Python and packages. Other than that, for Mac OS X, you can also install Python 3 via <a href="https://brew.sh/">Homebrew</a> and call <sub>brew install </sub>python3 . For Linux, you can install through sudo apt-get .

Set up Virtual Environment (For Mac OS/Linux)

In case you have different python package version and other issues, we recommend to use Python <a href="https://docs.python-guide.org/dev/virtualenvs/">virtualenv</a> which sets up a vitural environment. At a high-level, a virtual environment creates an environment where you may install packages that aren’t installed on your main system Python. This is useful for separating out projects. Further, if you accidentally break your Python during some package installation (it can happen and is not fun), but you were in a virtual environment, you can simply delete the virtual environment and start a new. Use <sub>pip</sub> to install it: <sub>sudo pip </sub>install virtualenv .

Please run the following in the terminal to start visual environment and install required packages of HW3 after installation:

cd HW3 virtualenv -p python3 .env       # Create a virtual environment (python3) # Note: you can also use “virtualenv .env” to use your default python source .env/bin/activate         # Activate the virtual environment pip install -r requirements.txt  # Install dependencies (this takes a while) # Work on the homework for a while … deactivate                       # Exit the virtual environment

Alternatively, you can use Anaconda to set up virtual environment if you have installed it. To set up a virtual environment with Anaconda, run (in a terminal):

conda create -n .env python=3.6 anaconda    # Create an environment called

.env source activate .env                        # Activate and enter the environment

# Work on the homework for a while … source deactivate .env                      # Exit the virtual environment

Check <a href="https://conda.io/docs/user-guide/tasks/manage-environments.html">here</a> for more details on managing virtual environments with Anaconda.

<strong>Do I have to use virtual environment?</strong> The answer is “No, probably you don’t”. Be advised, however, that if you choose not to use virtual environment, it is up to you to make sure all dependencies in the code are installed globally on your machine. However, if things break, it is not possible for us to help debug each student’s unique installation, as each computer setup is different, and the bug may be any package you have previously used or installed interacting negatively. That is why we prefer to have you use virtual environments and have provided you the <sub>requirements.txt</sub> file for the homework.

Installing Python and virtualenv for Windows

Download Python package from <a href="https://www.python.org/downloads/release/python-364/">https://www.p</a><a href="https://www.python.org/downloads/release/python-364/">y</a><a href="https://www.python.org/downloads/release/python-364/">thon.or</a><a href="https://www.python.org/downloads/release/python-364/">g</a><a href="https://www.python.org/downloads/release/python-364/">/downloads/release/p</a><a href="https://www.python.org/downloads/release/python-364/">y</a><a href="https://www.python.org/downloads/release/python-364/">thon-364/</a> and install it. Run cmd as administrator and run these commands:

<em>Note: We find the setup instructions from online (but all TAs do not have Windows sorry). Please tell us if you have problems. We suggest to search on StackOverflow or post your problem on Piazza first.</em>

Set up and Launch Jupyter Notebook

To finish this homework, we use <sub>jupyter notebook</sub> for coding and report. An IPython notebook lets you write and execute Python code in your web browser. IPython notebooks make it very easy and interactive to tinker with code and execute it in steps. Check <a href="https://jupyter.org/">here</a> for more details if you are not familiar with Jupyter Notebook and how it works.

If your virtual environment installed correctly, you should <strong>NOT </strong>have to manually install it from the instructions on the website. Just remember to run source .env/bin/activate in your homework folder.

probably a little bit more convenient .

This will launch a new browser window (or a new tab) showing the notebook dashboard. Or you can visit http://localhost:8888/ to open the dashboard.

When started, the jupyter notebook can access only files within its start-up folder (including any sub-folder). Make sure your relevant files are on the desired path.

<strong>Note:</strong> To write down the answers in the notebook, you may need a little knowledge of <strong>markdown </strong>syntax, which is basically like txt but more flexible and readable. <a href="https://guides.github.com/features/mastering-markdown/">Here</a> is a brief tutorial. (Fun fact: You can even use it when posting on Piazza!)

Congratulations for completing the setup for your coming exciting homework! Now let’s start! ^_^

<h1>Data Preparation</h1>

Download the CIFAR-10 dataset (file size: ~163M). Run the following from the <sub>HW3</sub> directory:

cd cs145/datasets ./get_datasets.sh

Also you can download the dataset <a href="http://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz">here</a>, and put it under <sub>cs145/datasets</sub> folder.

After downloading the dataset, you can start your notebook from the <sub>HW3</sub> directory.

<h1>Task 1: KNN</h1>

<strong>Task</strong>: Complete the k-nearest neighbors Jupyter notebook including codes and questions (following the instructions and notes in <sub>knn.ipynb </sub>). The goal of this workbook is to give you experiences with the CIFAR-10 dataset, training and evaluating a simple classifier, and k-fold cross validation.

Print out the entire workbook and submit jupyter notebook together with all source codes.

<h1>Task 2: Two-layer Neural Networks</h1>

<strong>Task</strong>: Compete the two-layer neural network Jupyter notebook including codes and questions (following the instructions and notes in <sub>toy_nn.ipynb </sub>). Print out the entire workbook and submit jupyter notebook together with all source codes.


