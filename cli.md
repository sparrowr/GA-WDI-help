*preface and disclaimers*

this is a rudimentary Unix CLI cheatsheet for people new to the command line.
Sparrow Rubin wrote it in March 2018, for macOS and Linux.
this is MIT licensed, and stored [in this github repo](https://github.com/sparrowr/GA-WDI-help/).
commands are in `back ticks`, things like $THIS are placeholders. I used [this Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to format this document, so it should be easy to read in Atom and on github.

*navigation*

`pwd` prints the working directory (shows which folder you're in)

`ls` shows contents of the working directory

`ls -a` shows everything in the working directory, including hidden files

`ls -l` shows everything with permissions and last modified times

`ls -G` shows everything in the working directory, color-coded

`cd $PATH` moves from current location to $PATH if it exists

`echo $WORDS` prints $WORDS the terminal (useful for confirming you can run commands here)

special directories: ~ is home, / is root, . is this directory, .. is up

*escaping/stopping*

ctrl+c to cancel or escape from almost anything

:wq! to escape from vi or vim if you accidentally open one of those

*help*

`man $COMMAND` will give you the manual page for $things if it exists

`$COMMAND --help` will sometimes give you a more concise explanation of $COMMAND

`whatis $COMMAND` will sometimes tell you what $COMMAND is

*creating, moving, destroying*

`mkdir $DIR` creates a new directory called $DIR in your working directory

`touch $FILE` creates a file called $FILE in your working directory, or updates that file if it exists

`mv $A $B` copies everything in $A to $B and gets rid of $B

`cp $A $B` copies everything in $A to $B

`rm $X` permanently destroys $X if it's a file, asking for confirmation

`rm -rf $X` permanently destroys $X and everything in $X without asking for confirmation

*interacting with contents of files*

`cat $FILE` prints everything in $FILE to the terminal

` | ` (called "pipe") redirects the output of one command to the input of another command

`grep $WORD $FILE` searches for $WORD in $FILE

`head` shows the beginning of a file

`tail` shows the end of a file

*examples*

`cat ~/.bash_history | tail` prints last ten commands you ran

`grep "id" index.html` shows all instances of "id" in index.html

`ls -alG ~` shows everything in your home directory, with details, color-coded
