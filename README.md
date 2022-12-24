# CSC180-Project4

Problem Formulation  
In this project, you practice with genetic algorithm by using Distributed Evolutionary Algorithms in 
Python (DEAP), the most popular Python library for evolutionary computation 
 
The n-queens problem was first invented in the mid-1800s as a puzzle for people to solve in their spare 
time, but now serves as a good tool for discussing computer search algorithms. In chess, a queen is the 
only piece that can attack in any direction. The puzzle is to place a number of queens on a board 
in such a way that no queen is attacking any other. 
In this project, we use DEAP to solve the 8  queens puzzle. The  8 queens  puzzle  is  the  problem  of  
placing  eight  queens  on  an  8  ×  8  chessboard  so  that  no  two  queens  attack  each  other. The eight 
queens puzzle is an example of the more general N queens problem of placing n non-attacking queens 
on an n ×n chessboard, for which solutions exist for all natural numbers with the exception of n = 2 
and n = 3. 
 
 
One way we can describe the board above is to say it has a cost of 0, because there are 0 pairs of 
queens attacking each other. We can then generalize this to say the cost of a given n-queens board 
is equal to the sum total number of distinct pairs of queens that are in the same row, column, or 
diagonal.  Consider this 5-queens puzzle. There are 5 pairs of queens attacking each other therefore the 
cost of this board is 5. 
 
 
 
 
2.  Major Challenges  
 
When we use DEAP, there are two major challenges: 
 
• How  should  we  encode  each  board  (a  given  arrangement  of  eight  queens)  using  numbers,  i.e.,  
what should the best numeric representation of each board? 
• How to write a (fitness) function to calculate the cost of any given board? 
 
 
 
 
 
3.  Chessboard Representation 
In this project, let us compare two different board representations.  
• Position-indexed-based: On an 8 × 8 board, each position will be represented as an integer 
from 0 to 63.We use one integer to represent the position of a queen.  Each board is a list of e
ight numbers (each number is taken from 0 to 63).   For example:   [14, 35, 51, 42, 12, 47, 62,
 2] 
 
 
 
• Row-indexed-based:  Each  row  of  the  board  is  indexed  from  0  to  7.    We  place  different  
queens on different rows from top to bottom. The sequence [a b c d .... ] means that in 0-
th row, a-th column, the  queen is present and so  on. Each board is a list of eight numbers 
(each number is taken from 0 to 7).  
 
 
 
4.  Notebook 
 
Write your code to complete the provided notebook on Canvas. For each representation, show the 
chessboard with eight queens you end up with having fewest conflicts as well as its fitness value.   
Note: you may try different GA parameters and run the code a few times to achieve the perfect 
chessboards without any conflicts.  
 
Compare the two chessboard representations and describe which one is better, e.g., in terms of 
ease of coding or final solution quality.    
 
Try different mutation and crossover operations and vary the number of generations and the population 
size to see the changes.  Write your findings in the report. 
