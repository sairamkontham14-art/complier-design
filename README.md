SAI RAM KONTHAM

CSE E

RA2311003050299

**1.LEXICAL-ANALYSER:**
# Lexical Analyzer using Python

## Description
This project is a simple lexical analyzer implemented using Python.  
It identifies tokens such as keywords, identifiers, operators, separators, and numbers from the given source code.

## Features
- Identifies keywords
- Identifies identifiers
- Identifies operators
- Identifies separators
- Identifies numbers

## Technologies Used
- Python
- VS Code

## How to Run the Program
1. Open the project folder in VS Code
2. Open `lexical_analyzer.py`
3. Run the file using:
   - Run button ▶️  
   - OR press `Ctrl + F5`
   - OR use terminal:
     ```
     python lexical_analyzer.py
     ```

## Output
The output is displayed in the terminal showing token type and value.

**2.PARSING-TABLE:**
# Parsing Table Construction

## Aim
To construct an LL(1) parsing table for a given grammar.

## Theory
LL(1) parsing table helps in predictive parsing by selecting productions using input symbols.

## Program
Implemented using Python.

## Output
Displays the LL(1) parsing table.

**3.ELIMINATION-OF-AMBIGUITY:**
# Elimination of Ambiguity, Left Recursion and Left Factoring

## Aim
To eliminate ambiguity, left recursion, and perform left factoring in a given grammar.

## Theory
Ambiguous grammars produce multiple parse trees. Left recursion and common prefixes cause problems in top-down parsing. These are removed to make the grammar suitable for parsing.

## Algorithm
1. Identify left recursive productions.
2. Eliminate left recursion.
3. Identify common prefixes.
4. Apply left factoring.

## Program
Implemented using Python.

## Output
Displays the modified grammar after eliminating left recursion and left factoring.

**4.NFA-TO-DFA:**
# NFA to DFA Conversion

## Aim
To convert a given Non-Deterministic Finite Automaton (NFA) into an equivalent Deterministic Finite Automaton (DFA).

## Theory
NFA to DFA conversion is done using the subset construction method where each DFA state represents a set of NFA states.

## Algorithm
1. Start with the initial NFA state.
2. Generate all possible subsets of NFA states.
3. For each subset and input symbol, compute transitions.
4. Mark final states containing NFA final state.

## Program
Implemented using Python.

## Output
The program displays DFA states, transitions, and final states.

**5.FIRST-AND-FOLLOW:**
# FIRST and FOLLOW Computation

## Aim
To compute FIRST and FOLLOW sets for a given context-free grammar.

## Theory
FIRST and FOLLOW sets are used in syntax analysis to construct predictive parsing tables.

## Algorithm
1. Define grammar productions.
2. Compute FIRST for all non-terminals.
3. Compute FOLLOW using FIRST information.
4. Display the sets.

## Program
Implemented using Python.

## Output
Displays FIRST and FOLLOW sets for the grammar.

**6.REGULAR-EXPRESSION-TO-NFA:**
## Regular Expression to NFA

### Aim
To convert a given Regular Expression into a Non-Deterministic
Finite Automaton (NFA).

### Description
This program takes a regular expression as input and constructs
an equivalent NFA.

### Algorithm
1. Read the regular expression
2. Create start state
3. Generate transitions for each symbol
4. Mark final state as accept state

### Language Used
Python

### Output
Displays start state, accept state, and NFA transitions.

**Lab 7: SHIFT REDUCE PARSING**
Aim
To implement Shift Reduce Parsing using Python.

Description
Shift Reduce Parser is a bottom-up parsing technique used in compiler design.

Algorithm
Shift input symbols into stack
Reduce using grammar rules
Accept if stack contains start symbol
How to Run
Open Codespaces
Run: python3 shift_reduce.py
Output
Displays shift and reduce operations step by step.Displays start state, accept state, and NFA transitions.

Lab 8: LEADING and TRAILING

Aim
To compute LEADING and TRAILING of a grammar.

Description
This program finds the starting and ending terminals for each non-terminal.

Output
Displays LEADING and TRAILING sets.

