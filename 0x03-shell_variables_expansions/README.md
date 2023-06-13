# 0x03. Shell, init files, variables and expansions

This repo contains tasks for my 0x02. Shell, I/O Redirections and filters Project. The following are topics covered in this project:

* Expansions
* Shell Arithmetic
* Variables
* Shell initialization files
* The alias Command
* Technical Writing
* man or help

## Tasks

The following are scripts in this directory and their uses: 

* `0-alias` - Create a script that creates an alias.

    * Name: `ls`	
    * Value: `rm *`

* `1-hello_you` - prints hello user, where user is the current Linux user.
* `2-path` - Adds `/action` to the `PATH`. `/action` should be the last directory the shell looks into when looking for a program.
* `3-paths` - counts the number of directories in the `PATH`.
* `4-global_variables` - lists environment variables
* `5-local_variables` -  lists all local variables and environment variables, and functions
* `6-create_local_variable` - creates a new local variable

    * Name: `BEST`
    * Value: `School`

* `7-create_global_variable` - creates a new global variable.

    * Name: `BEST`
    * Value: `School`

* `8-true_knowledge` - prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line
* `9-divide_and_rule` - prints the result of `POWER` divided by `DIVIDE`, followed by a new line. `POWER` and `DIVIDE` are environment variables
* `10-love_exponent_breath` - displays the result of `BREATH` to the power `LOVE`
    
    * `BREATH` and `LOVE` are environment variables
    * The script should display the result, followed by a new line

* `11-binary_to_decimal` - converts a number from base 2 to base 10.

    * The number in base 2 is stored in the environment variable `BINARY`  
    * The script should display the number in base 10, followed by a new line

* `12-combinations` - prints all possible combinations of two letters, except oo.

    * Letters are lower cases, from a to z 
    * One combination per line
    * The output should be alpha ordered, starting with aa
    * Do not print oo
    * Your script file should contain maximum 64 characters

* `13-print_float` - prints a number with two decimal places, followed by a new line. The number will be stored in the environment variable `NUM`
* `100-decimal_to_hexadecimal` - converts a number from base 10 to base 16.

    * The number in base 10 is stored in the environment variable `DECIMAL`
    * The script should display the number in base 16, followed by a new line

* `101-rot13` - encodes and decodes text using the rot13 encryption. Assume ASCII
* `102-odd` - prints every other line from the input, starting with the first line
* `103-water_and_stir` - adds the two numbers stored in the environment variables `WATER` and `STIR` and prints the result.

    * `WATER` is in base `water`
    * `STIR` is in base `stir`
    * The result should be in base `bestchol`
