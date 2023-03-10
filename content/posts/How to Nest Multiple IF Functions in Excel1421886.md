---
title: "You Won't Believe How Easy It Is To Nest Multiple If Functions In Excel - Click Here To Learn The Secret!"
ShowToc: true 
date: "2023-04-29"
author: "Mark Scott"
---
*****
title: You Won't Believe How Easy It Is To Nest Multiple If Functions In Excel - Click Here To Learn The Secret!

If you are an Excel user, you must know how important IF functions are. They are the backbone of Excel formulas and are used to execute certain actions based on a set of logical conditions. However, sometimes, you may need to apply multiple IF functions to arrive at the desired result. That's where nesting comes into play.

Nesting refers to the process of placing one function inside another. In Excel, you can create complex formulas by nesting multiple IF functions together. This allows you to perform calculations based on multiple conditions and create more advanced formulas.

The syntax of the IF function is as follows:

=IF(logical_test, value_if_true, value_if_false)

Here, logical_test refers to the condition you want to test, and value_if_true and value_if_false are the values you want to return if the condition is true or false, respectively.

To nest multiple IF functions, you use the IF function as a value_if_true or value_if_false argument of another IF function. Let's see an example to understand this better.

Suppose you have a worksheet that contains a list of students and their grades. You want to assign letter grades to the students based on their percentage score. Here's how you can do it using nested IF functions.

=IF(B2>=90,"A",IF(B2>=80,"B",IF(B2>=70,"C",IF(B2>=60,"D","F"))))

In this formula, the logical_test argument checks whether the percentage score in cell B2 is greater than or equal to 90. If it is, the value_if_true argument returns "A." If not, the second IF function is evaluated, and so on.

By nesting multiple IF functions in this way, you can create complex formulas that evaluate multiple conditions and return the appropriate values based on the results.

Nesting multiple IF functions can be a great way to simplify complicated formulas and make them more efficient. However, it's essential to use this technique judiciously and only when necessary. Large formulas can be difficult to read and understand, so it's important to keep them as concise as possible.

In conclusion, nesting multiple IF functions is a powerful technique that can help you create more advanced formulas in Excel. By using this technique, you can evaluate multiple conditions and perform complex calculations with ease. So why not give it a try and see how it can help you improve your Excel skills?

{{< youtube KkTaQ5OjAGc >}} 




This article explains how to nest IF functions in Excel to increase the conditions tested for and the actions performed by the function. Instructions cover Excel 2019-10, Excel for Mac, and Excel Online.

 
### 
What to Know
 
- =IF(D7<30000,$D$3*D7,IF(D7>=50000,$D$5*D7,$D$4*D7))= is the formula you enter to start the Nested IF function.Enter the Logical_test argument, which compares two items of data, then enter the Value_if_true argument.Enter the Nested IF Function as the Value_if_false Argument. To finish, copy the Nested IF functions using the Fill Handle.

 
##   Nest IF Functions Tutorial  
 

As shown in the image, this tutorial uses two IF functions to create a formula that calculates an annual deduction amount for employees based on their yearly salary. The formula used in the example is shown below. The nested IF function acts as the value_if_false argument for the first IF function.

 

=IF(D7<30000,$D$3*D7,IF(D7>=50000,$D$5*D7,$D$4*D7))

 

The different parts of the formula are separated by commas and carry out the following tasks:

 
- The first part, D7<30000, checks to see if an employee's salary is less than $30,000.If the salary is less than $30,000, the middle part, $D$3*D7, multiplies the salary by the deduction rate of 6%.If the salary is greater than $30,000, the second IF function IF(D7>=50000,$D$5*D7,$D$4*D7) tests two further conditions.D7>=50000 checks to see if an employee's salary is greater than or equal to $50,000.If the salary is equal to or greater than $50,000, $D$5*D7 multiplies the salary by the deduction rate of 10%.If ​the salary is less than $50,000 but greater than $30,000, $D$4*D7 multiplies the salary by the deduction rate of 8%.

 
##   Enter the Tutorial Data  
 

Enter the data into cells C1 to E6 of an Excel worksheet as seen in the image. The only data not entered at this point is the IF function itself located in cell E7.

 

 

 
The instructions for copying the data do not include formatting steps for the worksheet. This doesn't interfere with completing the tutorial. Your worksheet may look different than the example shown, but the IF function will give you the same results.
 
##   Start the Nested IF Function  
 

It is possible to just enter the complete formula

 

into cell E7 of the worksheet and have it work. In Excel Online, this is the method you must use. However, if you are using a desktop version of Excel, it is often easier to use the function's dialog box to enter the necessary arguments.

 

Using the dialog box is a bit trickier when entering nested functions because the nested function must be typed in. A second dialog box cannot be opened to enter the second set of arguments.

 

In this example, the nested IF function is entered into the third line of the dialog box as the Value_if_false argument. Since the worksheet calculates the annual deduction for several employees, the formula is first entered into cell E7 using absolute cell references for the deduction rates and then copied to cells E8:E11.

 
##   Tutorial Steps  
 
- Select cell E7 to make it the active cell. This is where the nested IF formula will be located.Select Formulas.Select Logical to open the function drop-down list.Select IF in the list to bring up the function's dialog box.

 

