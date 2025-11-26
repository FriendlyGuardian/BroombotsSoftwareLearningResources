Calling methods
================

In Java, methods are blocks of code that belong to objects. When you want an object to perform a specific action, you call its method.
Methods are also sometimes referred to as functions or procedures in other programming languages.
To call a method, you typically use the following syntax:
.. code-block:: java
    objectName.methodName(arguments);

Here, ``objectName`` is the name of the object whose method you want to call, ``methodName`` is the name of the method, and ``arguments`` are the values you pass to the method (if any).

Here is what this looks like with the robot
.. code-block:: java
    // initialized all of the systems of the robot using its method - This method has no parameters in this example
    robot.initialize()

    // makes the robot pause its movement but continue to hold its place - This method has one parameter: Time in seconds for the wait
    robot.chill(2)

.. note:: 
    These code examples are not something will are going to work if you just copied and pasted them!
    These functions in reality have more parameters or could be named something else in the future.

**Methods can also return things**
When we say return, we mean that calling this method will give us something back to work with. 
Technically, all methods return something. When a method does not need to give anything back, it returns ''Void''

Here is a method that adds two numbers together
.. code-block:: java
    public int sumTwoNumbers(int num1, int num2){
        return num1 + num2
    }

Here is what it would look like to use this method and store its return value in a variable called ''result''
.. code-block:: java
    int result = sumTwoNumbers(5, 10);
    // result now holds the value 15

