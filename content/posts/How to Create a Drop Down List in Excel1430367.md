---
title: "Revolutionize Your Excel Skills with this Insanely Simple Drop Down List Trick!"
ShowToc: true 
date: "2022-12-07"
author: "Elizabeth Macpherson"
---
*****
Revolutionize Your Excel Skills with this Insanely Simple Drop Down List Trick!

Do you struggle with keeping your Excel spreadsheets organized and streamlined? Have you ever found yourself wondering if there is a more efficient way to input data and reduce errors within your workbook? Look no further than the drop-down list trick! 

What is a drop-down list? It is a data validation tool that allows the user to select options from a pre-defined list, reducing the likelihood of incorrect data entry. By utilizing a drop-down list, you can streamline your data input process, reduce errors, and save time.

So how do you create a drop-down list in Excel? It's actually quite simple! Follow these steps:

Step 1: Create a list of options in a separate column or row within your workbook. This can be anything from a list of employees to different products or services.

Step 2: Highlight the cells where you want the drop-down list to appear.

Step 3: Click on "Data" in the Excel ribbon and select "Data Validation."

Step 4: In the "Settings" tab, select "List" as the validation criteria and input the range of cells containing the list of options from step 1.

Step 5: Select "OK." Your drop-down list should now be visible in the selected cells.

And that's it! With just a few clicks, you can easily create a drop-down list in Excel, making your data input process much more efficient and accurate. 

But the benefits of using drop-down lists don't stop there. Here are a few additional advantages:

1. Consistency: By using a pre-defined list of options, you can ensure consistency within your workbook. This is particularly useful when working with multiple users or when trying to maintain a specific standard.

2. Error-Reduction: With a drop-down list, there is less room for error as the user can only select from the pre-defined options. This means fewer mistakes and less time spent correcting them.

3. Time-Saving: Inputting data via a drop-down list is much faster than typing out each option manually. This means you can complete your work more quickly and move onto other tasks.

Overall, the drop-down list trick is a simple yet effective way to revolutionize your Excel skills. By using this tool, you can improve the accuracy, consistency, and efficiency of your data input process. So why not give it a try and see the impact it can make on your work?

{{< youtube qGmgX27D1qM >}} 




This article explains how to create a drop-down list in Excel. It includes information on using a list for data validation options, for protecting a drop-down list, and for making changes to a drop-down list. The instructions apply to Excel 2019, 2016, 2013, 2010, and Excel for Microsoft 365.

 
### 
What to Know
 
- Open two blank Excel workbooks named data-source.xlsx and drop-down-list.xlsx.Enter the options for the drop-down list in the source document. Enter the topic the list applies to in the drop-down list document.Create two named ranges—one for the list items and one in the workbook where the list is—to link them.

 
##   Entering the Data to Create a Drop-Down List  
 

When you add a drop-down list to a cell in Excel, an arrow appears next to it. Clicking on the arrow opens the list so you can select one of the items to enter into the cell. For example, if you're using a spreadsheet to track RSVPs for an event, you could filter that column by Yes, No, and Not Yet Replied.

 

The data used in the list can be located on the same sheet as the list, on a different sheet in the same workbook, or in a different workbook. In this example, the drop-down uses a list of entries located in a different workbook. The advantages of this method include centralizing list data for multiple users and protecting it from accidental or intentional change.

 
- Open two blank Excel workbooks.
 - Save one workbook with the name data-source.xlsx. This workbook will contain the data for the drop-down list.
 - Save the second workbook with the name drop-down-list.xlsx. This workbook will contain the drop-down list.
 - Leave both workbooks open after saving.
 - Enter the data as shown below into cells A1 to A4 of the data-source.xlsx workbook as seen in this image.
 - Save the workbook and leave it open.
 - Enter the data as shown in the image into cell B1 of the drop-down-list.xlsx workbook.
 - Save the workbook and leave it open.

 
###   Data for Cells A1 to A4 in data-source.xlsx  
 
- A1 — GingerbreadA2 — LemonA3 — Oatmeal RaisinA4 — Chocolate Chip

 
###   Data for Cell B1 in drop-down-list.xlsx  
 
- B1 — Cookie Type:

 
##   Creating Two Named Ranges  
 

A named range allows you to refer to a specific range of cells in an Excel workbook. Named ranges have many uses in Excel including in formulas and when creating charts. In all cases, you must use a named range instead of a range of cell references indicating the location of data in a worksheet.

 

Open two blank Excel workbooks.

 

Save one workbook with the name data-source.xlsx. This workbook will contain the data for the drop-down list.

 

Save the second workbook with the name drop-down-list.xlsx. This workbook will contain the drop-down list.

 

Leave both workbooks open after saving.

 

Enter the data as shown below into cells A1 to A4 of the data-source.xlsx workbook as seen in this image.

 

Save the workbook and leave it open.

 

Enter the data as shown in the image into cell B1 of the drop-down-list.xlsx workbook.

 
When the list data is in a separate workbook both must be open for the list to update.
 

When using a drop-down list from another workbook, you need to use two named ranges. One is for the list items and the second is in the workbook where the drop-down list is — this named range links to the one in the first workbook.

 
###   The First Named Range  
 
- Select cells A1 to A4 of the data-source.xlsx workbook to highlight them.
 - Click on the Name Box located above column A.
 - Type Cookies in the Name Box.
 - Press the Enter key on the keyboard.
 - Cells A1 to A4 of the data-source.xlsx workbook now have the range name of Cookies.
 - Save the workbook.

 
