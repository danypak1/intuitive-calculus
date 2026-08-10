# Unit 11: The Derivative as a Rate of Change

## 1. The idea, in plain words

You've already used derivatives to find velocity in earlier units — this unit gives that idea its full toolkit and vocabulary, and adds a brand-new character: **acceleration**.

**Picture a car driving along a straight road.** Its **position**, $s(t)$, tells you where it is at time $t$. Its **velocity**, $v(t) = s'(t)$, tells you how fast the position is changing — and, importantly, in which direction. Its **acceleration**, $a(t) = v'(t)$, tells you how fast the *velocity itself* is changing — in other words, acceleration is the derivative of the derivative of position.

**Velocity vs. speed — a crucial distinction:**

- **Velocity** can be positive, negative, or zero. The sign tells you the *direction*: positive means moving one way (say, forward or upward), negative means moving the other way (backward or downward), and zero means momentarily at rest.
- **Speed** is just $|v(t)|$ — velocity's size, with the direction information stripped away. Speed is never negative.

**The single most useful trick this unit teaches — figuring out if something is speeding up or slowing down:** compare the *signs* of velocity and acceleration at the same moment.

- If $v(t)$ and $a(t)$ have the **same sign** (both positive, or both negative), the object is **speeding up** — the push (acceleration) is working in the same direction the object is already moving, so it moves faster and faster.
- If $v(t)$ and $a(t)$ have **opposite signs**, the object is **slowing down** — the push is working against the direction of motion, like tapping the brakes.

**Picture it like a car and gas pedal:** if you're driving forward (positive velocity) and you press the gas (positive acceleration), you speed up. If you're driving forward but tap the brakes (negative acceleration), you slow down. If you're already in reverse (negative velocity) and you press the gas pedal in reverse (negative acceleration), you speed up too — going backward, faster and faster.

## 2. Toolbox

**Position, velocity, and acceleration:**
$$s(t) = \text{position} \qquad v(t) = s'(t) = \text{velocity} \qquad a(t) = v'(t) = s''(t) = \text{acceleration}$$

**Speed:**
$$\text{speed} = |v(t)|$$

**Direction of motion:**
$$v(t) > 0 \Rightarrow \text{moving in the positive direction}$$
$$v(t) < 0 \Rightarrow \text{moving in the negative direction}$$
$$v(t) = 0 \Rightarrow \text{momentarily at rest}$$

**Speeding up or slowing down test:**
$$v(t) \text{ and } a(t) \text{ same sign} \Rightarrow \text{speeding up} \qquad v(t) \text{ and } a(t) \text{ opposite signs} \Rightarrow \text{slowing down}$$

**General rates of change:** this same idea extends beyond motion — for any quantity $y$ that depends on $x$, $\dfrac{dy}{dx}$ tells you the instantaneous rate at which $y$ changes as $x$ changes (like marginal cost or marginal revenue from earlier units).

## 3. Common mistakes

- **Mixing up velocity and speed.** Velocity carries a sign (direction); speed is always the non-negative size of that velocity. If a problem asks for "speed," take the absolute value of your velocity answer.
- **Assuming negative velocity automatically means slowing down.** Negative velocity just means moving in the negative direction — whether it's speeding up or slowing down still depends on comparing it to the sign of the acceleration.
- **Forgetting acceleration is the derivative of velocity, not of position directly (well — technically the second derivative of position).** You must differentiate twice: once to get $v(t)$, and again to get $a(t)$.
- **Applying the speeding-up/slowing-down test using only the acceleration's sign, ignoring the velocity's sign.** You always need both signs together — acceleration by itself never tells you whether something is speeding up or slowing down.
- **Forgetting that $v(t)=0$ means "momentarily at rest," not "speeding up" or "slowing down."** At that exact instant, the speeding-up/slowing-down question doesn't really apply — it's a turning point.

## 4. Problem Set

### 🟢 Warm-up

