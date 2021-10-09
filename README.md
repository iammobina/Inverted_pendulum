#  Inverted Pendulum

In this project, a fuzzy controller was designed in order to solve the inverted pendulum problem. pendulum is located on a cart consists of a mass M at the top of a rod of length l pivoted on a horizontally moving base. The rod is considered massless and is carrying a mass m.

 For implementing the fuzzy controller, the code is written in inverted_pendulum.fcl file which is a Fuzzy Control Language file. 

First of all, declared my needed inputs and outputs. After that, it is necessary to FUZZYFY and DEFUZZYFY the required variables, and at the end write my fuzzy rules in the RULEBLOCK section.

 After every run, a report is given from the system that contains charts from x (cart position), x_dot (cart velocity), x_dot_dot (cart acceleration), theta - 180 (pendulum degree), theta_dot (pendulum angular velocity), theta_dot_dot (pendulum angular acceleration), and f (force applied to the cart).

 Note that theta starts from the bottom of the unit circle and goes on the counterclockwise circle. Therefore, theta value is always 90 degrees more than that of the unit circle. Stable state: a state in which the pendulum degree, pendulum angular velocity, pendulum angular acceleration, cart acceleration, and force applied to the cart equal to 0. 

1. designed the fuzzy controller so that the inverted pendulum stays at a stable state for enough time started from a random state that every variable except the pendulum degree is 0. 
2. Made the cart velocity 0 while being at a stable state.

[For more information , click here](http://pyfuzzy.sourceforge.net/doc/quickstart.html)

[For more information , click here](http://ffll.sourceforge.net/fcl.htm)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
