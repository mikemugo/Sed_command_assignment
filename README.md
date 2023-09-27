# Sed_command_assignment

## Assignment

Use the sed command in a for loop to remove the following lines in the file diary.html
- 1 to 221
- 265 to 330
Save the ouptput in a file called diary_no_header-no_footnote.txt

`for y in '1,221d;265,330d'; do sed $y diary.html > diary-nofoot.txt; done`

# grep assignment

## Assignemnt

- Cd to the directory /exercise-data/writing
- Create a for loop that you will use on the LittleWomen.txt
- The loop should count the names "Jo" , "Meg", "Beth", "Amy"
- And prints the output on the screen

`for l in Jo Meg Beth Amy; do printf "$l "; cat LittleWomen.txt | grep $l | wc -l; done`
|Jo  |1528|
|----|----|
|Meg | 685|
|Beth| 463|
|Amy | 643|
