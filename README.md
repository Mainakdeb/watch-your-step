# watch-your-step

The 'frozen-lake' environment is a grid which contains a starting point, ice blocks, holes and a goal block. Each of them are represented by an alphabet :
* S represents the starting point of tehe agent, it's safe. 
* F represents the frozen surface which too is safe.
* H represents a hole and if our agent steps into the hole, the episode terminates (he dies). 
* G represents the goal where the agent wants to reach.

There are 4 possible actions the agent can execute :
* Go up.
* Go Down.
* Go right.
* Go left.

The agent plays 9500 episodes on its own, making relevant changes to the Q table along the way.
![Test](https://github.com/Mainakdeb/watch-your-step/blob/master/images/update-Q-table.png)

This updated Q table guides the agent to the goal in the given cases below.

## When is_slippery = False :
![Test](https://github.com/Mainakdeb/watch-your-step/blob/master/gifs/frozen-lake-2.gif)

In this case, the agent always chooses the shortest path and successfully executes all the intended actions. 

## When is_slippery = True :
![Test](https://github.com/Mainakdeb/watch-your-step/blob/master/gifs/frozen-lake-1.gif)

The intended action (from the Q table) is not always successfully executed. The agent 'slips' most of the time but still reaches the goal. 


