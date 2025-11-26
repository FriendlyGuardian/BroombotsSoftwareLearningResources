Basic Java Syntax
==================

Java code consists of files that hold several lines of code
.. code-block:: lines_example
    // line of code that does something
    // line of code that does something else

Every instruction ends with a ';', the symbol for ending a line
.. code-block:: ending-lines-example
    instruction;
    differentIntruction;

To leave notes in code, start the line with '//'
.. code-block:: comment-example
    //Leaving notes on your code is really important to allow for others' to understand how to make changes
    ComplexCode;

Lines of Java are not exactly lines in a file, one line of Java can span multiple lines in one file
.. code-block:: multip-line
    array newArray = new Array(){"chocolate","is","good"};
    
    //is the same as

    array newArray = new Array(){
    "chocolate",
    "is",
    "good"
    };

    // using multiple lines of code for a comples instruction can make the code easier to read, but makes no difference when being compiled!

.. note:: compilers
    Compilers are things that read your code and break it down further into computer instructions, in the process, they check for syntax errors.
    Among other things, 'Gradle' is a compiler.