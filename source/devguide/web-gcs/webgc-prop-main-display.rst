.. _webgc-main-display-label:

Display
=======

Display is a property to show or hide a :term:`GC`. If the value is *true* the GC is displayed. When the value is
*false* the GC is hidden.


|

.. image:: ../../images/devguide/dfx-prop-main-display.png


**Values:**

* **true** to display the field
* **false** to hide the field
* **boolean angular expression** that evaulates to *true* or *false*, for example, 5 > 2 would evaluate to *true* and 5 < 2 would evaluate to *false*.
* **$scope variable** (defined in the script of the View in the Script Editor, if not set the default will be *false*).

**Default:** *true*

**Notes:**

Check out the Samples Gallery and mini apps for more examples of Dynamic fields that show or hide using the Display property.

The value can either be a literal *true* to display the field or *false* to hide it, an angular expression that evaulates
to *true* or *false*, or  It is also possible to use a $scope variable (defined in the script of the View in the Script
Editor).

On the right hand side of the field you will see **...** indicating that help in defining expression is available.
Click on the *...** and a Expression Editor will be displayed, indicating existing scope variables and functions. You
can use scope variables as part of your angular expression, for example, myVar == 5, would evaluate the expression
using the value stored in the scope variable myVar, if equal to 5 the expression would evaluate to **true** and the text
would be displayed.

See :ref:`angular-expression-label`  for more help on Angular Boolean Expressions

|