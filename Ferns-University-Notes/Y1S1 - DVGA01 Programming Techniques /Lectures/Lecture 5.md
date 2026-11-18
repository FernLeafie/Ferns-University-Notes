## Pointers
Different datatypes take up different amount of memory addresses
```c
char c = 'A';
```

| ADDRESS | VALUE |
| :-----: | ----- |
|  `00`   | `65`  |

```c
short c = 65;
```

| ADDRESS | VALUE |
| :-----: | ----- |
|  `00`   | `0`   |
|  `01`   | `65`  |


```c
int c = 65;
```

| ADDRESS | VALUE |
| :-----: | ----- |
|  `00`   | `0`   |
|  `01`   | `0`   |
|  `02`   | `0`   |
|  `03`   | `65`  |
Here our `int`, takes up four whole addresses in memory, as it takes up four bytes of memory.

```c
char text[5] = "test";
```

| ADDRESS | NAME      | VALUE |
| ------- | --------- | ----- |
| `00`    | `text`    | `'t'` |
| `01`    |           | `'e'` |
| `02`    |           | `'s'` |
| `03`    |           | `'t'` |
| `04`    |           | `0`   |
| `05`    | `pointer` | `0`   |
| `06`    |           | `0`   |
| `07`    |           | `0`   |
| `08`    |           | `0`   |
```c
char text[5] = "test";
char *pointer = 0;
```
`char *pointer`, doesn't actually contain a `char`, but contains a pointer to a char. Or the address of a memory space where a variable containing a char is stored. Pointers are usually the same size as an `int`.
So instead of storing a value, we store a reference to another value.
The `*` in the variable name indicates that it's a pointer.
However usually we can't just assign numbers to a pointer, as we have no idea where in memory a variable will end up.

There are two symbols relating to pointer, that somewhat serves as each other's opposites:
	`*` pointer ${}\to{}$ value
	`&` value ${}\to{}$ pointer

```c
int a = 5;
printf("%d", &a);
// the & gives us a pointer to a
// so printf will print the memory address where a is located

printf("%d", *a);
// * interprets 5 as a pointer, and memory address
// so printf will print the value at the memory address 5
```

Now to redefine vectors and strings using pointers, as that's how C actually works with them.
```c
char text[5];
// is actually stored as
// |
// V
char *text;
```
It's just that C makes sure there are 5 memory spaces allocated after the first address.
```c
text[2] = 'a';
// is in reality
*(text + 2) = 97;
// as c looks up the value, stored at that pointer, plus two
// text just being a memory address, * turning that into the value
```

```c
int * pointer = text;
// this takes the memory value stored at texts address, and interprets it as an integer?
*pointer; // -> -2761293
```

```c
void * pointer;
// seemingly doesnt care about what datatype is in the memory? highly confusing
```

> [!NOTE] Syntax
> As long as the `*` comes before the name, the spaces can come where ever you like.
> ```c
> void * pointer;
> void* pointer;
> void *pointer;
> printf("%d", * pointer);
> printf("%d", *pointer);
> ```
> should all be valid, with the exception that the `printf` statement fails for other reasons.
### Examples
```c
int number = 5;
printf("%d\n", *(int*)number);
// int* typecasts it to a pointer
```
This results in a segmentation fault, since memory address 5 is outside our processes memory, and the operating system says no.
```c
int number = 5;
printf("%p\n", &number);
```
`%p` is the format string for a pointer, so this prints out the memory address of number.
```c
int number = 5;
int number2 = 3;
printf("number = %p\n", &number);
printf("number2 = %p\n", &number2);
```
Should yield two address spaces 4 apart, as an int is 4 byte long.
```c
int *ptr;
printf("pointer = %p\n", &ptr);
```
Gives us the address of the pointer. Pretty useless.
Pointers should always be initialised to `NULL`, as otherwise the program might run, if it's `NULL`, the programme crashes, if not, the value of the pointer might be manipulated to point at different data, and could cause severe security issues.
```c
int *ptr = NULL;
printf("pointer = %p\n", ptr);
```
Gives us the actual pointer stored in the pointer.
```c
int number = 5
int *ptr = &number; // sets pointer to a pointer to number
printf("pointer = %d\n", *ptr); // gives 5, the value stored at number
```
Now with vectors.
```c
int vector[5] = {7, 4, 9, 3, 1};
int *ptr = vector; // vector is already a pointer
printf("ptr = %d\n", *ptr); // yields 7
printf("ptr = %d\n", *ptr + 1); // yields 4

printf("ptr = %d\n", *(ptr++) + 1); // still yields 4, as ptr++ increases the value after the row is run
printf("ptr = %d\n", *ptr); // now yields 4, because of ptr++
```
And with strings
```c
char text[5] = "test";

char *ptr = text;

printf("ptr = %c\n", *ptr); // yields t, as that is the value of the first one
printf("ptr = %s\n", &*ptr); // yields t, the & is needed as %s wants a pointer to a char
printf("ptr = %s\n", ptr); // also yields t, the & and * nullify each other
```

```c
char text[5] = "test";

char *ptr = text;

printf("ptr = %c\n", *ptr);     // yields t
printf("ptr = %c\n", *ptr + 1); // yields e
printf("ptr = %c\n", *ptr + 2); // yields s
printf("ptr = %c\n", *ptr + 3); // yields t
printf("ptr = %c\n", *ptr + 4); // yields \0
```

```c
int number = 5;
unsigned char *ptr = (unsigned char*) &number;

for (int i = 0; i < sizeof(number); i++) {
	printf("%d ", *(ptr + i));
}
```
is silly, and prints how number is stored in memory, one byte at a time :3, since char is a byte large, and interpreted as integers.

### An Exam Example
```c
int main() {
	char * src = "foobar";
	char * dst = malloc(6);
	char * ptr;
	
	dst[0] = src[3]; // dst[0] = b
	ptr = &(src[5]); // ptr is the address of r
	dst[1] = *ptr; // dst[1] = r
	dst[2] = 'i' + (ptr - src);
	ptr = src + 4;
	ptr--;
	dst[3] = *(++ptr);
	*(dst+4) = *(ptr-4);
	dst[5] = 0;
	
	printf("%s", dst);
	
	return 0;
}
```
Goddesses.