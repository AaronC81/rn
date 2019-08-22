# rn
## Overview
rn is an **organised dumping ground for quick experiments.**

Be honest - how many files with names like `test-something` do you have 
scattered around your user directory? rn offers an instant way of creating
these folders, with a single short command, out of the way of all of your
other files.

Everything gets put into directories in `~/.rn`. If something becomes important,
move it out of there!

## Usage
You don't need to give a name:
```
aaron:~$ rn
Created: ~/.rn/2019-08-22-1438/
aaron:~/.rn/2019-08-22-1438$
```

...but you can give a name if you like:
```
aaron:~$ rn my first test
Created: ~/.rn/2019-08-22-1438-my-first-test/
aaron:~/.rn/2019-08-22-1438-my-first-test$
```

You can even specify a command you'd like to run immediately. For example, to
create a new directory and then run `code .` inside it, you can make `+code` the
first argument:
```
aaron:~$ rn +code ide test 
Created: ~/.rn/2019-08-22-1438-ide-code/
Running: code .
aaron:~/.rn/2019-08-22-1438-ide-code$ # VS Code is now open in the directory
```

## Installation
rn is a bash function. Either source it in your `~/.bashrc`, or just copy-paste
it in.