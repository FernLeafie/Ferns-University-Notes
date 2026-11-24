Abstraction?
The ability to generalise code into generalised methods, or algorithms, to solve a problem, is what makes you good at programming and problem solving.
The ability to tweak a solution for one problem, to fit another problem. And for more complex problems, to be able to break it down into smaller solutions, so that multiple abstractions may be combined to solve the more complex problems.
This course will mostly cover algorithms on lists.

### Algorithms
We have two major types of algorithms: Mutating/Nonmutating algorithms.
The difference being that a Mutating one changes the original list, or mutates it, while a nonmutating one doesn't change the input.
All the names for algorithms here are mostly made up, but the principle behind them still exists, and it's more important to learn the methods behind it. The separation between mutating and nonmutating algorithms is often important.
### Nonmutating
#### Aggregation
Algorithms that preform a mathematical operation across the whole list, for example summation. And can be involved in operations such as averages, and standard deviations.
This is nonmutating.
```c
int acc = /*start*/;
for (int i = 0; i < n, i++) {
	acc = /*operation*/ list[i];
}
```
#### Traversal
Run a nonmutating function on all elements of a list. Can also be done with mutating
```c
for (...) {
	/*operation*/ list[i];
}
```
#### Selection
Conditionally run functions based on the contents of the index.
```c
for (...) {
	if (/*condition*/) {
		/*operation*/;
	} // else {}
}
```
A simple example would be printing out all odd numbers, or all values over a threshold.
If the operation is `break;`, we can go through a list till a certain condition is met.
If the operation is `continue;`, we can skip to the next iteration without executing the rest of the code in the loop. This can be used for negative selection, which can often be cleaner, so instead of nesting an operation in an if block `if (/*condition*/) {/*operation*/;}`, we can continue if the negative condition is met. `if (!/*condition*/) {continue;} /*operation*/; ` Often nice to not end up with layers of nested `if` statements.
### Mutating
There are a bunch of operations you can do on a list, with algorithms similar to the idea of traversal, but most can likely be improvised, or are too complex to do now.
#### Reversing
Reversing a list. We only need to go through half the list, as we have to swap each element, for the element on the opposite side. `list[i] ~ list[n-i-1]`
To not forget what value was in the first value we replace, we have to put it in a temporary other storage location, this is called a swap. XOR swap could be used 
```c
for (int i = 0; i < n/2; i++) {
	int tmp = list[i];
	list[i] = list[n-i-1];
	list[n-i-1] = tmp;
}
```
Here, like in whatever algorithm we have, we can generalise away whatever component we need for the purpose we need it for.
