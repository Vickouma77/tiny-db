# tiny-db

Writing sqlite clone from scratch in C.

## core
- `Interface` - the main interface to the database.
- `SQL Command Processor` - processes SQL commands and translates them into actions on the database.
- `Virtual Machine` - executes the bytecode generated by the SQL Command Processor.

## SQL Compiler
- `Tokenizer` - tokenizes SQL statements for the parser.
- `Parser` - parses SQL statements and generates an abstract syntax tree (AST).
- `Code Generator` - generates bytecode from the AST.

## Backend
- `B-Tree` - a B-Tree implementation for storing data.
- `Pager` - manages the database file and provides a way to read and write pages.
- `OS Interface` - provides an interface to the operating system for file I/O.

## Accessories
- `Utilities` - various utility functions and classes.
- `Tests` - unit tests for the database.

## Architecture
![sqlite architecture ](assets/images/arch1.gif)

## Build
- `Makefile` - the build system for the project.

## Documentation
- `README.md` - this file.