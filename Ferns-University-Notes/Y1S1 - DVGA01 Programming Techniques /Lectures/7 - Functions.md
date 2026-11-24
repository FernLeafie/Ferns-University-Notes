A program receives parameters and returns a result.
```c
int main() {
	return 0;
}
```
The function `main` (in this case) doesn't receive any parameters, but returns a value, `0`.
`main` can receive up to two parameters, `argc` and `argv`.
These functions work a bit like mathematical functions, they have a domain, and a codomain, a value received, and a processed value returned.

We have earlier called builtin functions.
```c
char text[10] = "Hello";
int n = strlen(text);
```

If we look at in libc, `strlen` is defined as:
```c
unsigned int strlen(const char *s);
/*return*/  /*name*/ /*inputs*/
```

This takes a parameter of the type `const char *s`.
And returns a value of type `unsigned int`. It could return `int`, but as the length of something can't be negative, we indicate to the user that we will never return a negative value.

A function's syntax can be defined generally as:
```c
<returntype> <name>(<paramtype> <paramname>, ...);
```
So a few examples of function declarations:
```c
int add(int a, int b);
int subtract(int a, int b);
float sum(float list[]); // obs [] needs to be empty
char * strcat(char * dst, char * src);
```

Functions can be declared with `void` as return type, meaning they don't return anything.
```c
void saymyname(char * name);
```
(They can still have a `return;`, it just isn't allowed to have a value)
Functions can also be without parameters, `void` is then written withing the parentheses.
```
int gettimeofday(void);
```
This can also be written with an empty parenthesis `()`. But then an end user can still pass arguments into the function, which may overwrite memory in weird ways.

If we have the declaration of a function, we know that parameters they take, and what they return.
For libc functions, these can be found in man pages
```bash
$ man 3 puts
```
```man
SYNOPSIS
     #include <stdio.h>
     
     int puts(const char *s);

DESCRIPTION
     puts() writes the string s and a trailing newline to stdout.
     
RETURN VALUE
     puts() and fputs() return a nonnegative number on success, or EOF on error.
```

We can create our own functions, in that case we need a declaration and a definition.
At the top of the file (under `#include` and `#define`), we declare it.
```c
int add(int a, int b);
```
(this is needed as C compilers read files from top to bottom)

Further down in the file, we define what it actually does.
```c
int add(int a, int b) {
	return a + b;
}
```

What do we use a function for? Essentially avoiding repeating code, and making it more readable, and easier to debug.

### Scope
Variables only exist within the block (`{}`), they're defined. Regardless of type. You know this from Rust.
Values passed into a function, exist only in the scope of the function.
```c
int a = 10;
{
	int b = 20;
}
int c = 10 + b; // not valid
```

Within a block you can access variables outside it, but outside it, you can't access variables within it.
```c
int a = 10;
if a > 5 {
	int b = a; // Ok
}
int c = a; // Ok
int c = a + b; // not valid
```

A function doesn't return a variable, but the value within the variable.
Variables within a functions are called local variables, as they're only accessible within their own scope.

Variables declared without a scope, are called global variables.
```c
int sum;
void add(int a, int b) {
	sum = a + b;
}
int main() {
	add(5, 10);
	printf("%d", sum);
	return 0;
}
```
This is completely valid, but totally horrid, and is not recommended.

If both a local and global variable share a name, the local takes president.
Parameters are local variables
```c
void fun(int x) {
	x += 5;
}
int main() {
	int x = 5;
	fun(x);
	printf("%d", x);
	return 0;
}
```
Still prints `5` as `x` is set to `5` and fun doesn't return the changed value, so it just goes out of scope, and `main` prints its own `5`.

What if we wanna make it print `10`? we return the value
```c
int fun(int x) {
	x += 5;
	return x;
}
int main() {
	int x = 5;
	x = fun(x);
	printf("%d", x);
	return 0;
}
```
prints `10`.

Arrays as parameters, the scoping doesn't apply to arrays, as they're pointers, and not values, so the function
```c
void fun(int a[]) {
	a[0] += 5;
}
int main() {
	int a[3] = {5, 5, 5};
	fun(a);
	printf("%d", a[0]);
	return 0;
}
```
So the function receives a reference to main's array, and can change it.
In the same way we can take pointers as the input of a function to achieve the same result, `scanf` for example does this.
```c
void fun(int * x) {
	*x += 5; // change the location of pointer x
}
int main() {
	int x = 5;
	fun(&x); // send the address to x
	printf("%d", x); // print the contents of x
	return 0;
}
```
Parameters like these are called out parameters.

## Examples
### String Length
```c
#include <stdio.h>
unsigned int mystrlen(char * text);

int main() {
	char * text = "Hello world!";
	int length = mystrlen(text);
	printf("%d\n", length);
	return 0;
}

unsigned int mystrlen(char * text) {
	char * start = text;
	// this works as anything other than all zeroes is true in C
	// and the nullbyte we're looking for is all zeroes
	while (*text) {
		// advance the pointer to look at the next byte
		text++;
	}
	// difference between final pointer location and starting pointer location
	// the length
	return text - start;
}
```
### String Concatenation
```c
#include <stdio.h>
char * mystrcat(char * a, char * b);

int main() {
	char text[32] = "Hello ";
	mystrcat(text, "world!");
	printf("%d\n", text);
	return 0;
}

char * mystrcat(char * a, char * b) {
	char * start = a;
	while(*a) {
		a++; // find end of first string
	}
	while(*b) {
		// copy chars of b into a until end of string b
		*a = *b;
		a++;
		b++;
	}
	return start;
}
```
Hopefully this runs, I have not double checked it, and it was written directly in obsidian.