# Sed_command_assignment

## Assignment

Use the sed command in a for loop to remove the following lines in the file diary.html
- 1 to 221
- 265 to 330
Save the ouptput in a file called diary_no_header-no_footnote.txt

`for y in '1,221d;265,330d'; do sed $y diary.html > diary-nofoot.txt; done`
