.. _webgc-main-binding-label:

Binding
=======

Name is the technical name of the :term:`GC`.

|

.. image:: ../../images/devguide/dfx-prop-main-name.png


**Value:**

* *scope variable*
* *'string'*

**Default:** for proposed default Names for Name see :ref:`style-gcnames-label`

**Notes:**


The databinding of the checkbox control to an angular scope variable. Type a scope variable name or select from
possible scope variables by clicking on the **...** to the right of the Binding field to open the Expression Editor to
one:

.. image:: ../../images/gcs/dfx-expression-editor.png

Binding can be:

simple: scope variable name (for example myVariable);
complex: the path to the variable (for example myArray[3].myVariable).

If the :term:`GC` is in a Repeatable Panel and needs to bind to to some repeatable item property, then the binding
should be: $dfx_item.myVariable. For more on $dfx_item see :ref:`dfx-webgc-panel-label`

**HTML Binding** - The HTML control can be bound to data coming from a service, for example a service that
goes to a content management system. Text that will be displayed in the field.
