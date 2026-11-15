Exercise 1: Build a small C program

Write a Makefile for this project:
text

project/├── src/│   ├── main.c│   ├── math.c│   └── math.h└── Makefile

Requirements:

    Compile src/main.c and src/math.c into object files in a build/ directory.
    Link the objects into build/calculator.
    If either .c file changes, rebuild its object file and relink the program.
    If src/math.h changes, rebuild both object files and relink.
    Create build/ automatically if it doesn’t exist.
    Provide all and clean targets. all should build the program; clean should remove the build/ directory.
    Make all and clean phony targets.

Assume gcc is available. You don’t need to write the C files—focus on the Makefile.
