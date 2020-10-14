Programming Assignment 3
Due: Wed Oct 21, 10am

Problem
Create a program that allows the user to choose any of the three sports options described below and computes the relevant statistic in each case:

Quidditch Score Total: Determined based on the number of goals and whether or not the snitch was caught. A goal is scored by propelling the quaffle through a hoop and each earns the team 10 points. If a team catches the snitch, that team earns an additional 30 points. The snitch can be caught at most once. More details on Quidditch available from the International Quidditch Association.

(Simplified) Quarterback Rating: Defined as

100 * [5(completions/attempts – 0.3) + 0.25(passing_yards/attempts-3) + 20(touchdown_passes/attempts) + 2.375 – (25 * interceptions/attempts)]/6,

where attempts is the number of passing attempts made, completions is the number of completed passing attempts, touchdown_passes is the number of passes for a touchdown, and interceptions is the number of times the ball was intercepted. A perfect passer rating in the NFL is considered to be a 158.3. In addition to the rating, tell the user whether or not the quarterback is a perfect passer.

Gymnast Score: Begins with six scores, one for difficulty and five for execution, each between 0 and 10. Of the execution scores, the highest and lowest are dropped. The final score is given by the sum of the difficulty score and the average of the three remaining execution scores.

Input Validation:

Check if you are going to divide by zero when relevant, and do not do the calculation if that is the case.
Before typecasting user inputs to an int, check that it is only digits, and don’t typecast or do the calculation otherwise. (For this assignment, do not worry about checking if floats are valid.)
In any case where an error is detected, output an error message. Do not continue the calculation. You may additionally output a result of zero in such a case.
Instructions
Create a new Python file and place intro comments using the template below.
Use comments to write the algorithm your program will follow, including functions. Use the function decomposition described in the section below.
Create an Excel file with at least one test case for each control path in your algorithm. Use one row per test case with one column for the case's label, one column for each input, and one column for each corresponding output.
Write the Python code corresponding to each of your algorithm's steps.
Note: This assignment does not require a flowchart.

Test your program using your test cases. If the output doesn't match, correct your program.

Commit and push changes and check your repository on github.com to confirm your updates before the deadline.

Intro comments template
# Programmers: [your name]
# Course: CS151, Dr. Rajeev 
# Programming Assignment:
# Program Inputs: [What information do you request from the user?]
# Program Outputs: [What information do you display for the user?]
Function decomposition
Your program should have a function for at least each of the following tasks. You may have additional helper functions.

One function for each sport's calculation. These functions should receive all data needed through parameters and return their result. These functions should not use input or print.
One function to handle each sports option. These functions should use input to get the values from the user, call the relevant statistic function from the previous item, and print the result to the user.
A main function to drive the program.
Additionally, if you are in a team with three members:

A min_score and max_score functions which, given 5 scores, return the minumum and maximum scores respectively. Do not use the built-in min/max functions for this exercise.
Teams with two members may use the built-in min and max functions.

Submission
GitHub: Completed .py file (including comments).
Moodle: An Excel file with test cases (no flowchart required for this assignment.)
