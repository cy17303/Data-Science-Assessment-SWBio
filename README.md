# Distributional-Temporal-Difference-Decoder

This is a pipeline written in python (version 3.10) to simulate ‘neural activity’ during receipt of reward in an environment where receipt of this reward is guaranteed.  This is done by using the distributional temporal difference algorithm, pioneered by Bellemare, et al., (2017), and a customisable ‘guaranteed reward environment’. 
These distributions of neural activity are thus parsed through dense neural nets which act as decoders, to determine if these distributions of ‘activity’ represent reward in the environment. 

To run: 
1)	Download the python notebook in this repository and open in a GPU enabled interface (e.g. google colab).
2)	Ensure that all necessary libraries are installed. All are included in the Anaconda distribution. If the user does not have anaconda, and does not wish to install it, libraries can be installed using the !pip command. A blank notebook cell has been inserted at the top of the notebook for this. 
3)	Edit the pipeline to change the hyperparameters of the neural network and environments. These include the number of states in the environment, the number of training and testing  iterations in the environment, the reward distribution used for training / testing, the base learning rate, the discount factor for calculation of temporal difference error, the number of training epochs in the neural network and the number of steps per epoch. This can mostly be done by changing the hyperparameters when calling functions. Base learning rate, discount factor, and neural network hyperparameters should be changed within the code.

The parameters in the downloaded notebook are those used to produce the data presented in the accompanying report.

4)	Execute each cell in order. This should result in a KDE plot and violin plot which checks the zero crossing assumption, a scatter plot which checks the assymmetric learning assumption, and a learning curve for the dense neural network decoder.


No data needs to be downloaded, as all data is simulated within the notebook. 





