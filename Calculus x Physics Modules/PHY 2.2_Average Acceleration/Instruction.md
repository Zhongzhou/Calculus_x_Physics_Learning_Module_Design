
## Introduction to Acceleration
In the previous module, we saw that a moving object can have different velocities at different times. You learned how to calculate its *instantaneous velocity* at a particular moment in time from the change in its position over time. But here’s another question to think about: if the velocity of an object changes as time goes on, can we similarly define a physics quantity that tells us how quickly that velocity itself is changing?

**2. Introducing average acceleration**
To answer that, let’s remember how we defined **average velocity**: it’s the change in position $\Delta x$ divided by the time interval $\Delta t$ over which that change occurs.

$$
\text{Average velocity} = \frac{\Delta x}{\Delta t}
$$

In exactly the same way, we can define **average acceleration** as the change in velocity $\Delta v$ divided by the time interval $\Delta t$ over which the velocity changes:

$$
\text{Average acceleration} = \frac{\Delta v}{\Delta t}
$$

Here, $\Delta v = v\_{\text{final}} - v\_{\text{initial}}$ tells us how much the velocity has changed, and dividing by $\Delta t$ tells us how quickly that change happened. Just like average velocity gives us the average rate of change of position, average acceleration gives us the average rate of change of velocity over a specific time period.

### Calculating average acceleration

If you already know how velocity changes with time, finding the average acceleration is just as straightforward as finding average velocity from position: you simply take the change in velocity and divide it by the change in time. However, even if you do not have velocity values directly, you can still determine the average acceleration from a position–time function. First, use the position data to calculate the velocities at the relevant times, then apply the same formula for average acceleration. Here’s an example of how this process works.


### Example — Autonomous warehouse cart

<!-- Put this directly where you want the image to appear in your .md -->
<figure style="margin:1rem 0; text-align:center;">
  <img
    src="./Figures/cart-in-aisle.png"          
    alt="Autonomous warehouse cart moving along a center aisle between tall racks"
    style="max-width:100%; width:300px; height:auto; border-radius:8px;"
  />
  <figcaption style="font-size:0.9rem; color:#666;">
    Autonomous warehouse cart in a storage aisle. Image generated with AI.
  </figcaption>
</figure>


An autonomous cart travels straight down a warehouse aisle. Let $x(t)$ (in meters) be its position measured **away from the loading dock** ($x=0$ at the dock). Its motion is modeled by

$$
x(t) = 12 + 7t + 1.6t^2 - 0.4t^3,\quad t\ \text{in seconds}.
$$

Find the **average acceleration** of the cart between the time interval $t = 2.0\,\text{s}$ to $t = 2.5\,\text{s}$.

---

**Solution overview:**
To find the average acceleration, we first need the velocities at $t = 2.0$ s and $t = 2.5$ s. Since velocity is the *instantaneous* rate of change of position, we’ll calculate each velocity by taking the limit of the average velocity over a very small time interval starting at that moment. Once we have both velocities, we’ll use the formula for average acceleration:

$$
\bar a = \frac{\Delta v}{\Delta t}.
$$

---

**Step 1: Find velocity at $t = 2.0\ \text{s}$**
Velocity is defined as

$$
v(t) = \lim_{\Delta t \to 0} \frac{x(t+\Delta t) - x(t)}{\Delta t}.
$$

Substitute $t = 2.0$:

$$
v(2.0) = \lim_{\Delta t \to 0} \frac{\big[12 + 7(2+\Delta t) + 1.6(2+\Delta t)^2 - 0.4(2+\Delta t)^3\big] - \big[12 + 7(2) + 1.6(2)^2 - 0.4(2)^3\big]}{\Delta t}.
$$

Simplifying and letting $\Delta t \to 0$ gives:

$$
v(2.0) = 8.6\ \text{m/s}.
$$

---

**Step 2: Find velocity at $t = 2.5\ \text{s}$**

$$
v(2.5) = \lim_{\Delta t \to 0} \frac{x(2.5+\Delta t) - x(2.5)}{\Delta t}.
$$

Substituting and simplifying yields:

$$
v(2.5) = 7.5\ \text{m/s}.
$$

---

**Step 3: Compute average acceleration**
The formula for average acceleration is

$$
\bar a = \frac{v_{\text{final}} - v_{\text{initial}}}{t_{\text{final}} - t_{\text{initial}}}.
$$

Here, $v_{\text{initial}} = 8.6\ \text{m/s}$ at $t_{\text{initial}} = 2.0\ \text{s}$ and $v_{\text{final}} = 7.5\ \text{m/s}$ at $t_{\text{final}} = 2.5\ \text{s}$.
The time interval is

$$
\Delta t = 2.5 - 2.0 = 0.5\ \text{s}.
$$

Substitute into the formula:

$$
\bar a = \frac{7.5 - 8.6}{0.5} = \frac{-1.1}{0.5} = -2.2\ \text{m/s}^2.
$$

The negative sign means the cart’s velocity is decreasing over time — in other words, it is slowing down — even though both velocities are still positive, so it continues moving away from the dock.

Here’s the student-facing rewrite:

---

**Accelerating or de-ccelerating?**
When you see a positive acceleration, it’s tempting to think, “Oh, the object must be speeding up,” and when you see a negative acceleration, you might think, “It’s slowing down.” But that’s not always true. Acceleration’s sign simply tells you the direction that the velocity is changing, not whether the speed is going up or down. The real key is to compare the signs of velocity and acceleration. If they have the same sign, the object’s speed is increasing. If they have opposite signs, the object’s speed is decreasing. We’ll dig deeper into this idea in a later module, but for now, remember: acceleration’s sign alone doesn’t tell the whole story. It needs to be compared to the sign of the velocity. 

---



