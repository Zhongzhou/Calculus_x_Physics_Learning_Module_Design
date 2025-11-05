
# Introduction to Instantaneous Velocity

In the previous modules, we practiced finding the *instantaneous rate of change* of a variable by starting with its *average rate of change* over a period of time, and taking the limit at which the time interval shrinks to zero. We also saw a simple example of calculating the instantaneous velocity of an tossed straight into the air, by applying this method to its position vs. time function. In this module, we will use the same mathematical techniques to more carefully examine the instantaneous velocity of objects moving in a single dimension -- motion along a straight line, either forward or backward.

**Definition of instantaneous velocity**

You have probably seen velocity described in everyday terms as *change in position divided by change in time*. This definition works well for average velocity: if an object moves from position $x(t)$ at time $t$ to position $x(t + \Delta t)$ at a later time $t + \Delta t$, the average velocity is

$$
v_\text{avg} = \frac{x(t+\Delta t) - x(t)}{\Delta t}.
$$

Now let’s make this more precise. Suppose we know—either exactly, or from enough data points to closely approximate—the position of the object at every instant in time. Based on what we learned in the previous module, we can define the *instantaneous velocity* at time $t$ as the limit of the average velocity as $\Delta t \to 0$:

$$
v(t) = \lim_{\Delta t \to 0} \frac{x(t+\Delta t) - x(t)}{\Delta t}.
$$

Knowing the instantaneous velocity of an object is crucial in many real-world situations. In space exploration, it allows scientists to calculate the momentum and energy of asteroids or spacecraft, which is essential for predicting their orbits and planning navigation. In autonomous vehicle systems, instantaneous velocity helps determine how quickly the car is approaching other vehicles or obstacles, enabling safe and timely braking or steering. In engineering and safety applications, such as crash testing or automated machinery control, monitoring instantaneous velocity ensures that systems operate within safe limits and respond quickly to changing conditions.

The definition of instantaneous velocity works for any kind of smooth motion, not just simple cases like tossing a ball in the air. As long as the position changes continuously over time—without sudden jumps—we can use it. This means we can find the instantaneous velocity of things like a car driving on a straight track, a drone moving through a tunnel, or even a spacecraft in flight. In real life, we might get position data from sensors or GPS and use a smooth curve to model the motion, then apply the definition to find the velocity at any instant.

### Example — Drone along a straight tunnel

A small inspection drone flies down a straight service tunnel. Its position $x(t)$ (meters from a fixed entrance doorway) is programed to be:

$$
x(t)=5+3.6t+0.30t^{2}-\frac{1}{15}t^{3}\qquad (0\le t\le 8\ \text{s}).
$$

Using the definition $v(t)=\lim_{\Delta t\to 0}\dfrac{x(t+\Delta t)-x(t)}{\Delta t}$, find the **instantaneous velocity** of the drone at $t=4.0\ \text{s}$ and at $t=8.0\ \text{s}$. Include the sign to indicate forward $(+)$ or backward $(-)$ motion.

<p align="center">
  <img src="drone_in_tunnel.png" 
       alt="A quadcopter drone flying inside a cylindrical concrete tunnel, illuminated from a distant opening." 
       width="300">
  <br>
  <em>Figure 1: An inspection drone flying inside a straight service tunnel from an entrance at changing velocity.</em>
</p>


---

### Solution

Start with the definition

$$
v(t)=\lim_{\Delta t\to 0}\frac{x(t+\Delta t)-x(t)}{\Delta t},
\quad
x(t)=5+3.6t+0.30t^{2}-\frac{1}{15}t^{3}.
$$

Expanding $x(t+\Delta t)$, forming the difference quotient, and simplifying gives

$$
v(t)=-0.2\,t^{2}+0.6\,t+3.6.
$$

Evaluate:

* At $t=4\ \text{s}$: $v(4)=-0.2(16)+0.6(4)+3.6= -3.2+2.4+3.6=+2.8\ \text{m/s}$ (forward).
* At $t=8\ \text{s}$: $v(8)=-0.2(64)+0.6(8)+3.6= -12.8+4.8+3.6=-4.4\ \text{m/s}$ (backward).

**Answers:** $v(4)=+2.8\ \text{m/s}$, $v(8)=-4.4\ \text{m/s}$. The sign change is consistent with the zero of $v(t)$ at $t=6\ \text{s}$.

## Velocity vs. Speed
---

It is important to distinguish between the terms **speed** and **velocity**. *Velocity* is a vector—it tells us both how fast an object’s position is changing and in which direction. *Speed*, on the other hand, is just the magnitude of this rate of change; it does not include direction. We will postpone the full discussion of velocity as a vector until after we introduce formal vector notation. For now, we will focus on the simplest case: objects moving in one dimension—back and forth along a straight line. In this case, velocity can be either positive or negative, depending on how we define the positive direction of motion. In the example above, the position–time function is measured from the tunnel entrance, so the positive direction is defined as moving away from the entrance. At $t=4\ \text{s}$ the drone’s velocity was $+2.8\ \text{m/s}$, meaning it was moving forward (away from the entrance), while at $t=8\ \text{s}$ the velocity was $-4.4\ \text{m/s}$, meaning it had reversed direction and was moving back toward the entrance. The **speed** at those moments would simply be $2.8\ \text{m/s}$ and $4.4\ \text{m/s}$, ignoring the sign.


