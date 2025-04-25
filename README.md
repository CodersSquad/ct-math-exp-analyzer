Math Expressions Analyzer
=========================

This is the time to apply what you have learned in the Computational Theory Class.
You will implement a math expression analyzers that will validate simple mathematical expressions. Below the criteria you need to consider.

- Support for balanced parenthesis `()`
- Supported operators:
  - `*` for multiplications
  - `**` for power (exponentiation) 
  - `/` for divisions
  - `+` for additions
  - `-` for subtractions
- Your program should support real numbers `(0, 0.1, 1.22, -1.23)`


Deliverables
------------
- A pdf document with the following content:
  - Presentation Page
  - Description of the project
  - Context-Free Grammar(s), Push-Down Automata or Finite Automata (any diagram or description of the automatas, language or grammar you designed)
  - Derivation Trees (in case you want to give an example)
  - Program's design process (diagrams, code snippets, etc)
  - Sample executions and output
  - Conclusions (one per team member)
- HOWTO.md with details on how to compile and run your program
- Main program should be impleted on [`math-exp-analyzer.go`](./`math-exp-analyzer.go)


How your program will be tested
-------------------------------

This is going to be simple, your program will be run as follows:

```
go run math-exp-analyzer.go -i expressions.txt -o results.txt
```

There's an [`expressions.txt`](`expressions.txt`) document sample file that you can use to test your program.

Your `results.txt` file should look as follows:

```
Expression 1: (6**6 / 2)      -  Valid
Expression 2: (6*6 / )        -  Invalid
Expression 3: (6*6 / 3)*(4)   -  Valid
.
.
.
.
```


