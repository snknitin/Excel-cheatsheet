# Excel-cheatsheet
This is a repository that documents all the tricks and tips I have come across when using Excel.

* Selecting the cell and dragging the small square at the bottom right corner will help autofill the pattern. Even works for names of months and weeks
* Anytime you make a formula it will make **relative references** if you copy and paste that cell. Relative to where that formula is, it will operate on those corresponding cells. This works if all the terms are in the same column and you copy the function to different columns.
* Use **$** to make an **absolute refernce** to a particular cell tat may not be part of the column you are operating on
* Reference a range using **:**, for example G4:G8 for a column and G4:L8 to reference a matrix selection
* Use **format painter**,(below the cut and copy options),which enables you to select the format of a cell that you like and then apply it to other cells you click
* If you see a series of '#' signs in excel like this, ##############, that means there are numbers in that column and the column needs to be expanded in order to see those numbers. It isn't wide enough. Double click to make it fit perfectly


## Formula

* All formulae start with **=**
* If you want to type the formula and siplay it, use a single quote before the = to print the whole formula in that cell(kind of like an escape character)
* Order of operations : Parentheses, Exponents, Multiplication, Division, Addition, Subtraction

