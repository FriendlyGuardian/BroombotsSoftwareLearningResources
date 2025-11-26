Connecting To The Robot
=======================

We need to connect to the robot in order to change the code on the robot
There are two ways to connect to the robot

* ``ADB`` (Android Debug Bridge)
* Direct Connection

ADB
---

``ADB`` is installed through Android Build-Tools. You can install it through through the ``SDK Manager`` in Android Studio. 
First step to connecting to the robot is to connect the robots wi-fi network. 
The control hub hosts its own wi-fi network as the only method for wireless communication. 
This is how the driver hub communicates with the robot.

Steps

* In Windows, Navigate to the task bar
* Click on the wi-fi symbol
* Click again onto the left part of the wi-fi tab
* In available networks, find the network that follows this format ``[team number]-[#]-RC``

.. note::
    The Control Hub network defaults to ``FTC-[some random string]``, if that is what you see,
    than connect to the network with the password ``password`` 
    in a web browser, enter the address ``192.168.43.1:8080``
    and navigate through the menus to change the name and password of the wifi network

* Make sure the network is checked as ``auto-connect``
* All Broombot Control Hub passwords are the same, ask senior members or mentors for it if you want it.
* In Android Studio, Navigate to the terminal; you can find it in view/Tool Windows/Terminal or on the left tool bar
* Enter in the following command ``adb connect 192.168.43.1:5555`` - the control hub's ip address and the port it operates on
* Make sure the terminal returns ``Connected``, if you do not get this, look at trouleshooting
* Now at the top of the screen, ``No Devices`` should be replaced with ``Rev Control Hub`` 
* Press the play or restart circle symbol to the right of the launch method to send code to the robot!

.. note::
    You will not have any internet connection while you are connected to the robot


.. warning::
    If you switch networks while still connected to the robot, 
    the robot will enter a state where it thinks it is still connected and will not accept any other connections
    If the Control Hub at the top of the screen shows an explanation mark, than your computer has lost connection
    The only way to fix this is to power-cycle the robot and reconnect

.. note::
    If you want to disconnect from the robot in a way that allows a reconnection,
    use the command in the terminal ``adb disconnect``


Direct Connection
-----------------

This is a wired connection to the robot. All you need to do is plug a wire into your computer and the USB-C port of the Control hub

.. note::
    This is a pretty good reason to make sure that the USB-C port is accessible at all times

.. warning::
    Make sure you unplug the wire before running the robot as to not damage anything!


Troubleshooting
---------------

**cannot connect to an unreachable host**

Either you are not actually connected to the robot or the robot already has a previous connection