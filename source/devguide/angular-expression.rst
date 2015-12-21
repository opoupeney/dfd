.. _angular-expression-label:

Angular Expression
==================

Many DreamFace graphical controls use Angular Expressions to define labels or content. Whenever you see a value in
single quotes, for example 'Button' or when a property requires a *true* or *false* you can use an :term:`Angular expression`.

Like javascript expressions, Angular expressions can contain any set of literal text, variables, operators, or expressions
that evaluate to a single value. The value can be a number, a string, or a logical value (true or false).

AngularJS expressions are written inside double braces are usually written inside {{ expression }}.

AngularJS expressions binds data to HTML the same way as the ng-bind directive.

AngularJS will "output" data exactly where the expression is written.

AngularJS expressions are much like JavaScript expressions: They can contain literals, operators, and variables.

Example {{ 5 + 5 }} or {{ firstName + " " + lastName }}


There are two types of expressions:

* expressions that assign a value to a variable
* expressions that evaluate to a single value

For example, the expression

x = 3

is an expression that assigns the value 3 to the variable x and the expression also evaluates to 3. This type of expression
uses the operator '=' to assign a value. Javascript has many operators that can be used in expressions. A detailed list of
javascript operators is provided below.


The second type of expression evaluates to a single value, for example

2 + 1

evaluates to the value 3.


JavaScript provides three different kinds of expressions:

* **Logical** expressions evaluate to *true* or *false*
* **Arithmetic** expressions evaluate to a number, for example y = 9 (would evaluate to 9) or ((2+3) * 20 / 4) would evaluate to 25
* **String** evaluates to a character string or text, for example "Save" or "64 West 23rd St." or "This or " + "that " would evaluate to *This or that*

Expressions can be a combination of the above types of expressions, for example:

if x = 16 (in DreamFace you could set the variable as follows $scope.x = 16, in the Script editor associated with the current View)
then try the following expression:

'We have ' + x + ' points; only ' + (25 - x) + ' left to reach 25' would evaluate to

*We have 16 points; only 9 left to reach 25*

|

Conditional Expressions
^^^^^^^^^^^^^^^^^^^^^^

A conditional expression can have one of two values based on a condition. The syntax is

(condition) ? val1 : val2

If condition is true, the expression gets the value of val1, otherwise it is gets the value of val2. Conditional expressions
can be used to test the value of a variable, for example:

(temp > 100) ? "hot" : "cold"

This expression tests the value of the variable temp. If it is greater than 100 the expression will evaluate to the value "hot"
otherwise it will evaluate to "cold".

|

Operators
^^^^^^^^

Any Javascript operators can be used in expressions. See a Javascript reference for a full list of javascript operators.

|
|
