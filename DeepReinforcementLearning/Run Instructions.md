To run the model download this github repo and create an environment with either pip or conda.

Use the requirements.txt file to install all required packages for this project.

While the GPU version of this software is not needed it is recommended to run on GPU as this process is very slow and computationally heavy!!!

If you run into errors with running the code install keras 2.2.4 manually from their github repo at https://github.com/keras-team/keras

Once you have all the packages installed cd into the folder that you used to download this repo. Open a command line and run this command:

jupyter notebook

After which jupyter will open up and you should be able to work with the files. You can edit the 'config.py' and 'game.py' files as you wish.

When you are ready to run, open up the 'train.ipynb' and if you are using gpu run all of the commands. if you are not using gpu just run the first command to import the modules and then run the 3rd command to start the training process.

The last two commands are to see the layers of the ConvResNet and to output a diagram of it.

To start the training process from a past starting point put in the version of the model, memory, and run number into the 'run_archive' folder. Then edit the file 'initialize.py' as stated in the file.

When you have versions of the game you want to compete or if you want to compete my versions. Open the 'test.ipynb' file and run the first command then edit the second command as follows:

env = Game()
playMatchesBetweenVersions(env, 1, 2001, 3001, 20, lg.logger_tourney, 0) # -1 for human players

playMatchesBetweenVersions(env, run_version, player1version, player2version, EPISODES, logger, turns_until_tau0, goes_first = 0)

Do not change the env, run_version, or logger. These are set variables that will throw errors at you. If you wish to change the player versions enter in the versions into the player1version and player2verions variables. The episodes variable is how many games the players will play in the tournament. The turns_until_tau0 varibale is how many games are random until they start trying; I recommend leaving it at 0 but if you want to change it go for it.

To edit the players settings go to the 'config.py' file in 'DeepReinforcementLearning' and in the 'run' folders.
