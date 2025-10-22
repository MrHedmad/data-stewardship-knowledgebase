# Programming

Knowing the basics of [:beginner: programming](https://en.m.wikipedia.org/wiki/Computer_programming) is essential for any data steward.
Indeed, most modern data is captured and processed by computers.
Additionally, the [:curly_loop: FAIR Principles]() are inherently enabling _machines_ (and, therefore, humans) to access more data, more accurately, transparently and quickly.

Knowing the basics of computer programming also allows you to make sense of the main limitations inherently embedded in the way that computers process information.
This, in turn, allows you to understand the reasons behind many Research Data Management (RDM) choices.

There are massive amounts of resources available online which can be used to learn programming even to high standards as a self-taught students.
At the end of this page, you will not know programming, but you will be equipped with all the tools enabling you to learn it as quickly and efficiently as possible.

A data steward does not need advanced programming knowledge, such as that that a degree in computer science might net you, but, according to the [:curly_loop: data steward competence framework](topics/basics/competences.md), a data steward should be able to:
- Develop and prototype specialised data handling procedures for specific needs.
- Develop and manage infrastructure for data handling and analysis, with emphasis on big data, data streaming and batch processing, while ensuring provenance and FAIRness.
- Develop, deploy and operate data infrastructure, including data storage, while following data management policies, with specific attention to the implementation of FAIR principles.
- Analyse, collect and assess data to achieve organizational goals, such as quality assurance of the organizational system;

All of these tasks (and more!) require or benefit heavily from some programming and computer science knowlege.

## How computers process information
[:beginner: Computers](https://en.wikipedia.org/wiki/Computer) are composed of several basic components:
- A [:beginner: motherboard](https://en.wikipedia.org/wiki/Motherboard), which connects all other components together;
- A [:beginner: central processing unit](https://en.wikipedia.org/wiki/Central_processing_unit), or CPU, which performs basic arithmetic operations (such as sums, subtractions, and comparisons between numbers) at a very fast rate.
  A CPU's speed is measured in how many computations it can do in a second, in other words, its *frequency*.
  Modern CPUs can reach frequencies of more than 3 gigahertz (3 \* 10^9), meaning 3 giga-computations per second.
- A computer is made up of many different types of [:beginner: memory](https://en.wikipedia.org/wiki/Computer_memory).
  Some, like Random Access Memory (or RAM) are very fast but require constant power to retain information.
  Others, like Hard Disks or the more modern Solid State Drives (SSDs) retain information even without power and thus for longer periods of time.
- To be useful, a computer requires a way to interface with human operators.
  This means it need to display its results (output) and accept inputs from humans.
  The devices that allow this kind of operations are called [:beginner: Input/Output peripherals](https://en.wikipedia.org/wiki/Input/output), or simply "Input/Output" or IO.
  Examples are screens, keyboards and mice.

While these are the most basic parts of a computer, it is important to underline that many more are possible, depending on the scale, size and complexity of the tasks placed on the computers themselves.

Computers process information via the CPU.
The CPU may only perform basic operations: reading and writing to memory, adding values, subtracting them, comparing them, and a handful more.
While the number of instructions are very limited, carefully designing complex series of instructions allows computers to perform a huge number of tasks.
These series of instructions are called [:beginner: programs](https://en.wikipedia.org/wiki/Computer_program).

CPUs are hard-wired in such a way in which the pattern of high and low voltages applies to specific wires in them causes the result of one of these basic structures to appear in another set out output pins.
These differences in voltage are well described by binary numbers: either 0 for low voltage or 1 for high voltage.

CPUs can therefore only understand these patterns of 0s and 1s, causing them to perform one of their basic instructions.
Writing these 0s and 1s is a difficult, almost impossible task, so methods of *abstraction* were developed in order to translate programs written in languages that humans can understand back to a series of instructions that a CPU might execute.

For example, summing two numbers, written out as basic CPU instructions, might look like this:
```ascii
.code
main proc
   mov ax, @data
   mov ds, ax
   mov ah, 09h
   mov dx, offset message1
   int 21h
   mov ah, 1
   int 21h
   sub al, 30h 
   mov num1, al
   mov ah, 09h
   mov dx, offset message2
   int 21h
   mov ah, 1
   int 21h
   sub al, 30h
   mov num2, al
   add al, num1
   mov result, al
   mov ah, 0 
   aaa
   add ah, 30h
   add al, 30h
   mov bx, ax
   mov ah, 09h
   mov dx, offset message3
   int 21h
   mov ah, 2
   mov dl, bh
   int 21h
   mov ah, 2
   mov dl, bl 
   int 21h
   mov ah, 4ch
   int 21h
main endp
end main
```

This is the language of the CPU, or *machine code* (actually, it ASCII, but the two are very similar).
As you can see, this program (which, by they way, does not work) is almost impossible to decipher by anybody who is not an expert in computer science.

Abstraction programs have been designed to take some simpler language, such as `3 + 4` and translate it to the set of instruction above.
The two forms are identical in output, but wildly different in how easy they are to create.
These abstraction programs are called *programming languages*.

## Programming languages
There are many different kinds of programming languages.
Usually, they are subdivided into "high level" and "low level" languages: low level languages are closer to machine code, but provide programmers with a higher level of control on specifically what the CPU is doing at any one time, while high level languages are easier to use but restrict what the computer can do and, oftentimes, waste resources to provide programming simplicity.

When a computer is turned on, a small, hard-coded program is executed.
This program is called a [BIOS](https://en.wikipedia.org/wiki/BIOS) or, in modern computers, [UEFI](https://en.wikipedia.org/wiki/UEFI).
The main task performed by the BIOS/UEFI system is to activate another program, called the [Operating System](https://en.wikipedia.org/wiki/Kernel_(operating_system)), which in turn interfaces with all the systems attached on the motherboard, and allows to be a "mediator" between the hardware (e.g. the CPU or the monitor) and the programs that are executed on it.

The main way to interact with the Operating System is another program called a [:beginner: shell](https://en.wikipedia.org/wiki/Shell_(computing)), which in turn allows exploring the memory on the computer, execute programs, and more.
Shells accepts strings of text (typed with a keyboard) and output the results of the programs as text to the screen.

![Example of a bash shell](https://upload.wikimedia.org/wikipedia/commons/1/16/OpenBSD_ksh_Interaction.png)

Examples of operating systems are [Linux](https://www.kernel.org/), [Microsoft Windows](https://www.microsoft.com/it-it/windows/), [Mac OS](https://en.wikipedia.org/wiki/MacOS) and [Android](https://www.android.com/).
Examples of shells are [SH](https://en.wikipedia.org/wiki/Bourne_shell), [BASH](https://www.gnu.org/software/bash/) and [ZSH](https://www.zsh.org/). 
As BASH is the most popular and one of the oldest shells, most other shells follow in some way or another the conventions put forth by BASH.

The operating system might execute other programs when it starts, such as those showing a desktop, which allows manipulating visual programs, which can be more pleasing and easy to use than interacting with the shells.

The most basic programming language is the so-called shell scripting.
A shell script is simply a simple text file (`.txt`) with shell commands, one per each line.