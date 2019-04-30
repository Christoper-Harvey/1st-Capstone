
To answer the first question I researched Alpha Zero from DeepMind. I created a working replica of there original methodology. I first trained it on Tic Tac Toe, TTT, as I do not have the computational power to train an agent on chess!

The agent took 5 hours to train running on my personal gtx 1080 graphics card. It learned how to play the game using a Monte Carlo Tree Search, MCTS, which learns from experience. It also used an Actor Critic model with a residual CNN as the Critic and a MCTS powered ResNet as the Actor.

This is what the error for the model over time looked like.

<img src="https://media.githubusercontent.com/media/Christoper-Harvey/1st-Capstone/master/Tic%20tac%20Toe/standard/ttt_std2_IterationsOverTime.png" >

As you can see it reduces quickly then levels out. This is a fairly stable result. Doing the same for Connect 4, and MetaSquares I am sure that the agent learned generalities and strategy for each game and quickly surpases human level.

Each generation of model makes large steps forward. After only 3 generations of TTT models the agent mastered the game and played perfectly no matter what the opponent does. I call this a 'Solved Model' because TTT and C4 are 'Solved' games meaning that humans have mathematically came up with a solution to the game to where is both players played perfectly it would result in this every time. TTT's solved state is a draw. C4's solved state is player 1 winning.

So I knew the model achieved complete success when they followed the perfect game almost every time.



