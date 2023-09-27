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

# Github on the command line

> On your github account, create a github repo named "Only alkanes"

> Clone the newly created repo to your local machine
`git clone git@github.com:mikemugo/Onlyalkanes.git`

> Copy the contents of alkanes folder from shell-lesson-data/exercise-data/, used in previous classes, into your "Only alkanes" repo  
`cp -r data/ ../../../Onlyalkanes/`

> Run the following command while inside the repo `for j in `ls *.pdb`; do for k in {1..100}; do cp $j $(basename -s .pdb $j)$k.pdb; done; done`

> Find the easiest way to push only the .pdb files whose number suffix is divisible by 10
`git add *0.pdb;git commit -m "first pdb commit"`
`git push`

> Document your answer/work-around for the task number 5 in a markdown file named "Easiest solution.md"
