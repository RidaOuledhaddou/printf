README PRINTF
Write a function that produces output according to a format.
Prototype: int _printf(const char *format, ...);
Returns: the number of characters printed (excluding the null byte used to end output to strings)
write output to stdout, the standard output stream
format is a character string. The format string is composed of zero or more directives. See man 3 printf for more detail. You need to handle the following conversion specifiers:
c
s
%
You don’t have to reproduce the buffer handling of the C library printf function
You don’t have to handle the flag characters
You don’t have to handle field width
You don’t have to handle precision
You don’t have to handle the length modifiers
Psuedo code :
Checking is the format is NULL, and return (-1) is case it is
Loop over format
Check if the character in the itteration is equal to %, if true :
Check if the next character is null, if true :
Return (-1)
Use the switch to check the character that is after the %;
In case it's s :
Print using ......
