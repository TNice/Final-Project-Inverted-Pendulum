# Final Project Inverted Pendulum
Note: This was tested on a computer with Intel i9 processor, 64GB of RAM and Windows 10 operating system
## Description
Using matlab I created 2 models of a PID controller balancing an inverted pendulum on a cart (image below). Both models extend the dynamics equations from a Cal Tech physics lab document by Kenneth G Libbrecht(http://pmaweb.caltech.edu/~phy003/handout_source/Inverted_Pendulum/InvertedPendulum.pdf) to having the pendulum on a cart opposed to a shaker table. The "simple model" has the assumption that the rod has 0 mass and the "better model" takes the mass of the rod into account.

## Running Models
### Version 1
1. open matlab
2. open the project file in matlab
3. go to the models folder in the project
4. double click on the model to open
5. modifiy desired parameters
6. click green play button to run 

### Version 2
1. open the models folder
2. double click on the model to open
3. choose to open just the model or the model with the project
4. modifiy desired parameters
5. click green play button to run 

## Model Descriptions

![alt text](https://github.com/TNice/Final-Project-Inverted-Pendulum/blob/main/images/Inverted%20Pendulum%20Pic.png)

### Simple Model
#### Notation
* M - mass of the cart
* m - mass of the weight
* l - length of the rod
* $\theta$ - angle of the rod
* g - acceleration of gravity
* $a_{cart}$ - acceleration of the cart

### Dynamics
$\theta = \theta_0 + d\theta$

$d^2\theta = \frac{g\theta}{l} - \frac{Ma_{cart}}{ml}$

### Better Model
#### Notation
* M - mass of the cart
* $m_m$ - mass of the weight
* $m_l$
* l - length of the rod
* $\theta$ - angle of the rod
* g - acceleration of gravity
* $a_{cart}$ - acceleration of the cart

### Dynamics
$\theta = \theta_0 + d\theta$

$I = (m_m + \frac{m_l}{3})l^2$

$d^2\theta = \frac{g\theta - Ma_{cart}}{lI} + \frac{m_l\theta g}{2lI}$
