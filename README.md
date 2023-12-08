# Lab 11 - Grammar in ANTLR

This repository contains tasks related to grammar implementation using ANTLR.

## About ANTLR

ANTLR (ANother Tool for Language Recognition) is a powerful parser generator that can be used for a wide range of language processing tasks, including building parsers, interpreters, compilers, and more. It facilitates the creation of grammar-based tools by generating parsers for input languages.

### Tasks

### Task 1: ANTLR Commands for Expr.g4

To execute Task 1 related to Expr.g4, follow these steps:

1. Navigate to the 'tour' directory:
    ```bash
    cd tour
    ```

2. Generate the lexer and parser using ANTLR for Expr.g4:
    ```bash
    antlr4 Expr.g4
    ```

3. Check the generated Java files for Expr:
    ```bash
    dir Expr*.java
    ```

4. Compile the generated Java files for Expr:
    ```bash
    compile Expr*.java
    ```

5. Run the program with the generated parser and a test input file t.expr:
    ```bash
    grun Expr prog -gui t.expr
    ```


### Task 2: Generating Parsers with ANTLR for LabeledExpr.g4

To generate parsers using ANTLR for LabeledExpr.g4, follow these steps:

1. Change directory to `calc`:
    ```bash
    cd calc
    ```

2. Generate parser without listener and with visitor:
    ```bash
    antlr4 -no-listener -visitor LabeledExpr.g4
    ```

3. Check generated Java files:
    ```bash
    dir LabeledExpr*.java
    ```

4. Compile generated files with Calc.java:
    ```bash
    javac Calc.java LabeledExpr*.java
    ```

5. Execute the program with a test input file t.expr:
    ```bash
    java Calc t.expr
    ```

Follow these sequential commands to generate parsers using ANTLR for LabeledExpr.g4.


## Contributors

- [Muhammad Ashhub Ali](https://github.com/NightWalker7558)
- [Ahmad Zafar](https://github.com/Arch-Frost)
- [Adeel Ahmad](https://github.com/itsAdee)
- [Abdul Arham](https://github.com/a-arham-x)
