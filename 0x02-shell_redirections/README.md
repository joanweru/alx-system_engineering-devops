# Shell, I/O Redirection

In typical Unix installations, commands are entered at the keyboard. By default, your keyboard is the standard input, sometimes denoted as **stdin**. The output resulting from these commands is displayed on the computer screen. By default,your screen is the standard output, sometimes denoted as **stdout**. Unix provides the capability to change where standard input comes from, or where output goes using a concept called **Input/Output (I/O) redirection**. I/O redirection is accomplished using a redirection operator which allows the user to specify the input or output data be redirected to (or from) a file.

## Output Redirection

The output from a command, which normally goes to the display device can be redirected to a file by typing the command followed by `> filename`. The output of the command is written to the specified file name. The **>** symbol is known as the *output redirection operator*.


When the notation`>> filename` is added to the end of a command, the new results of the output of the command are added to the end of the file rather than overwriting the pre-existing data, thus making the file longer each time the command is repeated. The **>>** symbol is known as the *append redirection operator*.

## Input Redirection

When the notation `< filename` is added to the end of a command, the input of the command is read from the specified file name. The **<** symbol is known as the *input redirection operator*

## Pipelines
Pipelines connect multiple commands together. With pipelines, each command reads the previous command’s output.

`command1 | command2 | command`

## Filters

Filters are programs that take plain text(either stored in a file or produced by another program) as standard input, transforms it into a meaningful format, and then returns it as standard output.

### Tasks

This repo contains tasks for my 0x02. Shell, I/O Redirections and filters Project. The following are scripts in this repo and their uses.

* `0-hello_world` - prints “Hello, World”, followed by a new line to the standard output
* `1-confused_smiley` - displays a confused smiley "(Ôo)'
* `2-hellofile` - displays the content of the `/etc/passwd` file
* `3-twofiles` - displays the content of `/etc/passwd` and `/etc/hosts`
* `4-lastlines` - displays the last 10 lines of `/etc/passwd`
* `5-firstlines` - displays the first 10 lines of `/etc/passwd`
* `6-third_line` - displays the third line of the file `iacta`
* `7-file` - creates a file named exactly `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` containing the text Best School ending by a new line
* `8-cwd_state` - writes into the file `ls_cwd_content` the result of the command `ls -la`
* `9-duplicate_last_line` - duplicates the last line of the file `iacta`
* `10-no_more_js` - deletes all the regular files (not the directories) with a `.js` extension that are present in the current directory and all its subfolders
* `11-directories` - counts the number of directories and sub-directories in the current directory
    * The current and parent directories should not be taken into account
    * Hidden directories should be counted
* `12-newest_files` - displays the 10 newest files in the current directory
Requirements: 

    * One file per line
    * Sorted from the newest to the oldest 

* `13-unique` - takes a list of words as input and prints only words that appear exactly once

    * Input format: One line, one word
    * Output format: One line, one word
    * Words should be sorted

* `14-findthatword` - Display lines containing the pattern “root” from the file `/etc/passwd`
* `15-countthatword` - displays the number of lines that contain the pattern “bin” in the file `/etc/passwd`
* `16-whatsnext` - displays lines containing the pattern “root” and 3 lines after them in the file `/etc/passwd`
* `17-hidethisword` - displays all the lines in the file `/etc/passwd` that do not contain the pattern “bin”
* `18-letteronly` - displays all lines of the file `/etc/ssh/sshd_config` starting with a letter
* `19-AZ` - replaces all characters A and c from input to Z and e respectively
* `20-hiago` - creates a script that removes all letters c and C from input
* `21-reverse` - a script that reverse its input
* `22-users_and_homes` - displays all users and their home directories, sorted by users
* `100-empty_casks` - finds all empty files and directories in the current directory and all sub-directories

    * Only the names of the files and directories should be displayed (not the entire path)
    * Hidden files should be listed
    * One file name per line
    * The listing should end with a new line
    * You are not allowed to use `basename`, `grep`, `egrep`, `fgrep` or `rgrep`

* `101-gifs` -  lists all the files with a `.gif` extension in the current directory and all its sub-directories

    * Hidden files should be listed	
    * Only regular files (not directories) should be listed
    * The names of the files should be displayed without their extensions
    * The files should be sorted by byte values, but case-insensitive (file `aaa` should be listed before file `bbb`, file `.b` should be listed before file `a`, and file `Ron` should be listed after file `jay`)
    * One file name per line
    * The listing should end with a new line
    * You are not allowed to use `basename`, `grep`, `egrep`, `fgrep` or `rgrep` 

* `102-acrostic` - decodes acrostics that use the first letter of each line

    * The ‘decoded’ message has to end with a new line
    * You are not allowed to use`grep`, `egrep`, `fgrep` or `rgrep`

* `103-the_biggest_fan` - arses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.

    * Order by number of requests, most active host or IP at the top
    * You are not allowed to use `grep`, `egrep`, `fgrep` or `rgrep`