**Lab 9: LR(0) ITEMS COMPUTATION**

Aim
To compute LR(0) items for a given grammar.

Description
This program generates LR(0) items by inserting a dot (.) at all possible positions in each production.

Algorithm
Take grammar productions
For each production:
Insert dot at every position
Display all LR(0) items
Input
Grammar: E->E+T E->T T->T*F T->F F->(E) F->i

Output
All possible LR(0) items

Result
Successfully generated LR(0) items.

**Lab 10: INTERMEDIATE CODE GENERATION(Postfix & Prefix)**

Aim
To convert infix expression into postfix and prefix expressions.

Description
This program converts infix expressions using stack-based method.

Algorithm
Use stack for operators
Follow precedence rules
Convert infix to postfix
Reverse logic for prefix
Input
Infix expression (e.g., A+B*C)

Output
Postfix and Prefix expressions

Result
Successfully converted infix to postfix and prefix.

**Lab 11: INTERMEDIATE CODE GENERATION**

Aim
To generate Quadruple, Triple and Indirect Triple representations.

Description
This program converts an expression into intermediate code forms.

Algorithm
Identify operators and operands
Apply precedence rules
Generate temporary variables
Form Quadruple, Triple and Indirect Triple
Input
Expression (e.g., A+B*C)

Output
Quadruple, Triple and Indirect Triple

Result
Successfully generated intermediate code representations.

**Lab 12: SIMPLE CODE GENERATOR**

Aim
To generate intermediate code from an expression.

Description
This program converts an infix expression into three-address code.

Algorithm
Identify operators and operands
Apply precedence rules
Generate temporary variables
Produce intermediate code
Input
Expression (e.g., A+B*C)

Output
Three-address code

Result
Successfully generated intermediate code.

**Lab 13: IMPLEMENTATION OF DIRECTED ACYCLIC GRAPH (DAG)**

Aim
To construct a Directed Acyclic Graph (DAG) for a given expression and perform basic code optimization.

Objective
To identify common subexpressions and eliminate redundant computations using DAG.

Theory
A Directed Acyclic Graph (DAG) is a graph with no cycles. It is used in compiler design for optimizing expressions by representing computations efficiently.

Each node represents an operator or operand.
Leaf nodes represent operands.
Internal nodes represent operators.
Common subexpressions are stored only once and reused.
Algorithm
Read the input expression.
Convert the infix expression into postfix form.
Initialize an empty stack.
For each symbol in postfix expression:
If operand → push to stack.
If operator → pop two operands and create a node.
Before creating a node, check if the same node already exists:
If yes → reuse it.
If no → create a new node.
Store all nodes in DAG.
Display DAG nodes.
Input
Arithmetic expression (e.g., A+B*C)

Output
DAG representation showing operators and operands.

Example
Input: A+B*C

Output: ('*', 'B', 'C') ('+', 'A', (B * C))

Result
Successfully constructed a Directed Acyclic Graph and optimized the expression by eliminating common subexpressions.

Applications
Code optimization
Common subexpression elimination

**Lab 14: GLOBAL DATA FLOW ANALYSIS**

Aim
To perform global data flow analysis using reaching definitions.

Description
This program computes GEN, KILL, IN, and OUT sets for a set of statements.

Theory
Data flow analysis tracks how data moves through a program. Reaching definitions determine which assignments reach a program point.

Algorithm
Read program statements
Compute GEN and KILL sets
Initialize IN and OUT sets
Iterate until no changes occur
Display results
Input
Set of assignment statements

Output
GEN, KILL, IN and OUT sets

Result
Successfully performed global data flow analysis.

**Lab 15: STORAGE ALLOCATION STRATEGY (Stack Allocation)**
Aim
To implement stack storage allocation.

Description
This program demonstrates stack allocation using push and pop operations.

Theory
Stack allocation follows Last In First Out (LIFO) principle. It is used for managing function calls and local variables.

Algorithm
Initialize empty stack
Perform push operation
Perform pop operation
Display stack contents
Input
User choice and values

Output
Stack operations results

Result
Successfully implemented stack allocation.
