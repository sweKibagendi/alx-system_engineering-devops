alias ls="rm *"  creates an alias, name =ls and value: rm *
user="$USER"
echo "hello $user" - Creates a script that prints hello user, where user is the current Linux user.
export PATH=$PATH:/action - Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.
echo $((`echo $PATH | grep -o ":/" | wc -l`+ 1)) - counts the number of directories in the PATH.
printenv - lists environment variables.
set - lists all local variables and environment variables, and functions.
BETTY=holberton - creates a new local variable.
export HOLBERTON=Betty = creates a new global variable
echo $((128+$TRUEKNOWLEDGE)) -  prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.
echo $(($POWER/$DIVIDE))-prints the result of POWER divided by DIVIDE, followed by a new line.
$(($BREATH**$LOVE)) - displays the result of BREATH to the power LOVE
echo $((2#$BINARY)) converts a number from base 2 to base 10.
echo {a..z}{a..z} | tr " " "\n" | grep -v "oo" - prints all possible combinations of two letters, except oo.
printf "%.2f" $NUM | sort - prints a number with two decimal places, followed by a new line.
perl -lne 'print if $. % 2 == 1' - prints every other line from the input, starting with the first line.
echo $((16#$DECIMAL)) - converts a number from base 10 to base 16.
tr `echo {a..z} | tr -d ' '` `echo {n..z} $(echo {a..m}) | tr -d ' '` | tr `echo {A..Z} | tr -d ' '` `echo {N..Z} $(echo {A..M}) | tr -d ' '`
encodes and decodes text using the rot13 encryption. Assume ASCII.
echo $(printf %o $(($((5#$(echo $WATER | tr 'water' '01234'))) + $((5#$(echo $STIR | tr 'stir.' '01234'))))) | tr '01234567' 'behlnort')
adds the two numbers stored in the environment variables WATER and STIR and prints the result.