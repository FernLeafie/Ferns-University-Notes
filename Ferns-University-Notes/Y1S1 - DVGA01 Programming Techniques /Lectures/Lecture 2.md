## Basics of C

Our hello world yesterday started with the line
`#include <stdio.h>`
this is a command to the preprocessor in the compiler.
`#include` takes one parameter, which is a file that it takes and copies into that spot in the code.
`"file.h"` will import the file from the same directory.

The `<` `>` in `<stdio.h>` tells the preprocessor to find the library in the systems library collection

```c
int main() {

}
```
Is our entry function, this is a function of the name `main`, that returns an `int` when it finishes

The `{ }` indicate a programming block, and mark the beginning and end of the function

```c
int main() {
  printf("Hello World\n");
}
```
`printf` is a function from the standard library input output, `stdio`, 
When calling a function it can take an argument or a list of arguments, which are used in the functions body, `fun(arg1, arg2, ..., argN)`. `printf` prints formatted text to the terminal

`"hello world"` is a string, indicated by the `" "`.

The `;` indicates the end of a line, or the end of a function call, all lines that don't open a new code block should be followed by a `;`. Multiple commands can be written on one line if separated by a `;`.

```c
int main() {
  printf("hello world");
  return 0;
}
```
`return 0;` ends the function, by returning an exit code, of the type `int` specified earlier, 0 is the Unix exit code for the program succeeding, but it can return any number it desires.

### Libraries

|    name    |           summary            |
| :--------: | :--------------------------: |
| `stdio.h`  |       input and output       |
| `string.h` |         text actions         |
| `stdlib.h` | miscellaneous help functions |
One can find more info about the libraries by searching the internet.
Or on Linux by running `man <library name>`, for example `man stdlib.h`.
### Variables
Memory is divided into segments of 64 bits, due to our CPU architecture, or 8 bytes.
if we declare a variable
`int size;`
the programme will request a bit of memory, and the computer will allocate it, or give it to the programme. The programme can then refer to it by the name of the variable, in this case `size`.

The `int` is a datatype, which tells the programme how to interpret the data stored there, and how to save it.

|  Datatype   |                                              |  size  |
| :---------: | -------------------------------------------- | :----: |
|    `int`    | integer, whole number, positive, or negative | 32-bit |
| `long long` | larger integer                               | 64-bit |
|   `short`   | smaller integer                              | 16-bit |
|   `char`    | one character                                | 8-bit  |
All these can be signed and unsigned, that meaning capable of being positive and negative, or only being positive.

| Datatype |                                           |  size  |
| :------: | ----------------------------------------- | :----: |
| `float`  | decimal number                            | 32-bit |
| `double` | more precise decimal number               | 64-bit |
|  `void`  | kinda a datatype, doesn't return anything | 0-bit  |

`float` - Single-precision floating-point
`double` - Double-precision floating-point
Both use the same theory as the scientific notation

```c
int size;
float number;
number = 5;
size = 5 * (1 + 1);
size = size + 1
```
Equals is different from in maths, in programming it usually means assigning a value to a variable, so assigning the right hand side to the left hand side. Calculating the right hand side by doing so.

C is sequential, so the order of things matter, and data changes throughout the progression of the programme

```c
int age = 30;
```
is both a declaration of the variable `age`, and assigning a variable, it essentially does both
```c
int age;
age = 30;
```

Until a value is assigned to a variable, the variable doesn't contain empty, it contains whatever was in the memory before, so random rubbish essentially.
So
```c
int sum;
sum = sum + 1;
```
Doesn't yield 1, but yields a random value plus 1

`sum = sum + 1`
Can also be written with the short hands
```c
sum += 1;
sum++;
++sum;
```

In this case `sum++` and `++sum` yield the same result
```c
int a = 1;
int b;
```
```c
b = a++;
// b == 1, a == 2, 
// assigns first, increases a second
```
```c
b = ++a;
// b == 2, a == 2
// increases a first, assigns b second
```
`sum--` and `--sum` also exist

#### Char
```c
char a = 97;
// stores the number 97 in a
```
This variable can either be interpreted as the number it contains, or the letter that number refers to, in a lookup table, normally ASCII or UTF-8.
```c
char b = 'a';
// this assigns the number which represents a in the ASCII lookup table
// a = 97
```
As char is just a number, you can do silly and stupid things to it.
```c
b = b + 5
// b == 'f'
```
We don't need to recall the numbers in ASCII which the letters are represented by, as we can always refer to them as letters in C

#### Type Casting
```c
int a = 10;
int b = 3;

int c = a / b;
// c == 3
// since both a and b are integers
// C will do an integer division
// which will always truncate the resulting value
// that meaning rounding down

float c = a / b;
// c == 3
// C will still do an integer division

float c = (float) a / (float) b;
// c == 3.3333...
// this will cast a and b into floats
// C will interpret them as floats
// and do a floating poinnt division
```
Type casting converts between types, and can have many unintended consequences if casting into a lower type.

#### Printing Values
```c
int main() {
  int size = 10;
  char letter = 'a';
  // letter = 97;
  
  printf("size is: %d \n", size);
  // %d refers to a digit in the input arguments

  printf("letter is: %c \n", letter)
  // %c prints the value as if it's a char

  printf("letter is: %d \n", letter)
  // this prints the value stored in letter
  // letter is interpreted as a digit
  // 97

  return 0;
}
```
Everything in a computer is digits, and can be manipulated as such, all we do is choose how to interpret it.
The `%d, %i, %c` decides how `printf` interprets the values
```c
int main() {
  char letter = 'a';
  letter = 'b' - ('a' - 'A');
  
  printf("%c \n", letter);
  // prints B
}
```

#### Reading Values
Values are read from the terminal using `scanf`
```c
int main() {
  int num1;
  int num2;
  
  scanf("%d %d", &num1, &num2);
  int sum = num1 + num2;
  
  printf("%d\n", sum);
  
  return 0;
}
```
`&` indicates a pointer, which will be covered later.

When doing labs in Autolab, output and input has to match fully, and the program shouldn't return anything other than 0.