The data entered into the blank lines in the dialog box form the arguments of the IF function. These arguments tell the function the condition being tested and what actions to take if the condition is true or false.

 
##   Tutorial Shortcut Option  
 

To continue with this example, you may:

 
- Enter the arguments into the dialog box as shown in the image above and then jump to the final step that covers copying the formula to rows 7 through 10.Or, follow through the next steps that offer detailed instructions and explanations for entering the three arguments.

 
##   Enter the Logical_test argument  
 

The Logical_test argument compares two items of data. This data can be numbers, cell references, the results of formulas, or even text data. To compare two values, the Logical_test uses a comparison operator between the values.

 

In this example, there are three salary levels that determine an employee's annual deduction:

 
- Less than $30,000.Between $30,000 and $49,999.$50,000 or more

 

A single IF function can compare two levels, but the third salary level requires the use of the second nested IF function. The first comparison is between the employee's annual salary, located in cell D, with the threshold salary of $30,000. Since the goal is to determine if D7 is less than $30,000, the Less Than operator ( < ) is used between the values.

 
- Select the Logical_test line in the dialog box.
 - Select cell D7 to add this cell reference to the Logical_test line.
 - Press the less-than key ( < ) on the keyboard.
 - Type 30000 after the less-than symbol.
 - The completed logical test displays as D7<30000.

 
Do not enter the dollar sign ( $ ) or a comma separator ( , ) with the 30000. An invalid error message appears at the end of the Logical_test line if either of these symbols is entered along with the data.
 
##   Enter the Value_if_true Argument  
 

The Value_if_true argument tells the IF function what to do when the Logical_test is true. The Value_if_true argument can be a formula, a block of text, a value, a cell reference, or the cell can be left blank.

 

In this example, when the data in cell D7 is less than $30,000, Excel multiplies the employee's annual salary in cell D7 by the deduction rate of 6 percent located in cell D3.

 
##   Relative vs. Absolute Cell References  
 

Normally, when a formula is copied to other cells, the relative cell references in the formula change to reflect the formula's new location. This makes it easy to use the same formula in multiple locations. Occasionally, having cell references change when a function is copied results in errors. To prevent these errors, the cell references can be made Absolute, which stops them from changing when they are copied.

 

Absolute cell references are created by adding dollar signs around a regular cell reference, such as $D$3. Adding the dollar signs is easily done by pressing the F4 key on the keyboard after the cell reference has been entered into the dialog box.

 

In the example, the deduction rate located in cell D3 is entered as an absolute cell reference into the Value_if_true line of the dialog box.

 
- Select the Value_if_true line in the dialog box.Select cell D3 in the worksheet to add this cell reference to the Value_if_true line.Press the F4 key to make D3 an absolute cell reference ($D$3).Press the asterisk ( * ) key. The asterisk is the multiplication symbol in Excel.Select cell D7 to add this cell reference to the Value_if_true line.The completed Value_if_true line displays as $D$3*D7.

 
D7 is not entered as an absolute cell reference. It needs to change when the formula is copied to cells E8:E11 in order to get the correct deduction amount for each employee.
 
##   Enter the Nested IF Function as the Value_if_false Argument  
 

Normally, the Value_if_false argument tells the IF function what to do when the Logical_test is false. In this case, the nested IF function is entered as this argument. By doing so, the following results occur:

 
- The Logical_test argument in the nested IF function (D7>=50000) tests all salaries that are not less than $30,000.For those salaries greater than or equal to $50,000, the Value_if_true argument multiplies them by the deduction rate of 10% located in cell D5.For the remaining salaries (those that are greater than $30,000 but less than $50,000) the Value_if_false argument multiplies them by the deduction rate of 8% located in cell D4.

 

As mentioned at the beginning of the tutorial, a second dialog box cannot be opened to enter the nested function so it must be typed into the Value_if_false line.

 
- Select the  Value_if_false line in the dialog box.
 - Enter the following IF function:IF(D7>=50000,$D$5*D7,$D$4*D7)
 - Select OK to complete the IF function and close the dialog box.
 - The value of $3,678.96 appears in cell E7. Since R. Holt earns more than $30,000 but less than $50,000 per year, the formula $45,987 * 8% is used to calculate his annual deduction.
 - Select cell E7 to display the complete function =IF(D7=50000,$D$5*D7,$D$4*D7)) in the formula bar above the worksheet.

 

After following these steps, your example now matches the first image in this article.

 
Nested functions do not start with an equal sign, but rather with the function's name.
 
IF(D7>=50000,$D$5*D7,$D$4*D7)
 

The last step involves copying the IF formula to cells E8 to E11 using the ​fill handle to complete the worksheet.

 
##   Copy the Nested IF Functions Using the Fill Handle  
 

To complete the worksheet, copy the formula containing the nested IF function to cells E8 to E11. As the function is copied, Excel updates the relative cell references to reflect the function's new location while keeping the absolute cell reference the same.

 

One easy way to copy formulas in Excel is with the Fill Handle.

 
- Select cell E7 to make it the active cell.
 - Place the mouse pointer over the square in the bottom right corner of the active cell. The pointer will change to a plus sign (+).
 - Select and drag the fill handle down to cell E11.
 - Cells E8 to E11 are filled with the results of the formula as shown in the image above.

 

Get the Latest Tech News Delivered Every Day