1. $s(t)=t^2-4t$. Find $v(t)$ and $a(t)$. Evaluate $v(1)$ and $a(1)$, and state whether the object is moving in the positive or negative direction at $t=1$.
2. $s(t)=3t^2+2t-5$. Find $v(t)$ and $a(t)$. Evaluate both at $t=0$.
3. $s(t)=t^3-3t^2$. Find $v(t)$ and $a(t)$. Evaluate $v(2)$.
4. $s(t)=-16t^2+40t$ (height in feet of a tossed object). Find $v(t)$. Evaluate $v(0)$ (the initial velocity), and find the time when $v(t)=0$ (the moment of peak height).
5. $s(t)=t^2-6t+8$. Find $v(t)$. Determine whether the object is moving in the positive or negative direction at $t=1$.
6. $s(t)=2t^3-9t^2+12t$. Find $v(t)$ and $a(t)$. Evaluate $v(1)$ and $a(1)$, and state whether the object is at rest at $t=1$.

### 🟡 Standard

7. $s(t)=t^3-6t^2+9t$. Find $v(t)$ and $a(t)$. At $t=0.5$, is the object moving forward or backward? Is it speeding up or slowing down?
8. $s(t)=t^2-8t+7$. Find $v(t)$ and $a(t)$. At $t=2$, find the speed and direction of motion, and determine whether the object is speeding up or slowing down.
9. $s(t)=-t^3+3t^2$. At $t=0.5$, find the velocity and acceleration, and determine whether the object is speeding up or slowing down.
10. $s(t)=t^3-3t^2-9t$. Find $v(t)$ and $a(t)$. At $t=4$, find the speed and describe the object's motion (direction, and speeding up or slowing down).
11. $s(t)=16-t^2$. Find $v(t)$ and $a(t)$. At $t=1$, determine the direction of motion and whether the object is speeding up or slowing down.
12. $s(t)=t^3-12t$. Find $v(t)$ and $a(t)$. Compare the object's speeding-up/slowing-down status at $t=1$ versus at $t=3$.

### 🔴 Challenge

13. $s(t)=t^3-6t^2+9t$ (same function as Problem 7). Find all $t\ge 0$ where the object is momentarily at rest. Then, for each of those times, determine the direction of motion (and whether the object is speeding up or slowing down) just before and just after that instant.
14. $s(t)=2t^3-3t^2-12t+5$. Find $v(t)$ and $a(t)$. Find all $t$ (including negative solutions, mathematically) where the object is at rest, noting which are physically relevant if we require $t\ge 0$. For the physically relevant rest time, describe the motion just before and just after.
15. $s(t)=\sqrt{t}+t$ for $t>0$. Find $v(t)$ and $a(t)$ using the power rule with fractional exponents. Evaluate both at $t=4$.
16. $s(t)=\dfrac{1}{t+1}$ for $t\ge 0$. Find $v(t)$ and $a(t)$. Determine the sign of $v(t)$ for all $t \ge 0$, and explain in words what this tells you about the object's motion (does it ever come to rest?).
17. You're given the velocity function directly: $v(t)=t^2-4t+3$ for $t$ in $[0,4]$ (no position function needed). Find $a(t)$. Then, by checking the signs of $v(t)$ and $a(t)$ on the subintervals between the times where $v(t)=0$, describe the full motion story across $[0,4]$: when is the object at rest, when is it speeding up, and when is it slowing down?

### 🌍 Applied

18. A model rocket's height in feet is $h(t) = -16t^2+200t+10$. Find $v(t)$ and $a(t)$. Evaluate $v(3)$ and $a(3)$, and explain physically whether the rocket is speeding up or slowing down at $t=3$ seconds.
19. An elevator's height in meters is $y(t) = t^3-9t^2+24t+2$ for $t$ in $[0,4]$. Find $v(t)$ and $a(t)$. Evaluate both at $t=1$, and describe the elevator's motion at that moment (direction, and speeding up or slowing down).
20. A stock's price in dollars is modeled by $P(t) = t^3-5t^2+3t+60$, where $t$ is measured in months. Find $P'(t)$ and $P''(t)$. Evaluate both at $t=1$, and interpret whether the stock's price change is accelerating or decelerating at that moment.
21. A dropped object's height in feet is $h(t)=100-16t^2$. Find $v(t)$ and $a(t)$. Evaluate $v(2)$ (interpreting it as a speed), and explain why $a(t)$ stays the same at every value of $t$ — what does this tell you about the object's fall?
