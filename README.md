# Calculator-using-QT-Widgets

I followed a tutorial explaining how QT widgets work and the basics of building a calculator GUI. All of my programming before attempting this calculator program
had been run through the terminal. This was the first time I attempted to build frontend code and connecting it to backened code. 

The tutorial had missing functions that challenged me to write my own code to complete the calculator. I coded the MemAddClearGet() function as well 
as the Clear() function. I connected those to the GUI using the steps that the tutorial instructed for previous functions.

The tutorial had two flaws: the calculator app was made using an older version of QT and the coder of the original project had used global variables in the project.
I first addressed the global variables. They all had a simple fix which was instead of listing it at the top of the cpp file, they needed to be added as private members
the class. 

The second flaw was that QT removed support for QRegExp in the newest version of the program which the tutorial relied heavily on. I found that QT5's QRegExp was no longer supported. instead I had to implement QT6's QRegularExpression function which had a completely different list of implemenatations. Through trial and error, I was able to replace any instance of QRegExp into QRegularExpression. Specifically, I altered the code so that the ChangeNumberSign() function worked as intended. 
