## How quickly is it changing?

In everyday life, we often want to know how quickly or slowly something changes, whether we're tracking our progress, monitoring a process, or making decisions. For example, if you have money in a bank account, you might be interested in how quickly interest accumulates as each day goes by. In biology, you might wonder how rapidly the height of a plant increases over the course of several days as it grows toward the sunlight. Or, in environmental science, you could be concerned with how fast the temperature of a lake drops as you move deeper below the surface. Each of these situations involves measuring how one quantity changes in relation to another—time, distance, or depth—and understanding that rate of change helps us interpret, predict, and manage the world around us.

In many situations, the rate at which something changes is not constant, but varies depending on the time or position. For example, when you go for a run, your heart rate might increase quickly at the beginning of your exercise and then rise more slowly as you settle into a steady pace. Or, the temperature in a swimming pool might drop quickly near the surface and much more slowly as you go deeper. When the rate of change is not the same everywhere, it becomes useful to measure the average rate of change over a certain period of time or across a particular range, giving us a single number that describes the overall trend.

### Average Velocity

One familiar example of a changing rate is **velocity**, which describes how quickly an object’s position changes with time. Imagine tossing a ball straight up into the air: as the ball rises, it slows down because gravity is pulling it back toward the ground. At the very top of its path, the ball briefly stops before starting to fall back down, speeding up as it descends. In this scenario, the velocity of the ball is not constant—it’s positive and decreasing on the way up, zero at the peak, and then negative (as it falls) and increasing in magnitude on the way down. This makes velocity a perfect example of a rate of change that naturally varies over time.

**Example 1: Average Velocity of a Tossed Ball**

Suppose you toss a small rubber ball straight up into the air from ground level, and its height above the ground (in meters) after $t$ seconds is given by the function

$$
h(t) = 10t - 5t^2
$$

where $t$ is measured in seconds.

What is the average velocity of the ball between $t = 1.0$ seconds and $t = 1.2$ seconds?

**Solution:**

The **average velocity** over a given time interval is defined as the change in position divided by the change in time. In other words, it tells us how much the position of the ball changes, on average, for each second during the specified time interval. Mathematically, the average velocity between times $t_1$ and $t_2$ is given by:

$$
\text{Average velocity} = \frac{h(t_2) - h(t_1)}{t_2 - t_1}
$$

where $h(t)$ is the position (height) at time $t$.

In this problem, we are asked to find the average velocity of the ball between $t_1 = 1.0$ seconds and $t_2 = 1.2$ seconds.

First, we calculate the height of the ball at both times using the given position function:

$$
h(1.0) = 10 \times 1.0 - 5 \times (1.0)^2 = 10 - 5 = 5\, \text{meters}
$$

$$
h(1.2) = 10 \times 1.2 - 5 \times (1.2)^2 = 12 - 5 \times 1.44 = 12 - 7.2 = 4.8\, \text{meters}
$$

Now, we substitute these values into the formula for average velocity:

$$
\text{Average velocity} = \frac{h(1.2) - h(1.0)}{1.2 - 1.0} = \frac{4.8 - 5}{0.2} = -1.0\, \text{meters per second}
$$

**Significance of the negative sign**
Notice that the negative sign in the answer (a negative velocity) means that the position of the ball is decreasing as time goes by—in other words, the ball is moving downward during this time interval. This tells us that at $t = 1$ second, the ball has already passed its highest point and is on its way back down toward the ground. The sign of the velocity gives us important information about the direction of motion, not just the speed.

---
## Calculating average rate of change

The example above illustrates a common approach used in many contexts: measuring how much one quantity changes, on average, with respect to another. More generally, if we have any function $f(x)$, the **average rate of change** of $f$ over an interval from $x$ to $x + \Delta x$ is given by the formula:

$$
\text{Average rate of change} = \frac{f(x + \Delta x) - f(x)}{\Delta x}
$$

This formula tells us how much the function’s value changes for each unit of change in $x$, providing a single number that summarizes the overall trend across the chosen interval. Whether we are talking about position changing over time, temperature changing with depth, or any other relationship, this difference quotient is the key tool for finding an average rate of change.

### Average Steepness
It's important to note that the variable $x$ in this formula does not necessarily have to represent time. In many situations, the independent variable could be something else—distance, depth, length, or even temperature. For example, if we are studying how the elevation of a hiking trail changes as you move along its length, then $x$ would represent distance rather than time. The average rate of change formula applies just as well, giving us useful information about how one quantity changes in relation to another, regardless of the context.

---

**Example 2: Average Steepness of a Ski Slope**

Suppose you are skiing down a man-made ski slope, and the elevation of the slope (in meters above sea level) at a horizontal distance $x$ meters from the starting point is given by

$$
E(x) = 900 - 0.06x - 0.0003x^2
$$

where $x$ is the horizontal distance along the slope.

Calculate the average steepness (average rate of change of elevation with respect to horizontal distance) between $x = 100$ meters and $x = 400$ meters.


**Solution:**

To find the average steepness of the ski slope between $x = 200$ meters and $x = 300$ meters, we use the formula for average rate of change:

$$
\text{Average rate of change} = \frac{E(x + \Delta x) - E(x)}{\Delta x}
$$

Here, $x = 200$ meters and $\Delta x = 100$ meters, so $x + \Delta x = 300$ meters.

First, calculate the elevation at both positions:

$$
E(200) = 900 - 0.06 \times 200 - 0.0003 \times (200)^2
= 876 \text{ meters}
$$

$$
E(300) = 900 - 0.06 \times 300 - 0.0003 \times (300)^2
 = 855 \text{ meters}
$$

Now substitute these values into the average rate of change formula:

$$
\text{Average steepness} = \frac{E(300) - E(200)}{300 - 200} = \frac{855 - 876}{100} = -0.21
$$

**Interpretation:**
The average steepness of the slope between $x = 200$ meters and $x = 300$ meters is $-0.21$ meters per meter. In other words, for every additional meter in the horizontal direction, the height of the slope is reduced by 0.21 meters. The negative sign indicates that the elevation decreases as you move along the slope—in other words, you are skiing downhill.

