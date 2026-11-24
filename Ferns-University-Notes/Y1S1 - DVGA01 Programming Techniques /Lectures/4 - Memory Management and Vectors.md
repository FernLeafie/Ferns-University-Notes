## Memory Handling
### Vectors
```c
char[]
int[]
```
```c
int b = 5;
int a[3]; // creates a list of three integers
int c;
```

|  ADDR  | NAME          | VALUE |
| :----: | :------------ | :---: |
| `0x00` | b             |   5   |
| `0x04` | a             |   ?   |
| `0x08` | reserved by a |   ?   |
| `0x0B` | reserved by a |   ?   |
| `0x10` | c             |   ?   |
| `0x14` |               |       |

> [!INFO]
> The `0x` prefacing the addresses, doesn't have any meaning, other than indicating that the following number is in hexadecimal

Here every address refers to a 4 byte large segment, or 32 bit.
As C doesn't clear the memory beforehand, the values of a variable after it's declared, is unknown, as it's the same values as what was in the memory there beforehand.

To access the values within this list `a`, we address it by an index. The list is called a vector in C, but usually arrays in other languages.
```c
a[0] = 4;
a[1] = 2;
a[2] = 0;
```
The vector starts at zero, since it can be thought of as the memory address of the first space, plus zero places, that being space one in the list.
```c
a[0] // a + 0, first address of a
a[1] // a + 1, second address of a
a[2] // a + 2, third address of a
```
To create an empty vector when initialising, to avoid the random memory, we can use the syntax:
```c
int a[3] = {0};
```

Do not create an array with the length of a variable, the compiler will allow it, but it can get weird, and has a performance cost.
```c
// don't
int n;
scanf("%d", &d);
int number[n];
```

If we wanna read in a sequence of values, we can do it simply through a for loop.
```c
int number[100];
int n;
scanf("%d", &n);
for (int i = 0; i < n; i++) {
	scanf("%d", &number[i]);
}
```

As a vector is just a continuous sequence of memory, we can't remove a value from the middle of the list. Since it's rather difficult to just, pick up a hammer and punch out the specific cell of memory

| `tal[100]` | ${}n=5{}$ |     |     |     |
| ---------- | --------- | --- | --- | --- |
| 3          | 7         | 0   | 1   | 9   |
So if we wanna remove 0, we'd have to move all values behind it forward, one step at a time, til we get `[3, 7, 1, 9]`.

| `tal[100]` | ${}n=4{}$ |     |     |
| ---------- | --------- | --- | --- |
| 3          | 7         | 1   | 9   |
If we wanna insert a value into an array, we'd do the opposite, copying values forward.

|     |     |     |     |
| --- | --- | --- | --- |
| 7   | 3   | 5   | 9   |
and then we can insert our value into the space we want to.

|     |     |     |     |     |
| --- | --- | --- | --- | --- |
| 7   | 3   | 1   | 5   | 9   |
But as the memory of this vector is statically allocated, we can't adjust the actual size the vector occupies in memory, just how much space we use of that vector.
If we attempt to write outside the allocated size of the vector, the operating system says no, and we get an error called `SEG FAULT`, or Segmentation Fault.
### Strings
C doesn't have a dedicated datatype for strings, instead strings are constructed from the same base components that many other languages use to build their strings, it's just a vector, of characters, or chars.
```c
char text[5];
text[1] = 'A';
```

|  ADDR  | NAME | VALUE |
| :----: | ---- | :---: |
| `0x00` | text |       |
| `0x01` |      | `'A'` |
|  ...   |      |  ...  |

```c
char text[5] = "Test"; // immedietly assign text into the string, or characters into the array
```

|  ADDR  | NAME | VALUE |
| :----: | :--- | :---: |
| `0x00` | text | `'T'` |
| `0x01` |      | `'e'` |
| `0x02` |      | `'s'` |
| `0x03` |      | `'t'` |
| `0x04` |      |  `0`  |
| `0x05` |      |       |
Here every address refers to 1 byte, or 8 bits, as a char only occupies a byte.
In C a string has to end with a `0` byte, also called a null byte terminator, it can be written as `\0` in strings. This is called C style strings.
When scanning in a string in C, no pointer `&` is needed. As a vector is already a pointer, and the format string `%s` is already a pointer (but we will go through pointers later).
```c
scanf("%s", text); // char *
// as opposed to
scanf("%d", &a); // int -> int *
```

If we wanna insert a string into a variable, after its creation, we can't set it equal to, we have to use `strcat()` from `<string.h>`
```c
#include <string.h>
int main() {
	char text[100] = {0}; // fill the string with null byte terminators
	
	strcat(text, "Hello");
}
```
`strcat()` looks up the first null byte of the variable, and inserts the string there. So it concatenates the string with your variable.

When writing out a string a character at a time, we have to stop at the first null byte terminator, or else we will spit out a bunch of garbage.
```c
#include <string.h>
#include <stdio.h>
int main() {
	char text[10] = {0}; // fill the string with null byte terminators
	
	strcat(text, "Meow");
	
	for (int i = 0; i < 10; i++) {
		printf("%c,", text[i]);
	}
	// will yield m,e,o,w,,,,,,,
	
	// if we instead loop it to strlen(),
	// which is a function that gives the length of the string, up until the first \n
	// sizeof(), will just give us the size of the vector so it's useless
	for (int i = 0; i < strlen(text); i++) {
		printf("%c,", text[i]);
	}
	// will yield m,e,o,w,
}
```

`strlen` doesn't return an int, it returns an unsigned long, which as previously mentioned, is just a really long int, without negative numbers.

The assignment syntax of `{0}`, can also assign multiple values across the vector, in which case the last value will be assigned across the rest of the vector. For example, `{0, 1, 2, 3, 4, 0}` will assign 0-4 to the first 5 memory addresses, and 0 to the rest.