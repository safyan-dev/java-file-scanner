# Java Code Scanner
A simple Java Code Scanner is a Java Swing application designed to analyze Java source code files and extract various elements such as keywords, identifiers, literals, operators, and special symbols. It provides a graphical user interface for users to input the file path, browse the file, and scan the code for different syntax elements.

## Getting Started
To use this application, make sure you have Java installed on your system. I used Eclipse IDE for Java to build this.

## How to Use
1. Launch the application.
2. Click on the "Browse" button to select the Java source code file you want to analyze.
3. Click on the "Scan" button to analyze the code.
4. The application will display the results in two sections:
5. Token Table: Displays various Java syntax elements such as keywords, identifiers, operators, and special symbols with their corresponding line numbers.
6. Literal Table: Displays literals (numeric and string literals) with their line numbers.

## Features
1. Identifiers: Identifiers (variable names, method names, class names, etc.) are identified and displayed in the Token Table.
2. Keywords: Special Java keywords are recognized and displayed in the Token Table.
3. Literals: Numeric and string literals are identified and shown in the Literal Table
4. Operators: Various Java operators like arithmetic operators, relational operators, assignment operators, and conditional operators are recognized and displayed in the Token Table.
5. Special Symbols: Parentheses, braces, square brackets, commas, periods, semicolons, and colons are recognized and displayed in the Token Table.

## Example
Upload a file that includes a java code snippet.
```
public class Example {
    public static void main(String[] args) {
        int num1 = 10;
        int num2 = 20;
        int sum = num1 + num2;
        System.out.println("Sum is: " + sum);
    }
}
```
The Literal Table will display:

```
Token        Desc                  LineNo
public       Spectial keyword      1
class        Spectial keyword      1
Example      Indentifier           1
{            Symbol                1
public       Spectial keyword      2
static       Spectial keyword      2
void         Spectial keyword      2
main         Indentifier           2
(            Symbol                2
String[]     Indentifier           2
args         Indentifier           2
)            Symbol                2
{            Symbol                2
int          Spectial keyword      3
num1         Indentifier           3
=            AssignmentOperator     3
10           PositiveInteger        3
;            Symbol                3
int          Spectial keyword      4
num2         Indentifier           4
=            AssignmentOperator     4
20           PositiveInteger        4
;            Symbol                4
int          Spectial keyword      5
sum          Indentifier           5
=            AssignmentOperator     5
num1         Indentifier           5
+            ArithmaticOpeartor     5
num2         Indentifier           5
;            Symbol                5
System.out   Indentifier           6
.println     Indentifier           6
(            Symbol                6
"Sum is: "   Symbol                6
+            ArithmaticOpeartor     6
sum          Indentifier           6
)            Symbol                6
;            Symbol                6
}            Symbol                7
}            Symbol                8
```
