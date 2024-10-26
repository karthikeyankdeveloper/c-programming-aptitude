## Question


Question 1
```
#include <stdio.h>

int process(int n) {

int result = 1;

for (int i = 1; i <= n; i++) {

result += i * i;  // Output?

}

return result;

}

int main() {

int num = 4;

printf("%d\n", process(num));  // Output?

return 0;

}
```
Question 2
```
#include <stdio.h>

int mysteryFunc(int n) {

if (n == 0)

return 0;

return (n % 2 == 0 ? n : 0) + mysteryFunc(n - 1);  // Output?

}

int main() {

printf("%d\n", mysteryFunc(6));  // Output?

return 0;

}
```
Question 3
```
#include <stdio.h>

int findValue(int a, int b) {

while (a != b) {

if (a > b)

a -= b;

else

b -= a;

}

return a;

}

int main() {

int x = 48, y = 18;

printf("%d\n", findValue(x, y));  // Output?

return 0;

}
```
Question 4
```
#include <stdio.h>

int calcValue(int n) {

int result = 0;

while (n > 0) {

result += n % 10;  // Output?

n /= 10;

}

return result;

}

int main() {

int num = 1234;

printf("%d\n", calcValue(num));  // Output?

return 0;

}
```
Question 5
```
#include <stdio.h>

int evaluate(int *arr, int size) {

int sum = 0;

for (int i = 0; i < size; i++) {

if (arr[i] % 2 != 0) {

sum += arr[i] * arr[i];  // Output?

}

}

return sum;

}

int main() {

int arr[] = {1, 2, 3, 4, 5};

printf("%d\n", evaluate(arr, 5));  // Output?

return 0;

}
```
Question 6
```
#include <stdio.h>

int sequence(int n) {

if (n == 0 || n == 1) return n;

return sequence(n - 1) + sequence(n - 2);  // Output?

}

int main() {

int num = 5;

printf("%d\n", sequence(num));  // Output?

return 0;

}
```
Question 7
```
#include <stdio.h>

int reverse(int n) {

int rev = 0;

while (n > 0) {

rev = rev * 10 + (n % 10);  // Output?

n /= 10;

}

return rev;

}

int main() {

int num = 12345;

printf("%d\n", reverse(num));  // Output?

return 0;

}
```
Question 8
```
#include <stdio.h>

int accumulate(int n) {

if (n == 1) return 1;

return n * n + accumulate(n - 2);  // Output?

}

int main() {

int num = 5;

printf("%d\n", accumulate(num));  // Output?

return 0;

}
```
Question 9
```
#include <stdio.h>

int transform(int n) {

return (n << 1) - 5;  // Output?

}

int main() {

int num = 6;

printf("%d\n", transform(num));  // Output?

return 0;

}
```
Question 10
```
#include <stdio.h>

int nestedCalc(int n) {

int count = 0;

for (int i = 1; i <= n; i++) {

for (int j = i; j <= n; j++) {

count += i * j;  // Output?

}

}

return count;

}

int main() {

int num = 3;

printf("%d\n", nestedCalc(num));  // Output?

return 0;

}

```

## Answer
-   Question 1: 31
-   Question 2: 12
-   Question 3: 6 (GCD of 48 and 18)
-   Question 4: 10 (Sum of digits of 1234)
-   Question 5: 35 (Sum of squares of odd numbers: 1² + 3² + 5²)
-   Question 6: 5 (Fibonacci of 5: 0, 1, 1, 2, 3, 5)
-   Question 7: 54321 (Reverse of 12345)
-   Question 8: 35 (5² + 3² + 1²)
-   Question 9: 7 ((6 << 1) - 5 = 12 - 5 = 7)
-   Question 10: 25