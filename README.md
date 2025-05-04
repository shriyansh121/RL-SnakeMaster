# RL-SnakeMaster
A classic Snake game built using reinforcement learning algorithms. The agent learns to navigate and grow by optimizing reward-based strategies. Ideal for exploring RL concepts in game environments with visual feedback and training dynamics. Clean, modular, and educational.


Step by step what to do:

First declare all the requirements needed for snake game including directions color blaock size and speed
Step1:
making a class named snakegameai and setting the width and height accordingly.

Step 2:
In that class display ui of game ,set caption, set clock time and call reset function.

Step 3: Reset Function 
at the start of game snake will be facing the direction of right and will move in right direction
place head of snake at hte center of ui block.
the rest of the body of snake is defined. the value of y axis will remain same and value of x axis will decrease as the body of snake is forming in right direction
now initialize score and food and call food placing fucntion
initialize frame iteration

Step 4: Food placing function
x and y are two corodinates of where food is going to appear. One important thing to keep in mind here is block size. bloack size is the size of square of which snake body is made of. So its is important to keep in mind while generating coordinates of food that snake can reach it and eat it otherwise snake could never reach the food is coordinates do not align with sblock size of snake. Once snake eats food its size increases and food placing function is called again.
Step 5: Play Step
the frame iteration keeps increasing by one. It has several sub steps to be followed.
collect user input
move the snake by updating it's head and check if the game is over.
