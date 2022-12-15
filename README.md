# Final Project Inverted Pendulum
 
## Description
Using matlab I created 2 models of a PID controller balancing an inverted pendulum on a cart (image below). Both models extend the dynamics equations from a Cal Tech physics lab document by Kenneth G Libbrecht(http://pmaweb.caltech.edu/~phy003/handout_source/Inverted_Pendulum/InvertedPendulum.pdf) to having the pendulum on a cart opposed to a shaker table. The "simple model" has the assumption that the rod has 0 mass and the "better model" takes the mass of the rod into account.

## Models

### Simple Model
#### Notation
* M - mass of the cart
* m - mass of the weight
* l - length of the rod
* $\theta$ - angle of the rod
* g - acceleration of gravity
* a_cart - acceleration of the cart
