# CS50 Final project
## Common feedback

Below are some of the most common comments I inserted into student code.

* *Before a `#include "../somedir/somefile.h"`:*
Do not put a pathname in #include lines; leave it to Makefile to provide -I

* *In the .c file for a module that has a corresponding .h file:*
You must `#include "module.h"` so compiler can cross-check the declarations in the header file with the definitions in this file.

* *In a module with no main() function and with a corresponding header file:*
The following prototypes should be marked 'static', if they are meant to be for internal-use only, or should be removed entirely if they are defined in the corresponding header file.

* *In a program with a main() function:*
The following prototypes should be marked 'static', since they are internal-use only.  Also, use 'const' where possible in function prototypes.

* Use 'const' where possible in function prototypes.

* *In a file with global variables, particularly if they are not wrapped in a struct:*
Global variables are always risky, and I *strongly* suggest wrapping them into a single struct so their use throughout the code becomes immediately clear that they are globals, not some local variable.
Recall the hint about global variables:
https://github.com/cs50spring2021/nuggets-info#global-variables

* *Before a local (static) function that has no header comment:*
Local functions need good header comments because they are not described in a header file.

* *In a function-header comment:*
What's the memory contract?

* *At the top of a function receiving parameters:*
Be defensive here, check parameters before using them.                            

* *Before a statement that calls a function that might return NULL:*
What if this fails and returns NULL?

* *Before a call to malloc or calloc:*
What if malloc fails (returns NULL)?

* *Before the definition of a `struct`:*
Each member of the struct should have a brief inline comment to describe it.

* Define named constants for all the grid characters (like walls, spots, and gold) rather than sprinkling code with character constants.  A named constant will make the code more readable, and more adaptable if there is a later need to change characters.

* *In cases where code uses `malloc` to allocate space for a fixed-size string:*
When you need a string variable of a fixed size, there is no need for malloc.  Just declare a local string variable.

* *In cases where code uses `malloc` to allocate space for a string to pass to `message_send()`:*
You use malloc when it is not necessary; e.g., to create a message string, it would be sufficient to define one local variable `char message[message_MaxBytes]` and sprintf into that string.  Such a string is (by definition) big enough for any message in the game.  No malloc/free needed.

* *In cases where code parses the `seed` parameter with `atoi()` or similar:*
`atoi`is inadequate for parsing an integer from user input.  Recall the trick we learned:
https://www.cs.dartmouth.edu/~cs50/Lectures/units/examples/atoi.c

* *In handleMessage code to parse messages:*
Recall the hint about parsing messages:
https://github.com/cs50spring2021/nuggets-info#parsing-messages

* *In code with complex approaches to convert numbers to letters:*
Recall the hint about translating numbers to letters, and letters to numbers:
https://github.com/cs50spring2021/nuggets-info#converting-from-letters-to-numbers-and-back

* Your code often uses "magic numbers", i.e., literal integer constants that just happen to be the right number for something, but often without explanation.  Such practice is risky because the code is less readable and more fragile to future changes.  Define a named constant for such numbers, or find another approach.

* Try to keep code lines less than 80 characters wide, so the code reads well in a standard 80-column window.  Set the indentation step size at 2 characters (or at most 4 characters) to keep the code horizontally compact.  Use spaces rather than tabs so the code views the same way in all viewers/editors.  Wrap lines at readable points rather than letting the viewer/editor wrap arbitrarily. Restructure code if needed.  Move in-line comments to the prior line if needed.

* *In files with DOS line endings:*
This file has DOS line endings; recall we are coding for UNIX not DOS.
