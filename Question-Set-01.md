## Question Type
1. Pointer Basics
2. Pointer Arithmetic
3. Recursion
4. While Loop
5. Recursion with Return
6. Pointer with Function
7. Nested Loops
8. Pointer and Array

## Question

Question 1

```
	#include <stdio.h>

	int main() {

	int a = 10;

	int *ptr = &a;

	printf("%d\n", *ptr);  // Output?

	*ptr = 20;

	printf("%d\n", a);  // Output?

	return 0;

	}

```

Question 2
```
	#include <stdio.h>

	int main() {

	int arr[] = {10, 20, 30, 40};

	int *ptr = arr;

	printf("%d\n", *(ptr + 2));  // Output?

	printf("%d\n", *ptr);  // Output?

	ptr++;

	printf("%d\n", *ptr);  // Output?

	return 0;

	}
```
Question 3
```
	#include <stdio.h>

	int factorial(int n) {

	if (n == 0)

	return 1;

	else

	return n * factorial(n - 1);

	}

	int main() {

	int num = 5;

	printf("%d\n", factorial(num));  // Output?

	return 0;

	}
```

Question 4
```
#include <stdio.h>

int main() {

int count = 5;

while (count > 0) {

printf("%d\n", count);  // Output each iteration?

count--;

}

return 0;

}
```
Question 5
```
#include <stdio.h>

int fun(int x) {

if (x == 1)

return 1;

else

return x + fun(x - 1);

}

int main() {

printf("%d\n", fun(5));  // Output?

return 0;

}
```
Question 6
```
#include <stdio.h>

void changeValue(int *ptr) {

*ptr = 50;

}

int main() {

int num = 10;

changeValue(&num);

printf("%d\n", num);  // Output?

return 0;

}
```

Question 7
```
#include <stdio.h>

int main() {

for (int i = 1; i <= 3; i++) {

for (int j = 1; j <= 3; j++) {

printf("%d ", i * j);  // Output for each iteration?

}

printf("\n");

}

return 0;

}
```
Question 8
```
#include <stdio.h>

int main() {

int arr[] = {1, 2, 3, 4, 5};

int *ptr = arr;

printf("%d\n", *(ptr + 3));  // Output?

return 0;

}

```

## Answer 
Question 1:

-   10 (Dereferencing the pointer to get the value of a)
-   20 (The value of a is updated through the pointer)

 Question 2:

-   30 (Value at the 3rd position in the array, arr[2])
-   10 (Value at the 1st position in the array, arr[0])
-   20 (Pointer moves to the 2nd position, arr[1])

Question 3:

-   120 (Factorial of 5: 5 * 4 * 3 * 2 * 1 = 120)

Question 4:

-   5 4 3 2 1 (The loop prints the value of count as it decrements from 5 to 1)

Question 5:

-   15 (Recursive sum of 5 + 4 + 3 + 2 + 1)

 Question 6:

-   50 (The value of num is changed to 50 through the pointer in the function)

Question 7:

-   1 2 3
-   2 4 6
-   3 6 9 (Multiplication table of 1 to 3)

Question 8:

-   4 (Value at the 4th position in the array, arr[3])
