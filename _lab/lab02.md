---
layout: lab
num: lab02
ready: true
desc: "Input/Output and Simple Flow"
assigned: 2017-04-12 08:00:00.00-7
due: 2017-04-18 12:00:00.00-7
---

<div markdown="1">

<h1>CS16: Programming Assignment 02</h1>
<h2>Introduction</h2>
The assignment for this week will utilize concepts of input and output and simple control flow (Chapter 2 in the book). We will cover these topics in class this week.

<h2>Step 1: Getting Ready</h2>
If you have not gotten a CoE account yet, please do so as soon as possible!
Open a terminal window and log into the correct machine - refer to the instructions in Lab #1, if you forgot how to do that.

Start by changing into your CS 16 directory:

`$ cd cs16`

And then create and change into the lab02 directory:

`$ mkdir lab02`

`$ cd lab02`

Remember that at any time, you can check what directory you are currently in with the command <b>pwd</b>.

<h2>Step 2: Create and Edit Your C++ Files</h2>
For a reminder on how to open and use a text editor to create and edit new source files, refer back to Lab #1.

This assignment consists of 3 problems, each of which is described below. The first two are worth 30 points each, and the last is worth 40 points. Each should be solved in its own file and all three must be submitted for full assignment credit. These exercises are inspied by ones from the textbook (in Ch. 2) - but they are NOT the same, so follow the instructions on THIS sheet carefully.

<h2>COINS.CPP</h2>
Write a program that allows the user to enter a number of quarters, dimes, and nickels and then outputs the monetary value of the coins in cents. For example, if the user enters 2 for the number of quarters, 3 for the number of dimes, and 1 for the number of nickels, then the program should output that the coins are worth 85 cents.

The program should print a string of text to the terminal before getting each piece of input from the user. A session should look <b><i>exactly</i></b> like the following example (including whitespace and formatting), with possibly different numbers for inputs and the output (so the following is just ONE example of how the program might run, but the FORMATTING has to be exactly the same in order for you to get full credit):

<img src="coins_img.PNG" alt="coins program example" />

Each string printed by the program should include a newline at the end, but no other trailing whitespace (i.e. extra space characters at the end of the line).

<h3>BLOCK.CPP</h3>
Write a program that takes input from a user for number of rows and number of columns and prints out a block of characters that is based on these 2 parameters. The program should keep asking the user for input, and printing out the result, until the user enters zero for each of the input parameters.

A session should look <b><i>exactly</i></b> like the following example (including whitespace and formatting - although note that there is no whitespace at the end of each of these lines), with all manners of different numbers for inputs and the output:

<img src="block.png" width="700" alt="block program example" />

Each string printed by the program should include a newline at the end, but no other trailing whitespace (i.e. extra space characters at the end of the line).

<h3>PI.CPP</h3>
Write a C++ program that approximates the value of the constant π, based on the Leibniz formula for π. The formula is shown in the image below:

<img src="pi_formula.png" alt="pi formula" />

Put another way, the formula can be written as:

pi = 4 · [ 1 – 1/3 + 1/5 – 1/7 + 1/9 ... + (–1 ^ n)/(2n + 1) ]

The Leibniz formula works well for high values of n.

The program takes an input from the user for the value of n, which determines the number of terms in the approximation of the value of pi. The program then outputs that calculation. You must also include a loop that allows the user to repeat this calculation for new values n until the user says she or he wants to end the program by issuing an input of 0.

The program should print a string of text to the terminal before getting each piece of input from the user. A session should look like the following example (including whitespace and formatting), with various and different inputs and numbers in the output:

<img src="pi.png" width="700" alt="pi program example" />

Note that each string printed by the program should include a newline at the end, but no other trailing whitespace (whitespace at the end of the line).

In addition, all approximated floating pointer numbers must be displayed to exactly three  digits after the decimal point.

<h2>Step 3: Compile the Codes</h2>

To compile our codes, we will use the same g++ command as we described in previous labs. The following three commands will compile the three source files (in the same order as listed above):

`$ g++ -std=c++11 -o block block.cpp`

`$ g++ -std=c++11 -o coins coins.cpp`

`$ g++ -std=c++11 -o pi pi.cpp`

(NOTE: the -std=c++11 option in these commands is optional to use (that is, not critical to define). All this does is force the compiler to use the latest version of C++).

If the compilation is successful, you will not  see any output from the compiler. You can then use the following commands to run your programs:

`$ ./block`

`$ ./coins`

`$ ./pi`

<b>If you encounter an error, use the compiler hints and examine the line in question. If the compiler messsage is not sufficient to identify the error, you can search online to see when the error occurs in general.</b>

Remember to re-compile the relevant files after you make any changes to the C++ code.

<h2>Step 4: Submit</h2>

Once you are satisfied that your programs are correct, it is time to submit them. Login at [https://submit.cs.ucsb.edu](https://submit.cs.ucsb.edu), then navigate to “CS16_f16” and click on “lab02”. Then click “Make Submission”, and make your submission the same way as last week. Remember to submit all three .cpp files.

Please remember that you must submit the programs to obtain any credit for the assignment; just completing the programs is not enough.

Once you submit, you should see a page detailing your submission. The system will automatically grade your program and will show you the results on this page after a 1 minute delay.

You can alternatively submit your code from the command line (terminal) on any CS machine, including the Phelps lab machines or the CSIL server. You can use this method when logged in remotely. To submit the the three source files to this assignment by running the command:

`$ ~submit/submit -p 696 block.cpp coins.cpp pi.cpp`

You can copy the URL shown in the output of the above and paste into a web browser to reach the submission result page.

<h2>Step 5: Check Submission Results</h2>

After the 1 minute delay, the submit system will show your score and give you feedback on your submission. Refresh the webpage after a minute to see this information.

You may submit this lab multiple times. You should submit only after local compilation does not produce any errors and runs as expected. The score of the last submission uploaded before the deadline will be used as your assignment grade.

<h2>Step 6: Done!</h2>

Once your submission receives a score of 100/100, you are done with this assignment.

If you are in the Phelps lab or in CSIL, make sure to log out of the machine before you leave. Also, make sure to close all open programs before you log out. Some programs will not work next time if they are not closed. Remember to save all your open files before you close your text editor.

If you are logged in remotely, you can log out using the exit command:

`$ exit`

</div>
