Events
^^^^^^

Events allow developers to perform actions when the event is triggered on a control in the View.
Events are used in combination with functions. The function is executed when the the event occurs (for example, when a
user clicks a button, when the mouse moves over the control, ..).

.. figure:: ../../images/gcs/events-areachart.png
   :width: 400px

   Each of the events takes a function name that will be executed when the user invokes the event. In the example above
   the function named *myFunction* will be executed on the *On Double Click* event.


Functions called in a View are defined in the view controller in the script of the View. Clicking on the ... opens a window
providing the current list of functions that are available to be used from the View.

|

+---------------------+-----------------+----------------------------------------------------------------------------------------------------+
| **Events**          | Possible Values | Description                                                                                        |
+=====================+=================+====================================================================================================+
| On Area Click:      | *Function call* | The function is executed when the user clicks on the area of the graph triggering the event.       |
+---------------------+-----------------+----------------------------------------------------------------------------------------------------+
| On Area Mouse Over: | *Function call* | The function is executed when the user passes the mouse over the area of the graph.                |
+------------------+-----------------+-------------------------------------------------------------------------------------------------------+
| On Area Mouse Leave:| *Function call* | The function is executed when the mouse is moved out of the area of the graph.                     |
+---------------------+-----------------+----------------------------------------------------------------------------------------------------+
| On State Change:    | *Function call* | The function is executed when the user presses a mouse button over the control.                    |
+---------------------+-----------------+----------------------------------------------------------------------------------------------------+
| On Render End:      | *Function call* | The *Mouse Up* event occurs when the mouse is released over the control which triggers the function|
|                     |                 | to be executed.                                                                                    |
+---------------------+-----------------+----------------------------------------------------------------------------------------------------+

|