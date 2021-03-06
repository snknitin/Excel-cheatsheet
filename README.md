# Excel-cheatsheet
This is a repository that documents all the tricks and tips I have come across when using Excel.

* Selecting the cell and dragging the small square at the bottom right corner will help autofill the pattern. Even works for names of months and weeks
* Anytime you make a formula it will make **relative references** if you copy and paste that cell. Relative to where that formula is, it will operate on those corresponding cells. This works if all the terms are in the same column and you copy the function to different columns.
* Use **$** to make an **absolute reference** to a particular cell tat may not be part of the column you are operating on
* Reference a range using **:**, for example G4:G8 for a column and G4:L8 to reference a matrix selection
* Use **format painter**,(below the cut and copy options),which enables you to select the format of a cell that you like and then apply it to other cells you click
* If you see a series of '#' signs in excel like this, ##############, that means there are numbers in that column and the column needs to be expanded in order to see those numbers. It isn't wide enough. Double click to make it fit perfectly
* **Conditional formating**. You can choose a different highlight or format of a cell based on value or other attributes
* If you have empty rows in your spreadsheet between 2 every rows, you can remove them by 
   * Creating Macros
   * sort the rows
   * filter blanks
* If you want to transpose the rows and columns, Copy the data, ad then paste it by selecting the transpose option 
* **Freeze Pane** option allow you to freeze the rows and columns to the left and above the selected row allowing you to scroll through the data horizontally or vertically without missing track fo what columsn or rows you are looking at, since those are frozen


## Formula

* All formulae start with **=**
* If you want to type the formula and siplay it, use a single quote before the = to print the whole formula in that cell(kind of like an escape character)
* Order of operations : Parentheses, Exponents, Multiplication, Division, Addition, Subtraction


## Functions

Unlike formula this isn't user defined. Rather it is predefined and already exists

* **VLOOKUP** - Provide ranges for the data and give it value or a grade. like 0-60% is F, 60-70 is D, 80-90 is A. You just need to have the lower limits and then the corresponding grades in the column beside it. Give this as the table array and lookup values of a particular column and return the value from column 2 in your table array which are the grades
* **=CONCATENATE($E$6," < ",$E$7)** - this gives us something like *75 < 100* in the cell
* **IF** - (Condition,value if true, value if false) . This is like the conditional operator in python with the (a<b)?a:b
* **IFERROR** - Dynamic amortization tables. returns a custom result when a formula generates an error, and a standard result when no error is detected. You can default it to leave empty cells. =IFERROR (value/function/formula, value_if_error)


## Charts(or Graphs)

[Dynamic visualization of GDP and life expectancy yearly](http://www.gapminder.org/world/)    
[Flight path mapped](http://www.aaronkoblin.com/)      

* You can select the headers along with the data and then chart it out to have the titles also written automatically
* Don't use the total or the sum amount while plotting. make sure you avoid it to not get an incorrect graph
* You can also have miniature small graphs for each row in the data as a separate column. These are called **spark lines**. You can also select high point or low point for it.
* You can also add a trend line to a scatter or line plot
* You can switch row and column data with most charts but maybe not with scatter plots
* You can create a chart and then copy values of another column and paste it onto the chart 


## Data Manipulation

* Get unique records from advance filter or use **Remove duplicates** and select which combination of columns to consider as unique indexes
* You can do a **multiple sequential sort criterias**(Like sort by first name, then sort by salary range) by sorting first with one column and then **Add level** and give other sorting criteria
* If there are blank columns in between your data columns then they might get considered as separate tables and rows won't be sorted together
* **Sub-totalling data** - You can sort by some criteria and then at each change in some category value, you can apply a function that operated on that group sorted above the next group of rows and have sub-totals. Helpful when you want to get some monthly or daily estimates, you can sort by month and based on every change in month get averages or sums


## Pivot tables and charts

* Might not update immediately if the soruce data changes.  
* It is possible to group items in pivot tables
* Slicers also data to be filtered in a more visual way. Choose **Insert slicer** and then selecting column will give you a slicer with all the unique values and you and view different selections by clicking
* You can also select a **Pivot Chart** and that also changes dynamically based on your selections 








