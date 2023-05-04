Download Link: https://assignmentchef.com/product/solved-csci360-assignment-5-multiplication-and-division
<br>
Write an Assembler program to calculate payroll for a business.  Each employee has an hourly pay rate, a number of hours worked in the pay period, a deduction amount for any lunches eaten in the company cafeteria during the pay period, and, if earned, a bonus amount.  Of course, each employee has a name and employee identification number.




To begin this assignment, you can use TSO/ISPF option 3.3 to copy a previous assignment member in your

Partitioned Data Set Extended (PDSE) and name the new copied member .  If you do this, be sure to change     in the source code wherever necessary.




<h1>Input</h1>




The first input record has a single integer representing the current tax withholding percentage.  Read that record and get the percentage into a register to use in arithmetic in the body of the loop.




Each of the rest of the input record contains, from left to right across the 80-byte record, the following data about a single employee:  employee name, employee id number, hourly pay rate, number of hours worked in the pay period, deduction amount, and bonus amount, with the three dollar amounts rounded to the whole dollar.  Remember to use MVC to move character data (even thought it is numeric, you may consider the employee id number character data – people do not do arithmetic with ID numbers…usually).




<h1>Calculations</h1>




Your program must calculate each employee’s gross pay amount using the following formula:







And then calculate each employee’s net pay amount using the following formula:







Your program also must count the number of employees processed and keep a running total of each of the  deduction, bonus, gross pay amount, withholding amount and net pay amount.




Finally, after the loop ends, your program must calculate the average gross pay and net pay amount for the employees listed.  Use the following formulas:







Note:  When doing division, disregard the remainder and use only the quotient of the division.  Working with decimal points will be included in a future assignment.




Be VERY smart about your register usage.  For example, after you get the gross pay calculated and added to the total gross pay amount register, you can reuse the registers that were used to hold hourly pay rate, number of hours worked, deduction amount and bonus amount (of course, you also need to have

those values into the print line and have added the deduction and bonus amount registers to their total registers too).




<h1>Output</h1>




For each record, print out (using ) the employee’s name, employee id number, hourly pay rate, number of hours worked, deduction amount, bonus amount, gross pay amount, withholding amount and, finally, net pay amount, that you calculated across one output line, double spaced.




At the end of the report, and on separate lines and on the left, just under the employee’s ID, print out the number of employees processed, the total deduction amount, total bonus amount, total gross pay, total withholding amount and total net pay amount.  And finally, on a fifth line, print out the average gross pay amount and average net pay amount.  Be sure that you double space all of the output lines.




For guidance, see the exact output document named:







The data above can be accessed by copying or typing in the following into your  PDSE member replacing what is there from your previous assignment’s PDSE member:

<strong> </strong>