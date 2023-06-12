# SICP-Interpreter

This is a simple interpreter for the Scheme programming language, based on the book "Structure and Interpretation of Computer Programs" (SICP). It provides functionality to evaluate Scheme expressions, define variables and procedures, and perform basic operations.

## Features
Evaluation of self-evaluating expressions, such as numbers and strings.
Evaluation of variables by looking up their values in the environment.
Quoting of expressions to treat them as literal data.
Assignment of values to variables using the set! construct.
Definition of variables and procedures using the define construct.
Evaluation of conditional expressions using the if construct.
Evaluation of sequences of expressions using the begin construct.
Evaluation of cond expressions, which are a generalization of if.
Evaluation of procedure applications.
Support for primitive procedures, such as car, cdr, cons, and +.
Creation and execution of compound procedures.
Recursive evaluation of procedures and expressions.

## Usage
The interpreter provides a driver-loop function that reads Scheme expressions, evaluates them, and displays the results. To start the interpreter, execute the following code:

***(driver-loop)***

You will be prompted with ;;; M-Eval input:. Here, you can enter Scheme expressions and see their evaluated results displayed as ;;; M-Eval value:. The interpreter supports various built-in procedures, as well as user-defined procedures and variable definitions.

## Examples
Here are some examples of valid Scheme expressions that you can try in the interpreter:

### Arithmetic operations:

***(+ 2 3)   ; Addition
(- 5 2)   ; Subtraction
(* 4 6)   ; Multiplication
(/ 10 2)  ; Division***

### Variable definitions and assignments:

***(define x 5)
(set! x 10)
x***

### Conditional expressions:

***(if (> 5 3) 'true 'false)***

### Procedure definitions and applications:

***(define (square x) (* x x))
(square 4)***

### Recursive procedures:

***(define (factorial n)
  (if (= n 0)
      1
      (* n (factorial (- n 1)))))
(factorial 5)***

## Limitations
This interpreter is a simplified implementation and may not support all features and advanced constructs of Scheme. It is primarily designed for educational purposes and as a starting point for understanding language interpretation.

## Acknowledgments
The core logic and code structure of this interpreter are based on the concepts and examples presented in the book "Structure and Interpretation of Computer Programs" by Harold Abelson and Gerald Jay Sussman.
