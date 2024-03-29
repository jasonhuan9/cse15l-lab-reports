# Lab 4

## Log into ieng6

Keys pressed: `<up><enter>`, the command I ran was `ssh jah053@ieng6.ucsd.edu`, the command was 1 up in the history, so I used the up arrow to access it.

![ssh ieng6](lab4_files/ssh.png)

## Cloning my fork of the repository 

Keys pressed: `git <space> clo <tab> <command>v <enter>`, the command I ran was `git clone git@github.com:jasonhuan9/lab7.git`, I copied the ssh url to my clipboard and pasted it after typing git clone.

![git clone](lab4_files/clone.png)

## Run the test, showing that they fail

Keys pressed: `cd <space> l <tab><enter>`, I ran `cd/lab7`. Then I pressed `bash <space> t <tab><enter>` to run `bash test.sh`.

![test fail](lab4_files/testfail.png)

## Fix the code

Keys pressed: `vim <space> L <tab> .j <tab><enter>`, to run `vim ListExamples.java` Then in vim, I pressed `43j e r2 :x` to change `index1` to `index2`.

![vim](lab4_files/vim.png)

![fix code](lab4_files/fixcode.png)


## Run the test, showing that they pass

Keys pressed: `<up><up><enter>`, to run `bash test.sh`, the command was 2 up in my history.

![test pass](lab4_files/testpass.png)

## Commit and push the changes to Github

Keys pressed: `git <space> add <space> -A <enter>`, running `git add -A` to add the files, then `git <space> com<tab> -m <space> fix <enter>`, to run `git commit -m fix`, to commit the changes with the message "fix", and then `git <space> push <enter>`, running `git push` to push the changes to Github.

![commit and push](lab4_files/commitandpush.png)
