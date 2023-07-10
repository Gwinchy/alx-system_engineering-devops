Commands:

head: Displays the beginning lines of a file or the output of a command.
tail: Displays the ending lines of a file or the output of a command.
find: Searches for files and directories based on specified criteria.
wc: Counts the number of lines, words, and characters in a file or the output of a command.
sort: Sorts the lines of a file or the output of a command.
uniq: Filters out repeated adjacent lines from a file or the output of a command.
grep: Searches for lines matching a specified pattern in a file or the output of a command.
tr: Translates or deletes characters in a file or the output of a command.
Redirecting Standard Output to a File: To redirect the standard output of a command to a file, you can use the > operator followed by the filename. For example:

bash
Copy code
command > output.txt
This command will execute the command and save its output to the output.txt file, overwriting any existing content.

Getting Standard Input from a File: To use a file as the input for a command instead of the keyboard, you can use the < operator followed by the filename. For example:

bash
Copy code
command < input.txt
This command will execute the command using the contents of input.txt as the input.

Sending Output from One Program to Another: To send the output of one program as the input to another program, you can use the pipe (|) operator. For example:

Copy code
command1 | command2
This command will execute command1 and pass its output as the input to command2.

Combining Commands and Filters with Redirection: You can combine commands and filters with redirection operators to perform complex operations. For example:

lua
Copy code
command1 | filter1 | command2 > output.txt
This command will execute command1, pass its output through filter1, and then execute command2 with the filtered output, saving the final result to output.txt.

Special Characters:

White spaces: Used to separate command-line arguments and options.
Single quotes (''): Preserve the literal value of each character within the quotes, preventing variable expansion and command substitution.
Double quotes (""): Allow variable expansion and command substitution within the quotes.
Backslash (): Escapes the next character, preserving its literal meaning.
Comment (#): Indicates the start of a comment. The rest of the line after the '#' symbol is ignored by the shell.
Pipe (|): Connects the output of one command to the input of another command.
Command separator (;): Separates multiple commands on a single line.
Tilde (~): Represents the home directory of the current user or a specified user.
Understanding when and how to use these special characters is important for writing effective shell commands and scripts. Their usage varies depending on the specific context and requirements of the task at hand.
