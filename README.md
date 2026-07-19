# sweep-action

In this task i programmed 4 servos to perform sweep action and then returning to 90 degrees using a tinkecad.

To achieve a the sweep action we need 3 main components:
breadboard ( to connect the voltage throught the servos)
arduino ( to program the servos and also use it as a voltage source)
servo ( i used four in this task).

When it comes to coding the arduino i used normal setups lines and while loop with a millis() function.

The millis function works like a timer, when it reaches the line code [unsigned long start = millis();] the variable start stores whatever millie second it reached.
Then using while loop i did a simple math equation [while (millis() - start < 2000)] which stops the action if it reaches 2 seconds.
I did 2 while loops one from 0 to 180 then 180 to 0 ( sweep action), after the to seconds all servos stops at 90 degrees using a simple line [servo1.write(90)].

