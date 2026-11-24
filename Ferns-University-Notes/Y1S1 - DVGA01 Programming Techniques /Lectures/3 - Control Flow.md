## Control Flow

`if` ${}\iff{}$ `switch`

`for` ${}\iff{}$ `while`

When do we use which?
`switch` is fitting when we need to compare a variable against exact contents, as the comparison is only exact and not an expression.
`if` is fitting for expressions, more complex comparison, or expressions made out of multiple expressions.
The difference between `for` and `while` is mostly syntactical, as you can accomplish the same behaviour with both.
```c
for (;status == 1;) {
	
}
// and 
while (status == 1) {
	
}
// have the same behaviour
```
`while` might be more fitting when you're not aware of how many iterations are needed til the condition is met, but the same can be accomplished with a `for`, since expression 2 of `for` doesn't need to compare the iterator.

### For
```c
for (/*expr 1*/; /*expr 2*/; /*expr 1*/) {
	
}
// is equivalent to

/*expr 1*/
while (/*expr 2*/) {
	
	/*expr 3*/
}

```
Expression 1 is a variable initialisation, ran before the loop.
Expression 2 is an expression for which the loop will run whenever it's true.
Expression 3 is a function changing the initialised value, ran at the end of the loop.

```c
#include <stdio.h>
int main() {
	int const count = 5;
	int numbers[count];
	for (int i = 0; i < count; scanf("%d", &numbers[i])) {
		i++;
	}
	for (int i = 0; i < count; printf("%d\n", numbers[i])) {
		i++;
	}
	return 0;
}
```
You don't have to be smart with what expressions you put where, it's mostly for legibility, this is valid C, although a little stupid.
If we wanna iterate over something backwards with a for loop, we can just change the expressions
```c
for(int i = 9; i >= 0; i--) {

}
```
I mean it's programming, do whatever you want.
### Do While
For loops the value is checked before the loop is run. However, while loops can check the expression at the end instead, with a `do while` loop.
```c
do {
  // ...
} while ();
```
### Scoping!
A variable only exists from its initialisation, until the end of its scope, or block, where it's dropped.
```c
int main {
	char a;
	if (a == 'b') {
		int number = 7;
		// a and number exist here
	}
	// a exists here, but number has gone out of scope
	a = 5;
}
// a has gone out of scope
```
There is also a global scope, which is the block outside the main function. This is just essentially what rust does and explains really well.