.. _angular-expression-label:

Angular Expression
==================

Many DreamFace graphical controls use Angular Expressions to define labels or content. Whenever you see a value in
single quotes, for example 'Button' or when a property requires a *true* or *false* you can use an :term:`Angular expression`.

Like javascript expressions, Angular expressions can contain any set of literal text, variables, operators, or expressions
that evaluate to a single value. The value can be a number, a string, or a logical value (true or false).

AngularJS expressions are written inside double braces {{ expression }}.

AngularJS expressions binds data to HTML the same way as the ng-bind directive.

AngularJS will "output" data exactly where the expression is written.

AngularJS expressions are like JavaScript expressions: They can contain literals, operators, and variables.

Example {{ 7 + 3 }} or {{ firstName + " " + lastName }}

AngularJS expressions do not support conditionals, loops, and exceptions, while JavaScript expressions do.

AngularJS expressions support filters, while JavaScript expressions do not.


JavaScript provides three different kinds of expressions:

* **Logical** expressions evaluate to *true* or *false*
* **Arithmetic** expressions evaluate to a number, for example y = 9 (would evaluate to 9) or ((2+3) * 20 / 4) would evaluate to 25
* **String** evaluates to a character string or text, for example "Save" or "64 West 23rd St." or "This or " + "that " would evaluate to *This or that*

Expressions can be a combination of the above types of expressions, for example:

if x = 16 (in DreamFace you could set the variable as follows $scope.x = 16, in the Script editor associated with the current View)
then try the following expression:

'We have ' + x + ' points; only ' + (25 - x) + ' left to reach 25' would evaluate to

*We have 16 points; only 9 left to reach 25*

literal will be in single quotes 'My Name is '

1234 | number:2



Additional Resources
^^^^^^^^^^^^^^^^^^^

For more information on Angular Expressions consult the `Angular Documentation <https://docs.angularjs.org/guide/expression>`_

Angular Expression `Cheatsheet <https://docs.angularjs.org/guide/expression>`_

|
|
