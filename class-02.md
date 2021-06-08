# HTML Text, CSS Introduction, and Basic JavaScript Instructions

&nbsp;


## HTML Text

### Key Terms

Term | Definition
----- | -----
white space collapse | The process by which a browser ignores unnecessary white space and condenses the information accordingly.
empty elements | unique HTML tags that do not require a closing tag.

&nbsp;


### Structural versus Semantic Markup
&nbsp;


**Structural Markup**

>Organizes elements into a heirarchy of information.

&nbsp;


**Semantic Markup**
>Provides additional context for which information within an element is important, emphasized, edited, abbreviated, and more. Many semantic markup tags alert screen readers to convey information in specific ways.

&nbsp;

### Key Semantic Markup Tags

Tag | Useage
----- | -----
`<em>` | italics or emphasis
`<strong>` | bold or emphasis
`<q>` | short quote within a paragraph
`<abbr>` | designates an abbreviation
`<cite>` | designates a cited work (italicizes)
`<dfn>` | used to denote the first use of a new term
`<address>` | can be used to include website author's contact information
`<del>` | used to markup information that has been deleted (strikethrough)
`<ins>` | used to markup new content added to the document (underline)
`<s>` | denotes data that is no longer accurate

&nbsp;

## CSS Introduction

Term | Definition
----- | -----
selector | the initial part of a CSS rule that identifies *which* element will be affected by the CSS code.
declarations | the second part of a CSS rule. Identifies *how* the element will be presented or affected by the CSS code
property | defines *what* will be changed within the element (ie color, position, font, etc)
value | specifies *how much* or *to which setting* the property will adhere

&nbsp;

### External versus Internal CSS

**External CSS**
>A CSS reference instructing the browser to retrieve CSS styles from a stylesheet located outside the HTML document.

&nbsp;

**Internal CSS**
>CSS code written directly into the HTML document, within the element to which it applies.

***NOTE: External stylesheets are preferred and considered industry standard.***

&nbsp;

## Basic JavaScript Instructions

### Key Concepts

- JavaScript relies on script, or step-by-step instructions on how to gather, return, or interact with data. Each of these series of steps is called a **STATEMENT**.
- JavaScript is case sensitive.
- Statements begin on a new line.
- Statements encapsulated by `{ }` form **CODE BLOCKS**.
- 
----------
&nbsp;

- To **DECLARE** the variable is to assign it a name
>Example: `let example;`
&nbsp;
- In the above example, `let` is a JavaScript keyword or a built-in cue that JavaScript will recognize. `example` is our variable, which we have now assigned a unique identifying name or identifier.
- The use of camelCase is industry standard in naming variables with more than one word.
- Programmers often comment out notes regarding the code. This code will not be read or displayed on the browser. Longer comments are enclosed within the `/* */` symbols. Single-line comments are denoted using `//`.
- A variable can **NOT** begin with a number.
- Do **NOT use a - or . when naming a variable.
- You can **NOT** use a keyword within the name of a variable.

----------
&nbsp;

- To **ASSIGN A VALUE** to a variable, you need to state what information will be stored or substituted whenever the variable name is listed within the code.
- Variable names should give clear indication as to what data will be collected.
- An **ASSIGNMENT OPERATOR** is a symbol used to denote the phrase **can be understood to mean**. Be careful: An `=` as an assignment operator does not mean the same as a mathematical = symbol.
- The value of a variable may evolve throughout the code depending on the statements performed.
- If a variable has not been assigned a value, it is considered **UNDEFINED**.

-------
&nbsp;
- Numeric data describes data comprised of numbers.
- String data describes data comprised of text. Strings are written as: `'example'` 
- A **BOOLEAN** can be either true or false.
- Escaping is a technique used to instruct JavaScript to temporarily ignore a symbol or punctuation. This allows a string to contain punctuation without confusing the process of operations.

----------
&nbsp;

- An **ARRAY** stores a list of related values.
- Separate array values with `,`
- Encapsulate array values within `[ ]` when using writing an **ARRAY LITERAL**
- Arrays can store different data types (string, numeric, boolean)
- An **ARRAY CONSTRUCTOR** uses the `( )` symbols to contain values.
- Array literal is the preferred method.
- Array values are automatically assigned a number, starting with zero, and treated like a numbered list.
- The `length` keyword refers to the number of items or values within an identified array.

 ----------
&nbsp;

## Decisions and Loops

&nbsp;

**Evaluation of a Condition**
>Checks statements for a true/false comparison value.

&nbsp;

**Conditional Statement**
>Based on *if, then, else* instructions, which affect the order in which steps or statements are performed.

&nbsp;

### Key Comparison Operators

Operator | Meaning
----- | -----
`==` | is equal to
`!=` | is not equal to
`===` | (preferred) compares equal value **AND** same data type (string/numeric)
`!==` | evalutates two values to verify value and data type are **NOT** the same
`>` | greater than (numeric data)
`<` | less than (numeric data)
`>=` | greater than or equal to (numeric data)
`<=` |  less than or equal to (numeric data)

&nbsp;

**Anatomy of an Expression with Comparison Operators**

**Example 1**
>`(operand1 >= operand2)`

&nbsp;

- The conditional expression begins and ends with `( )`
- The values or variables being evaluated are known as **OPERANDS**
- The symbol between them is the **COMPARISON OPERATOR**

**Example 2**
>`((operand1 * operand2) !== (example1 + example2))`

&nbsp;

In this example we can see that the operands on either side of the `!==` operator are actually expressions themselves. The individual expressions will return a single value, which can then be compared in the same way as **EXAMPLE 1**.

--------

### Logical Operators

&nbsp;

- Another type of operator is a **LOGICAL OPERATOR**.
- The difference between a logical and comparison operator is that a logical operator is used to compare the results of multiple comparison operators to reach a `true` or `false` outcome.

### Key Logical Operators

Operator | Useage
----- | -----
LOGICAL AND | Evaluates more than one condition on either side to compare values for `true`.
LOGICAL OR | At least one condition must evaluate as `true` to return `true`, even if the other expression evaluates as false. In other words, 1 out of 2 expressions must be true to return `true`.
LOGICAL NOT | Inverts a Boolean value. A `false` return then becomes `true`.

&nbsp;

**NOTE: Computers read logical expressions from right to left.**

&nbsp;

>If the first comparison expression in a LOGICAL AND evaluates to `false`, the entire logical expression returns as `false`, and no additional information in the expression will be evaluated, as the expression can no longer return a `true && true`.

&nbsp;

>If the first comparison expression in a LOGICAL OR evaluates to `true`, the entire logical expression returns as `true`, and no additional information in the expression will be evaluated, as the condition of at least one conditional expression resulting in a `truthie` has been met.

------------
&nbsp;


## If Statements
&nbsp;


### Key Concepts

- `if` is a JavaScript keyword that signals an evaluation of a condition. If the condition returns `true`, the steps following the condition will be read by the computer and performed.
- The following steps are statements within code blocks contained in the `{ }` symbols.
- When the condition returns a `false` the following steps will not be performed.

&nbsp;

## If - Else Statements
&nbsp;

### Key Concepts

- When the `if` statement resolves to `false`, an `else` statement is used to perform alternative statements or steps.

&nbsp;


**Please Note: This information is a summary derived from Jon Duckett's *HTML & CSS* and *JAVASCRIPT & JQUERY.***