###   The Second Named Range  
 

The second named range does not use cell references from the drop-down-list.xlsx workbook. Instead, it links to the Cookies range name in the data-source.xlsx workbook, which is necessary because Excel will not accept cell references from a different workbook for a named range. It will, however, except another range name.

 

Select cells A1 to A4 of the data-source.xlsx workbook to highlight them.

 

Click on the Name Box located above column A.

 

Type Cookies in the Name Box.

 

Press the Enter key on the keyboard.

 

Cells A1 to A4 of the data-source.xlsx workbook now have the range name of Cookies.

 

Save the workbook.

 

Creating the second named range, therefore, is not done using the Name Box but by using the Define Name option located on the Formulas tab of the ribbon.

 
- Click on cell C1 in the drop-down-list.xlsx workbook.
 - Click on Formulas > Define Name on the ribbon to open the Define Name dialog box.
 - Click on the New button to open the New Name dialog box.
 - Type Data in the Name line.
 - In the Refers to line type ='data-source.xlsx'!Cookies
 - Click OK to complete the named range and return to the Define Name dialog box.
 - Click Close to close the Define Name dialog box.
 - Save the workbook.

 
##   Using a List for Data Validation  
 

All data validation options in Excel, including drop-down lists, are set using the data validation dialog box. In addition to adding drop-down lists to a worksheet, data validation in Excel can also be used to control or limit the type of data that users can enter into specific cells in a worksheet.

 

Click on cell C1 in the drop-down-list.xlsx workbook.

 

Click on Formulas > Define Name on the ribbon to open the Define Name dialog box.

 

Click on the New button to open the New Name dialog box.

 

Type Data in the Name line.

 

In the Refers to line type ='data-source.xlsx'!Cookies

 

Click OK to complete the named range and return to the Define Name dialog box.

 

Click Close to close the Define Name dialog box.

 

Save the workbook.

 
- Click on cell C1 of the drop-down-list.xlsx workbook to make it the active cell — this is where the drop-down list will be.
 - Click on the Data tab of the ribbon menu above the worksheet.
 - Click on the Data Validation icon on the ribbon to open the drop-down menu. Select the Data Validation option.
 - Click on the Settings tab in the Data Validation dialog box.
 - Click on the down arrow at the end of the Allow line to open the drop-down menu.
 - Click on List to choose a drop-down list for data validation in cell C1 and to activate the Source line in the dialog box.
 - Since the data source for the drop-down list is in a different workbook, the second named range goes in the Source line in the dialog box.
 - Click on the Source line.
 - Type =Data in the Source line.
 - Click OK to complete the drop-down list and close the Data Validation dialog box.
 - A small down arrow icon should appear on the right side of cell C1. Clicking on the down arrow will open the drop-down list containing the four cookie names entered into cells A1 to A4 of the data-source.xlsx workbook.
 - Clicking on one of the names in the drop-down list should enter that name into cell C1.

 
##   Changing the Drop-Down List  
 

Since this example used a named range as the source for our list items rather than the actual list names, changing the cookie names in the named range in cells A1 to A4 of the data-source.xlsx workbook immediately changes the names in the drop-down list.

 

Click on cell C1 of the drop-down-list.xlsx workbook to make it the active cell — this is where the drop-down list will be.

 

Click on the Data tab of the ribbon menu above the worksheet.

 

Click on the Data Validation icon on the ribbon to open the drop-down menu. Select the Data Validation option.

 

Click on the Settings tab in the Data Validation dialog box.

 

Click on the down arrow at the end of the Allow line to open the drop-down menu.

 

Click on List to choose a drop-down list for data validation in cell C1 and to activate the Source line in the dialog box.

 

Since the data source for the drop-down list is in a different workbook, the second named range goes in the Source line in the dialog box.

 

Click on the Source line.

 

Type =Data in the Source line.

 

Click OK to complete the drop-down list and close the Data Validation dialog box.

 

A small down arrow icon should appear on the right side of cell C1. Clicking on the down arrow will open the drop-down list containing the four cookie names entered into cells A1 to A4 of the data-source.xlsx workbook.

 

Clicking on one of the names in the drop-down list should enter that name into cell C1.

 

Follow the steps below to change Lemon to Shortbread in the drop-down list by changing the data in cell A2 of the named range in the data-source.xlsx workbook.

 
If the data is entered directly into the dialog box, making changes to the list involves going back into the dialog box and editing the source line.
 
- Click on cell A2 in the data-source.xlsx workbook to make it the active cell.
 - Type Shortbread into cell A2 and press the Enter key on the keyboard.
 - Click on the down arrow for the drop-down list in cell C1 of the drop-down-list.xlsx workbook.
 - Item 2 in the list should now read Shortbread instead of Lemon.

 
##   Options for Protecting the Drop-Down List  
 

Since the data in this example is on a different worksheet than the drop-down list, the options available for protecting the list data include:

 

Click on cell A2 in the data-source.xlsx workbook to make it the active cell.

 

Type Shortbread into cell A2 and press the Enter key on the keyboard.

 

Click on the down arrow for the drop-down list in cell C1 of the drop-down-list.xlsx workbook.

 

Item 2 in the list should now read Shortbread instead of Lemon.

 
- Protecting the worksheet by locking cells A1 to A4 on sheet 2
 - Requiring a password to modify the workbook
 - Having the workbook open as Read-only

 

Get the Latest Tech News Delivered Every Day




