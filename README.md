Download Link: https://assignmentchef.com/product/solved-eecs658-assignment-8
<br>
Deliverables:

<ol>

 <li>Copy of Rubric8.docx with your name and ID filled out (do not submit a PDF)</li>

 <li>Python source code.</li>

 <li>Screen print showing the successful execution of your Python code. (Copy and paste the output from the Python console screen to a Word document and PDF it).</li>

 <li>Answer to Part 1, Question 1. 5. Answer to Part 2, Question 2. 6. Answer to Part 3, Question 3. 7. Answer to Part 3, Question 4. 8. Answer to Part 3, Question 5. 9. Answer to Part 4, Question 6. 10. Answer to Part 4, Question 7.</li>

 <li>Answer to Part 4, Question 8.</li>

</ol>




Assignment:

<ul>

 <li>For all Parts, we are going to use the same modified version of the Gridtask World, which we used for Assignment 7:</li>

</ul>

<table width="192">

 <tbody>

  <tr>

   <td width="38"> </td>

   <td width="38">1</td>

   <td width="38">2</td>

   <td width="38">3</td>

   <td width="38">4</td>

  </tr>

  <tr>

   <td width="38">5</td>

   <td width="38">6</td>

   <td width="38">7</td>

   <td width="38">8</td>

   <td width="38">9</td>

  </tr>

  <tr>

   <td width="38">10</td>

   <td width="38">11</td>

   <td width="38">12</td>

   <td width="38">13</td>

   <td width="38">14</td>

  </tr>

  <tr>

   <td width="38">15</td>

   <td width="38">16</td>

   <td width="38">17</td>

   <td width="38">18</td>

   <td width="38">19</td>

  </tr>

  <tr>

   <td width="38">20</td>

   <td width="38">21</td>

   <td width="38">22</td>

   <td width="38">23</td>

   <td width="38"> </td>

  </tr>

 </tbody>

</table>

<ul>

 <li>The goal of the Gridworld Task is for a robot, starting at any square in the grid, to move through the grid and end up in a termination state (grey squares) which ends the game.</li>

 <li>Each grid square is a state (s).</li>

 <li>The actions (a) that can be taken are up, down, left, or right.</li>

 <li>The rewards (r) will be different for each Part.</li>

 <li>Assume for all 4 Parts:</li>

</ul>

o γ (Gamma) = 0.9

<ul>

 <li>Separate the output for each Part by printing out a line identifying which Part the output is from.</li>

</ul>




Part 1: RL Monte Carlo First Visit Algorithm

<ul>

 <li>Write a Python program that uses the RL Monte Carlo First Visit algorithm to develop an optimal policy (π*).</li>

 <li>The rewards (r) are:

  <ul>

   <li>-1 on all transitions o 0 terminal state</li>

   <li>-1 when it hits a wall (no transition, but still a reward)</li>

  </ul></li>

 <li>The program should print out the N(s), S(s), and V(s) arrays with the epoch number for epoch 0 (the initial values), epoch 1, epoch 10, and the final epoch.</li>

 <li>The program should also print out an array showing k, s, r, γ, and G(s) for all values of k for epoch 1, epoch 10, and the final epoch.</li>

 <li>Determine a method for deciding when the Monte Carlo algorithm has converged.</li>

 <li>Question 1: Explain the convergence method and why you picked it. There is no wrong answer. You will get credit for any method you pick as long as it converges and you provide a reasonable explanation of why you picked it.</li>

</ul>




Part 2: RL Monte Carlo Every Visit Algorithm

<ul>

 <li>Write a Python program that uses the RL Monte Carlo Every Visit algorithm to develop an optimal policy (π*).</li>

 <li>The rewards (r) are:

  <ul>

   <li>-1 on all transitions o 0 terminal state</li>

   <li>-1 when it hits a wall (no transition, but still a reward)</li>

  </ul></li>

 <li>The program should print out the N(s), S(s), and V(s) arrays with the epoch number for epoch 0 (the initial values), epoch 1, epoch 10, and the final epoch.</li>

 <li>The program should also print out an array showing k, s, r, γ, and G(s) for all values of k for epoch 1, epoch 10, and the final epoch.</li>

 <li>Use the same method for deciding when the Monte Carlo algorithm has converged as you did in Part 1.</li>

 <li>Question 2: Did Part 1 and Part 2 converge in the same number of epochs? Why? There is no right or wrong answer as long as you make a reasonable attempt to explain why.</li>

</ul>

Part 3: RL Q-Learning Algorithm

<ul>

 <li>Write a Python program that uses the RL Q-Learning algorithm to develop an optimal policy (π*). The rewards (r) are:

  <ul>

   <li>100 on transitions to the terminal state o 0 on all other transitions</li>

  </ul></li>

 <li>Question 3: Draw a Q-Learning State Diagram for the Gridtask World above.</li>

 <li>Your program should first display the Q-Learning Rewards Matrix (R) as a Python array.</li>

 <li>The program should print out the Q-Learning Value Matrix (Q) with the episode number for episode 0 (the initial values), episode 1, episode 10, and the final episode.</li>

 <li>Determine a method for deciding when the Q-Learning algorithm has converged.</li>

 <li>Question 4: Explain the convergence method and why you picked it. There is no wrong answer. You will get credit for any method you pick as long as it converges and you provide a reasonable explanation of why you picked it.</li>

 <li>Question 5: Based on your final Value Matrix (Q) what is the optimal path from square 7 to the upper left-hand termination state. Part 4: RL SARSA Algorithm</li>

 <li>Write a Python program that uses the RL SARSA algorithm to develop an optimal policy (π*).</li>

 <li>Use the same Q-Learning State Diagram for the Gridtask World that you developed for Part 3.</li>

 <li>Your program should first display the SARSA Rewards Matrix (R) as a Python array.</li>

 <li>The program should print out the SARSA Value Matrix (Q) with the episode number for episode 0 (the initial values), episode 1, episode 10, and the final episode.</li>

 <li>Determine a method for deciding when the SARSA algorithm has converged.</li>

 <li>Question 6: Explain the convergence method and why you picked it. There is no wrong answer. You will get credit for any method you pick as long as it converges and you provide a reasonable explanation of why you picked it.</li>

 <li>Question 7: Based on your final Value Matrix (Q) what is the optimal path from square 7 to the upper left-hand termination state.</li>

 <li>Question 8: Did Part 3 and Part 4 converge in the same number of episodes? Why? There is no right or wrong answer as long as you make a reasonable attempt to explain why.</li>

</ul>




Remember:

<ul>

 <li>Your Programming Assignments are individual-effort.</li>

 <li>You can brainstorm with other students and help them work through problems in their programs, but everyone should have their own unique assignment programs.</li>

</ul>