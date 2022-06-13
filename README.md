# Electricity and Magnetism Simulations

Below, I document some physics simulations that fall under E&M.

* **The gif and picture could be from clearly different runs of the experiments**

## RLC Circuit with Lightbulb

In this simulation, there is a circuit consisting of a capacitor, resistor, inductor, and lightbulb. As the voltage changes, the power that grows through the lightbulb changes and so, the color of my lightbulb goes to black as the power gets closer to 0. All three cases below were made with Special Two-Derivative Runge Kutta Nyostrom method for numerical integration since the expression of the second derivative accounted for the first derivative as well. 

Here are the values of the parameters (that remain constant for all three cases):
- Inductance (L) of the inductor = 10**(2.1) Henry
- Capacitance (C) of the capacitor = 10**(-2) Farad
- Resistance (R_lb) of the lightbulb = 9.5 Ohms

### Case 1: Underdampened

![](https://media.giphy.com/media/20LEonxJEZyekDBM80/giphy.gif)
![](https://i.imgur.com/UggKlYe.png)

In this case, R^2 << L/C, where R is the total resistance of the circuit and is positive. This creates a sort of sinosodial pattern, except the amplitude is less than the previous maximum or minimum. Thus, there are portions in which the voltage is negative. Since power is only dependent on V^2, the lightbulb gets brighter as voltage goes from 0 to a negative number. 

### Case 2: Critically Dampened

![](https://media.giphy.com/media/esACsmXkOQh25t542e/giphy.gif)
![](https://i.imgur.com/Ak67uha.png)

In this case, R^2 = L/C, where R is positive. This creates a curve that is initially concave down for a period, then turns concave up and approaches 0 as time goes on forever.

### Case 3: Overdampened

![](https://media.giphy.com/media/oRQLuk2dOmB6MPtuzC/giphy.gif)
![](https://i.imgur.com/ZbxRrFL.png)

In this case, R^2 > L/C, where R is positive. This creates a curve that is concave up and approaches 0 as time goes on forever.

## Particle in an Electric and Magnetic Field

![](https://media.giphy.com/media/AvdIScvatXOtjdP0jW/giphy.gif)
![](https://i.imgur.com/3I5V6Fw.png)

In this simulation, the particle is deployed with a random velocity in a random magnetic and electric field. As seen in the picture and gif, there are three unit vectors pointing from the particle:
- Magnetic Field: Magenta
- Electric Field: Cyan
- Velocity: Yellow

In the position vs t plot:
- x values are red
- y values are green
- z values are blue