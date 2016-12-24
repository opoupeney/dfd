Dynamic CSS Class
=================

The Dynamic Class is a CSS class that will be added to the graphical control if an Boolean Angular Expression is verified.

|

.. image:: ../../images/devguide/dfx-prop-style-dynamic.png



**Value:** - **expression** Name of CSS Class followed by an boolean expression that sets a style if the expression evaluates to *true*.

**Default:** - *None*

**Notes**


Consider the following CSS class:
::

    .RedMessage {
         color: red
    }

    Dynamic class could be an angular expression like

    *RedMessage: my_variable<0*


--- or another example might be ---

::

   .RedValue {
       color: red;
   }
   .GreenValue {
       color: green;
   }

   Dynamic class could be an angular expression like

   RedValue: my_variable<0; GreenValue: my_variable>=0


depending on the value of my_variable, the component will have the RedValue class and not the DOM.

|