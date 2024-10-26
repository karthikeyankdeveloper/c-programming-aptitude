## Question Type

-   Question 1 - String with Pointer
-   Question 2 - String Modification via Pointer
-   Question 3 - Pointer to String Literal (Error-prone)
-   Question 4 - Null Pointer with String
-   Question 5 - Pointer to Pointer (String)
-   Question 6 - Common Error: Uninitialized Pointer
-   Question 7 - String Length Calculation (Pointer)
-   Question 8 - Array of Pointers to Strings
-   Question 9 - Pointer Arithmetic on Strings
-   Question 10 - Pointer Error: Invalid Memory Access

  

## Question

Question 1
```
#include <stdio.h>

int main() {

char str[] = "Hello";

char *ptr = str;

printf("%c\n", *ptr);

printf("%c\n", *(ptr + 1));

return 0;

}
```
Question 2
```
#include <stdio.h>

int main() {

char str[] = "World";

char *ptr = str;

*ptr = 'H';

printf("%s\n", str);

return 0;

}
```
Question 3
```
#include <stdio.h>

int main() {

char *str = "Hello";

str[0] = 'Y';  // Is this allowed? What happens?

printf("%s\n", str);  // Output?

return 0;

}
```
Question 4
```
#include <stdio.h>

int main() {

char *str = NULL;

printf("%s\n", str);  // Output? Is this correct?

return 0;

}
```
Question 5
```
#include <stdio.h>

int main() {

char *str[] = {"Hello", "World", "C"};

char **ptr = str;

printf("%s\n", *ptr);  // Output?

printf("%s\n", *(ptr + 1));  // Output?

return 0;

}
```
Question 6
```
#include <stdio.h>

int main() {

char *str;

printf("%s\n", str);  // Is this correct? What happens?

return 0;

}
```
Question 7
```
#include <stdio.h>

int stringLength(char *str) {

int len = 0;

while (*str != '\0') {

len++;

str++;

}

return len;

}

int main() {

char str[] = "C Programming";

printf("%d\n", stringLength(str));  // Output?

return 0;

}
```
Question 8
```
#include <stdio.h>

int main() {

char *colors[] = {"Red", "Green", "Blue"};

printf("%s\n", colors[1]);  // Output?

return 0;

}
```
Question 9
```
#include <stdio.h>

int main() {

char str[] = "Pointer";

char *ptr = str;

printf("%c\n", *(ptr + 3));  // Output?

return 0;

}
```
Question 10
```
#include <stdio.h>

int main() {

char *str = "Hello";

printf("%c\n", str[10]);  // Is this allowed? What happens?

return 0;

}

```

## Answer
Answer 1

-   Output:

-   H
-   e

Answer 2

-   Output:

-   Horld

Answer 3

-   Error:

-   Modifying a string literal leads to undefined behavior (usually segmentation fault).

Answer 4

-   Output:

-   Likely a runtime error (dereferencing NULL pointer).

Answer 5

-   Output:

-   Hello
-   World

Answer 6

-   Error:

-   Uninitialized pointer str, behavior is undefined.

Answer 7

-   Output:

-   13 (length of "C Programming")

Answer 8

-   Output:

-   Green

Answer 9

-   Output:

-   n (4th character in "Pointer")

Answer 10

-   Error:

-   Out of bounds access, undefined behavior (likely segmentation fault).