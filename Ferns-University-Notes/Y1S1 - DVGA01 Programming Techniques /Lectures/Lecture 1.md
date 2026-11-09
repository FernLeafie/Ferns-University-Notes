## What Is Programming
Programming is giving instructions to a computer for it to execute
- Often done in computer programmes
- Websites, databases, video games, simulations etc.
Why learn programming?

Computers are everywhere and are just getting more common
- IoT, smart grid/cities, self driving vehicles
- Artificial intelligence (bleh, gross)

What is a computer?
Most things that have a processor and are programmable. Not just computer programmes, but embedded systems, industrial machines, and whatnot


> [!NOTE] Von Neuman
> Computers independant of type consists of three parts:
>
> > [!NOTE] Processor
> > Central processing unit. The computers "brain". Calculates and coordinates
>
> > [!NOTE] Memory
> > Primary
> > Fast, but temporary. RAM.
> > Secondary
> > Slow, but permanent. Hard drive.
>
> > [!NOTE] In and Out
> > Devices that feed in, or feed out data. Mice, keyboards, screens, monitors.


Files are stored on devices in a filesystem hierarchy

Operating systems
- In the beginning programmes were run directly on the computer
- Now days there's an operating system between programmes and hardware

The programming code that the processor understand is hard to read, machine code
```asm
xor ebp, ebp
mov r9, rdx
pop rsi
mov rdx, rsp
and rsp, 0xfffffffffff0
push rax
```
So we write in a simpler language, that is compiled into machine code, which the computer understands, an intermediary language
```c
int main() {
	printf("Hello World");
	return 0;
}
```

We will use the programming language C
- A high level language, that compiles to machine code
  (as it is abstracted from what the processor reads)
- Designed at AT&T Bell Laboratories by Dennis Ritchie 1969–1973
- A procedural programming language, which means the program is comprised of one or more functions
- C is one of the most used programming languages throughout time
	- Many other languages are based on C

The courses contents
- Computers components and functions
- Basic data types, syntax, and semantics
- Iteration and selection
- Vectors and text
- Functions and modularity
- Sorting and searching
- Memory management and pointers
- Compound data types and file management

Learning programming requires lots of practice
- Course information has the simplest exercises
  more simple exercises exist in the course literature
- When you're done with all of those, move onto
  https://open.kattis.com
- Solve exercises continuously during the course

The tenta will be a practical tenta
- Same types of exercises as in the course
- Done on a computer, individually, surveilled
- Old tenta are somewhat relevant, more on that as they approach

Labs
Solved in pairs and showed to an adviser
- Three different
	- Lab 1 - exercises in Autolab
	- Lab 2 - vehicle register
- See canvas for deadlines
	- Never mind, verbal examination at the end of the semester

Plagiarism
Plagiarism is strictly forbidden
- Applies to both code and report
- We have strong systems to find plagiarism
You're allowed to ask for *conceptual help*, but copying programming code isn't allowed

Programming is mostly practical
Practice and practice a lot

Exercises on online platforms
- Kattis
- Codeforces
- CodeChef

https://hub.cse.kau.se
- Log in with KauID
- Create a text file, not C console
- Rename the file
	- should end in `.c`
	  no shit
- File -> New Launcher
	- Choose terminal
	- Wowee linux terminal

