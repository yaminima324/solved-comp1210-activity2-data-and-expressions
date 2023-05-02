Download Link: https://assignmentchef.com/product/solved-comp1210-activity2-data-and-expressions
<br>
<strong>Terminology: </strong>

<table width="620">

 <tbody>

  <tr>

   <td rowspan="2" width="224">string literalmethod parameter string concatenation escape sequence variable variable declaration variable initialization</td>

   <td width="224">assignment statement assignment operator constantbyte, short, int, long float, double char boolean</td>

   <td width="172">arithmetic operator operator precedenceincrement, decrement operators assignment conversion promotion casting delimiter</td>

  </tr>

  <tr>

   <td colspan="2" width="396">character literal</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<h1>Course Coding Standard Additions</h1>

<ul>

 <li>Follow the standards in the book when naming variables and constants.</li>

 <li><u>Class names</u> should begin with a capital letter, and <u>method names and variables</u> should start with a lower case. Both should use medial capitals (also called “camelCase”. Examples:</li>

</ul>

<em>FirstProgram, HelloWorld, main, numberPeople</em>, <em>xAxis</em>, <em>result, finalResult</em> o Local variables should be declared at the beginning of the method in which they are used.

<ul>

 <li>Constants should be in all caps with words separated by an underscore. In addition to the type, a constant must be declared as <em>static final </em>(e.g., static final int MAX_NUMBER).</li>

</ul>

Constants must be placed at the class level (e.g., before the first method in the class).

Examples: <em>MAX_NUMBER</em>, <em>BASELINE</em>, <em>TAX_RATE</em>

<ul>

 <li>Both variables and constants should have descriptive variable names. <strong>This convention is not enforced by Checkstyle; however, it will be graded by your Instructor/GTA in the projects. </strong>Example:</li>

</ul>

<strong>Good </strong>J<strong>:  </strong><strong>int</strong> numberJobs, numEmployees;

<strong>Bad </strong>L<strong>:  </strong><strong>int</strong> n, m; <strong> </strong>

<strong> </strong>

<strong>Goals:</strong>

By the end of this activity you should be able to do the following: Ø Get user input using the Scanner class

<ul>

 <li>Create variables and concatenate variables with a string</li>

 <li>Use arithmetic operators to manipulate <strong>integer</strong> and <strong>double</strong> data types</li>

 <li>Use a basic <em>if</em> statement to determine which output is appropriate</li>

 <li>Run your program in a viewer canvas , including creating and saving the canvas file</li>

</ul>




<strong>Program Description: </strong>

The goal of this activity is to create a program that displays someone’s name, age, and gender, along with calculations for age in minutes and centuries well as max heart rate based on age and gender.

<strong> </strong>

<strong>Directions:  <u>After you enter each segment of code below, be sure to compile and/or run</u> <u>your program.  You should correct any errors prior to entering additional code</u>.   </strong>

<h1>Part 1: Getting user’s name and age</h1>

<ul>

 <li>Create the following class in jGRASP and <strong>save it as AgeStatistics.java </strong>as soon as you have entered the skeleton code for the class<strong>.</strong></li>

</ul>




<ul>

 <li>Add Javadoc comments for the class and main method.</li>

</ul>




<ul>

 <li>Declare the following variables in the main method then compile your program:</li>

 <li><strong>Add lines to prompt for and input the user’s gender after the previous code. Make sure that your program has the EXACT output as below. </strong></li>

</ul>

<strong> </strong>

—-jGRASP exec: java -ea AgeStatistics

Enter your name: Pat

Enter your age in years: 71

Enter your gender (1 for female and 0 for male): 1




—-jGRASP: operation complete.







<h1>Part 2: Converting age</h1>

<ul>

 <li>First, calculate and print the age of the user in minutes (minutes = years * 525600). Note that the tab escape sequence is included in the print statement; tab character is set to three spaces in jGRASP.</li>

</ul>




<ul>

 <li>Now calculate the age in centuries. <u>You should be familiar with type conversion between</u> <u>numeric types</u>.</li>

</ul>










—-jGRASP exec: java -ea AgeStatistics

Enter your name: Pat

Enter your age in years: 71

Enter your gender (1 for female and 0 for male): 1

Your age in minutes is 37317600 minutes.

Your age in centuries is 0.71 centuries.




—-jGRASP: operation complete.




<strong> </strong>

<h1>Part 3: Max heart rate prompt</h1>

<ul>

 <li>Add the code to print max heart rate (note the print rather than println):</li>

</ul>




<ul>

 <li>Add an <em>if-else</em> statement that will be used to assign maxHeartRate to the max heart rate calculation for male and female. <u>The comments below are there to help you in the Part 4</u></li>

</ul>

<u>where you will insert the code to do the calculations on the line after each comment.</u>




<ul>

 <li>Add one more print statement to print the max heart rate:</li>

</ul>




<h1>Part 4: Max heart rate calculations</h1>




<ul>

 <li>On your own, complete the <em>if-else</em> statement by adding an <u>assignment statement</u> for female and another for male to assign the appropriate expression below to the variable maxHeartRate.</li>

</ul>




The maximum heart rate is calculated as follows:

<ul>

 <li>Max heart rate for females:</li>

</ul>

209 – (0.7 * ageInYears)




<ul>

 <li>Max heart rate for males:</li>

</ul>

214 – (0.8 * ageInYears)




Test your program and make sure that the output is exactly as shown below. Your lab instructor may ask you to use a different set of values to test your program when you demo it for your activity grade.




Output # 1:

—-jGRASP exec: java -ea AgeStatistics

Enter your name: Lucy

Enter your age in years: 25

Enter your gender (1 for female and 0 for male): 1

Your age in minutes is 13140000 minutes.

Your age in centuries is 0.25 centuries.

Your max heart rate is 191.5 beats per minute.




—-jGRASP: operation complete.







Output # 2:

—-jGRASP exec: java -ea AgeStatistics

Enter your name: Kao

Enter your age in years: 19

Enter your gender (1 for female and 0 for male): 0

Your age in minutes is 9986400 minutes.

Your age in centuries is 0.19 centuries.

Your max heart rate is 198.8 beats per minute.




—-jGRASP: operation complete.













<strong>Web-CAT</strong> – After you have completed Part 4, you should submit your AgeStatistics.java file to Web-CAT.  This is the only file you will submit for this activity.

<h1>Part 5: Using the jGRASP Viewer Canvas</h1>

<strong> </strong>

In this part, you will run AgeStatistics.java in a <strong><em>viewer canvas</em></strong>.  In the process, you will create visualization of your program that can provide insight into what exactly happens when the program executes (runs).  Although AgeStatistics.java is a simple program, this exercise is intended to introduce you to viewer canvas so that you’ll know how to use it when you need to debug more complicated programs.  For more information on using the canvas see Section 2.10 in <em>Getting Started with jGRASP 2.0</em> (Shift-click to open the link in separate browser window).                <u>http://www.jgrasp.org/tutorials200/jGRASP_02_Getting_Started.pdf</u>




<ul>

 <li>With AgeStatistics.java in the CSD edit window, click the Run in Canvas button on the toolbar.  You should see an empty viewer canvas window as shown below.  In the CSD window, you should see that the program is stopped at the first executable statement:</li>

</ul>

Scanner userInput = new Scanner(System.in);




<ul>

 <li>As indicated by the message in the canvas, click the debug step button to execute the statement to create a Scanner object on System.in which is the keyboard. You should now see the variable name userInput in the Debug tab.  Now select and drag userInput from the Debug tab onto the canvas (i.e., left-click the mouse on userInput and hold as you drag it onto the canvas).   You should now see a viewer for userInput in the canvas.</li>

</ul>

This will show the stream of characters coming in from the keyboard after you press ENTER.




<ul>

 <li><u>four</u> more times so that you see name, ageInYears,</li>

</ul>

gender, and maxHeartRate in the Debug tab.  Now drag each of these variables into the

canvas window and arrange them as shown in the figure below.  Click the Save button  on the canvas toolbar.  You have now constructed and saved your first canvas.







<ul>

 <li>To complete the <em>run in canvas</em>, you can continue to click the step button and enter the required input (name, ageInYears, etc.), or alternatively, since the canvas has all the viewers we need, you can click the play button  (which means auto step-in) on the canvas.  After the <em>run in canvas</em> ends, close the canvas window.  Now click the <em>run in canvas</em> button   on the toolbar as you did in the first step above.  Your saved canvas file should open in the canvas window.  Click the play button , and your program will begin auto-stepping until is pauses waiting for input.  After you enter the requested input each time, the viewers on canvas will be updated.  The <em>run in canvas</em> will continue until your program terminates at which time the viewers on the canvas will display their last values as shown in the example below.  Note that the Scanner userInput indicates that “18” was entered followed by a press of the Enter key (which produces the escape characters <strong>r
</strong> on Windows or <strong>
</strong> on Mac OS X or Linux), then “1” was entered followed by a press of the Enter key.  The green arrowhead indicates that the “1” has been read but not the escape character(s)<strong> r
</strong> or <strong>
</strong>.</li>

</ul>


