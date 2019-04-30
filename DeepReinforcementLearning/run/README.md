To view the history of games and the MCTS process go into the 'logs' folder. You can view any log in any text editor. When the files become too large to open in a text editor you can open up any bash line and type in the following command:

tail -n 50 '../path/to/log/file.log'

This will give you the last 50 lines of the log of choice. Change the number to see more or less. You can also save to a file by using the > character and adding a file name.

tail -n 50 '../path/to/log/file.log' > AwesomeLogs.log

Beaware that the logs will increase over time after every game and this process will take up MASSIVE amounts of data storage on your computer.

To stop a log from running locate the 'loggers.py' file and set any log to 'True'. This will disable the log during training. You can also stop and start logs with this process if you only want to view the logs every couple of hours.