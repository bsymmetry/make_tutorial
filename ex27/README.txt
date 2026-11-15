Exercise 2: Generate reports from input files

Write a Makefile for this project:
text

project/├── data/│   ├── north.csv│   └── south.csv├── templates/│   └── report.tpl└── Makefile

Assume a command-line program named reportgen works like this:
sh

reportgen --template TEMPLATE --input INPUT --output OUTPUT

Requirements:

    Generate out/north.html from data/north.csv, and out/south.html from data/south.csv.
    Each report depends on its corresponding CSV file and templates/report.tpl.
    Create out/ automatically if it doesn’t exist.
    Provide an all target that builds both reports, plus a clean target that removes out/.
    Use one pattern rule for generating the reports rather than writing a separate recipe for each file.
    Make all and clean phony targets.

Submit your two Makefiles, labeling them Exercise 1 and Exercise 2. I’ll review correctness, dependency tracking, target design, and any GNU make pitfalls.
