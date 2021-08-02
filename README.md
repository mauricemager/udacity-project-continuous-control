[//]: # (Image References)

[image1]: https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif "Trained Agent"

# Train a Unity Environment (Banana field) using Deep Q-learning (DQN)

## The Environment

This project works with the Unity ML-Agent Reacher Environment. In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.




![Reacher Environment][image1]


- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, the environment is considered solved when the trained agent achieves an average score of +13 over 100 consecutive episodes.

## Getting Started

1. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__: 
	```bash
	conda create --name drlnd python=3.6
	conda activate drlnd
	```
	- __Windows__: 
	```bash
	conda create --name drlnd python=3.6 
	activate drlnd
	```


2. Perform minimal installation of OpenAI Gym with PyPI
    ```
    pip install gym  
    ```

3. Clone this repository and navigate to the `python/` folder. Then, install several dependencies. 
    ```
    git clone https://github.com/mauricemager/udacity-project-continuous-control.git
    cd udacity-project-navigation/python
    pip install .
    ```

4. Create an [IPython kernel](https://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the drlnd environment.
    ```
   python -m ipykernel install --user --name drlnd --display-name "drlnd"
    ```

5. Move one folder up, and open the `Navigation.ipynb` notebook. 
   Next, change the Python3 kernel to the new installed drlnd kernel under (_Kernel > Change Kernel > drlnd_)

    ```
    cd ..
    jupyter notebook Continuous_Control.ipynb
    ```

6. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS or headless machines_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md))
, then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) to obtain the environment.


7. Place the downloaded `Banana` directory in the `data` directory and make sure the path to the `Banana.x86_64` file matching to your system in cell 2 of the Navigation notebook


8. Run all the cells of the `Navigation.ipynb` to see training and evaluation of the model

