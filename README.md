ALX Software Enginering Printf Team Project
This team project is a custom made printf function for the C programming language called _printf. It has been optimized to take various inputs and optional arguments based exactly on how the standard library function printf works. We submitted this as part of the ALX software engineering course requirement for grading.

printf Function in C
Syntax:

#include <stdio.h>

int printf(const char *format, ...);
Description:
The printf function is part of the standard input/output library (<stdio.h>) in C. It is designed for formatted output to the standard output, typically the console. The function takes a format string (format) and a variable number of arguments, which are inserted into the format string according to specified format specifiers.

Parameters:
format (const char):*

A string that specifies the format of the output. It may contain ordinary characters and format specifiers. Format specifiers begin with a percent sign % and are replaced by the corresponding values of additional arguments.
... (ellipsis):

An ellipsis indicates a variable number of arguments. These are the values to be formatted and inserted into the format string.
Return Value:
The printf function returns the total number of characters written to the standard output. In case of an error, a negative value is returned.
Format Specifiers:
printf uses format specifiers to control the formatting of the output. Some common format specifiers include:

%d: Signed decimal integer
%u: Unsigned decimal integer
%f: Decimal floating-point
%s: String
%c: Character
%x: Hexadecimal (lowercase)
%X: Hexadecimal (uppercase)
Example Usage:

#include <stdio.h>

int main() {
    int num = 42;
    float pi = 3.14159;
    char name[] = "John";

    printf("Integer: %d\n", num);
    printf("Float: %f\n", pi);
    printf("String: %s\n", name);

    return 0;
}
Notes:
Format String:

The format string may contain ordinary characters and format specifiers. Ordinary characters are printed as they are, while format specifiers are replaced by the corresponding argument values.
Argument Matching:

The order and type of arguments must match the format specifiers in the format string. Mismatched types can result in undefined behavior.
Escape Sequences:

Escape sequences, such as \n for newline, can be used within the format string.
Usage Recommendations:
Safety Considerations:

Be cautious with user input to prevent format string vulnerabilities.
Type Safety:

Ensure that the format specifiers match the type of the corresponding arguments to avoid unexpected behavior.
Precision and Width:

Format specifiers often support precision (%.2f) and width (%10s) options for more control over the output.
