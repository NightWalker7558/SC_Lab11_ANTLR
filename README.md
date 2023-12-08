# Lab 11 - Grammar in ANTLR

This repository contains tasks related to grammar implementation using ANTLR.

## About ANTLR

ANTLR (ANother Tool for Language Recognition) is a powerful parser generator that can be used for a wide range of language processing tasks, including building parsers, interpreters, compilers, and more. It facilitates the creation of grammar-based tools by generating parsers for input languages.

## Installation

To set up ANTLR, follow these steps:

1. **Download ANTLR:**
   - Download the ANTLR tool folder, named as `antler` in the repo.

2. **Place ANTLR Folder:**
   - Once downloaded, extract the contents of the ANTLR folder to a location of your choice. For instance, you might place it in the `D` drive (`D:\antlr`).

3. **Set CLASSPATH System Environment Variable:**
   - Create a new System Environment Variable named `CLASSPATH`.
   - Set its value to include the ANTLR JAR file. For example, `.;D:\antlr\antlr-4.13.1-complete.jar`.
     - This value includes the current directory (`.`) and the path to the ANTLR JAR file.

4. **Update Path System Variable:**
   - Edit the `Path` System Variable to include:
     - `%CLASSPATH%`
     - `D:\antlr`

   These additions allow Java to locate ANTLR classes and resources necessary for executing ANTLR-related commands and programs.

5. **Verify Installation:**
   - To verify that ANTLR is correctly installed, open a command prompt and type `antlr` or `java org.antlr.v4.Tool`. If the installation was successful, you'll see ANTLR's command-line help.

## Tasks

### Task 1: ANTLR Commands for Expr.g4

To execute Task 1 related to Expr.g4, follow these steps:

1. Navigate to the 'tour' directory:
    ```bash
    cd tour
    ```

2. Generate the lexer and parser using ANTLR for Expr.g4:
    ```bash
    antlr Expr.g4
    ```

3. Check the generated Java files for Expr:
    ```bash
    dir Expr*.java
    ```

4. Compile the generated Java files for Expr:
    ```bash
    javac Expr*.java
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
    antlr -no-listener -visitor LabeledExpr.g4
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
