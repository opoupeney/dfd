.. _angular-expression-label:

Angular Expressions
===================

Many DreamFace graphical controls use Angular Expressions to define labels or content. Whenever you see a value in
single quotes, for example 'Button' or when a property requires a *true* or *false* value you can use an
:term:`Angular expression`.

Like javascript expressions, Angular expressions can contain any set of literals (text inside single quotes), scope
variables, operators, or expressions that evaluate to a single value. The value can be a number, a string, or a logical
value (true or false).

Angular expressions evaluate to one of the three different kinds of single value :

* **Logical** expressions evaluate to single boolean value of *true* or *false*
* **Arithmetic** expressions evaluate to a number, for example if the expression is ((2+3) * 20 / 4) it would evaluate to 25
* **String** evaluates to a character string, for example 'Save' or '64 West 23rd St.' or 'This or ' + 'that' would evaluate to *This or that*


Expressions can be a combination of the above types of expressions :

**Example 1:**

if x = 16 (in DreamFace you could set the variable as follows $scope.x = 16, in the Script editor associated with the current View)
then try the following expression:

'We have ' + x + ' points; only ' + (25 - x) + ' left to reach 25' would evaluate to

--> *We have 16 points; only 9 left to reach 25*

|

**Example 2:**

if myName = 'Fred' (in DreamFace you could set the variable as follows $scope.myName = 'Fred', in the Script editor
associated with the current View) then try the following expression:

'My Name is ' + myName    This expression would evaluate to:

--> *My Name is Fred*

|

Samples
^^^^^^^

For more examples see Sample Angular Expressions in the Samples Gallery

* Samples Gallery Video (1-2 minutes)

* Samples Gallery Link sampleAngularExpressions

|

Additional Resources
^^^^^^^^^^^^^^^^^^^^

For more information on Angular Expressions consult the `Angular Documentation <https://docs.angularjs.org/guide/expression>`_

Angular Expression `Cheatsheet <https://docs.angularjs.org/guide/expression>`_

|
|
