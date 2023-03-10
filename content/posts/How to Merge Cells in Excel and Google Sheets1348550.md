---
title: "You've Been Merging Cells In Excel and Google Sheets The WRONG Way - Here's The Correct Method!"
ShowToc: true 
date: "2022-12-14"
author: "Pedro Eady"
---
*****
TITLE: You've Been Merging Cells In Excel and Google Sheets The WRONG Way - Here's The Correct Method!

Introduction:

Merging cells in Excel and Google Sheets can make your spreadsheet look organized and professional. However, if you use the wrong method, merging cells can cause more harm than good. In this article, we'll discuss the correct method of merging cells in Excel and Google Sheets, and why it matters.

Body:

The wrong way to merge cells in Excel and Google Sheets is by using the merge cells button in the toolbar. While this may seem like the logical way to merge cells, it can cause problems, especially when you're using formulas.

Let's say you have a worksheet with cells A1 to A10 and B1 to B10. You want to merge cells A1 to B1, so you highlight the cells and click the merge cells button. This will give you one cell covering cells A1 and B1. However, if you have any formulas referencing cells A1 or B1, the formulas will be deleted. This is because merge cells only keep the data in the top-left cell, deleting the rest.

This can be frustrating if you had important formulas and data you didn't want to be deleted. So, to avoid this problem, we need to use the correct method of merging cells.

The correct method is by using the "Center Across Selection" option. This option allows you to merge cells without deleting the data and formulas in the individual cells. Here's how to do it:

1. Highlight the cells you want to merge.
2. Right-click on the highlighted cells and select "Format Cells".
3. In the "Format Cells" dialog box, go to the "Alignment" tab.
4. Under the "Horizontal" dropdown, select "Center Across Selection".
5. Click "OK".

Now, you've merged the cells without deleting any data or formulas! The best part is that if you choose to unmerge the cells in the future, your data and formulas will remain intact.

Conclusion:

Merging cells in Excel and Google Sheets can make your spreadsheet look clean and organized. However, it's crucial to use the correct method of merging cells to avoid deleting important data and formulas. By using the "Center Across Selection" option, you can merge cells without losing any information. Remember to use this method the next time you need to merge cells!

{{< youtube XTWT8vGQIG0 >}} 




In Microsoft Excel and Google Sheets, a merged cell is a single cell that is created by combining or merging two or more individual cells. Both spreadsheets merge cells horizontally, vertically, or both.

 
##   How to Merge Cells in Microsoft Excel  
 

Excel offers one-click access to the merge tool. Highlight the cells you want to merge (the cells must be contiguous either horizontally or vertically), then go to the Home tab and select Merge & Center.

 
Instructions in this article apply to the current release of Google Sheets and all versions of Microsoft Excel since Excel 2010.
 

When you select Merge & Center, the selected cells are merged into one cell and content is centered in the upper-left cell across the merge. To change this behavior, select the Merge & Center drop-down arrow and select an alternative behavior:

 
- Merge Across: Merges the cells, but does not center the content across the cells. This only works on a row level. For example, if you select a block of four rows by four columns, this option results in four one-column rows.Merge Cells: Merges the cells into one large block. For example, if you select a block of four rows by four columns, this option results in a single block that's four rows high by four rows wide.Unmerge Cells: When you select a merged cell, this option unmerges the cells.

 

Although the Merge & Center function is most often used to consolidate row-level headers in reports, you can merge cells vertically, too — or even in rectangles. You cannot, however, merge non-contiguous cells.

 
##   How to Merge Cells In Google Sheets  
 

As with Microsoft Excel, Google Sheets also offers one-button access to its merge feature. Highlight the cells to be merged, go to the toolbar and select Merge (the icon looks like a square with arrows pointed inward).

 

The default behavior is to merge all cells. To find other merge types, select the Merge drop-down arrow:

 
- Merge All: This is the default behavior. Renders all the cells into a single block, regardless of how many rows and columns are within the range.Merge Horizontally: Merges the cells along the row axis. If you select more than one row, this option results in each row standing alone with the columns merged into one or more single-row cells.Merge Vertically: Merges the cells along the column axis. For example, if you select a six-row-by-six-column range, this option renders six merged cells, each of which is one column wide by six rows tall.Unmerge: Removes a merge on the affected cells.

 

Merges in Google Sheets preserve only the contents of the upper-left cell within the merged range. You can only merge cells in contiguous blocks.

 
If you lose data in a merge, use the undo feature in Microsoft Excel or Google Sheets. However, if you can't undo, un-merging the cells won't restore the data, because the data is discarded as part of the merge procedure.
 

Get the Latest Tech News Delivered Every Day




