# sudoko-js

a draft - plain html and pure javascript implementation of sudoko resolver.

there are two implemenations as of now

- recursive - with a blocking user interface, but it logs to the browser console (open javascript tools of your browser to see). it will solve most sudoko's (normal difficult) within a few seconds - using javascript - not too bad :-)
- stack based - (instead of recursion) and with an interactive loop where the board is painted on a regular base as html. this one much slower then the recursive one since it runs in the browser loop. you can see the stack operations and follow the search path also in the console log of your browser.


# how it works

the program calculates a search path for each cell based of the possible values and the given constraints (each number unique in a row, column and block) and crosses them out if no solution is found in the line of search.

the recursive implementation shows how the idea behind is.

the stack based implementation is more complex and therefore more a piece of fun stuff. anyway it shows that recursion is not always needed to solve a problem ;-)


# how to use

enter the sudoko in the textfield and press import. after that press 'recursive and blocking' or 'run interactive' button to start processing.
after a sudoko is imported use the mouse and hover the cells then the title will show the cell coordinates and the constrain dependencies. by clicking on a single cell the possible values are shown below the board.


# sudoko input format

the import eliminates all data from the textfield matching not one of 0-9 or '.' (period, what is replaced by 0). you can enter as single line or multiple lines. blank lines are also removed. the value 0 or '.' is used for an empty cell in the grid and the numbers 1-9 represent a given predefined value.


# view the sample

[open sudoko-js in your browser](https://kr-g.github.io/sudoko-js/)


# read the full article

https://another-software-development-blog.blogspot.com/2018/12/sudoko-re-solver-in-javascript.html


