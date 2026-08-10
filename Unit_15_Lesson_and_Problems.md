# Unit 15: Related Rates

## 1. The idea, in plain words

Imagine a balloon being filled with air. As it inflates, its radius is growing — but so is its volume, at the very same time, because they're tied together by the same shape. **Related rates problems are about exactly this: when two or more quantities are connected by an equation, and they're all changing over time, knowing how fast one of them changes lets you figure out how fast another one changes too.**

**Picture it like a see-saw of connected gears.** If two gears are locked together, turning one automatically turns the other at some related speed — you don't need to know anything else about the second gear except how it's mechanically connected to the first. Related rates problems work the same way: find the equation that "locks" your variables together (usually a geometry formula, or something from the word problem itself), then use implicit differentiation — but this time, with respect to **time**, $t$ — to link the *rates* together.

**The step-by-step strategy (memorize this order — it matters):**

1. **Draw a picture** if the problem describes a physical situation (a ladder, a shadow, two moving cars). Label every quantity that changes over time with a variable.
2. **Write down what you're given and what you want** — in derivative language. "The radius is growing at 3 cm/s" becomes $\dfrac{dr}{dt}=3$. "Find how fast the area is changing" means you want $\dfrac{dA}{dt}$.
3. **Find an equation connecting the variables** — usually a geometry formula (area, volume, the Pythagorean theorem, similar triangles) or something given directly in the problem.
4. **Differentiate both sides of that equation with respect to $t$**, using the chain rule — every variable that depends on time picks up its own rate term (like $\dfrac{dr}{dt}$), exactly like the $y'$ trick from implicit differentiation, just with $t$ instead of $x$ as the "hidden" variable everything depends on.
5. **Now — and only now — plug in the specific numbers** you were given for that instant (the specific radius, the specific rates, etc.).
6. **Solve for the rate you were asked to find.**

**The single most important rule in this whole unit:** *never* substitute in the specific numbers until *after* you've differentiated. If you plug numbers in too early, you accidentally turn a changing quantity into a fixed constant, and its derivative becomes $0$ — which destroys the whole problem.

## 2. Toolbox

**Common connecting equations:**
$$\text{Circle area: } A=\pi r^2 \qquad \text{Sphere volume: } V=\frac{4}{3}\pi r^3$$
$$\text{Square area: } A=s^2 \qquad \text{Cube volume: } V=s^3$$
$$\text{Cylinder volume: } V=\pi r^2h \qquad \text{Cone volume: } V=\frac13\pi r^2h$$
$$\text{Pythagorean theorem: } a^2+b^2=c^2 \qquad \text{Rectangle area: } A=LW$$
$$\text{Box volume: } V=lwh \qquad \tan\theta = \frac{\text{opposite}}{\text{adjacent}}$$

**Differentiating with respect to time — the key move:** every variable gets its own rate term when you differentiate, exactly like implicit differentiation:
$$\frac{d}{dt}\big[r^2\big] = 2r\cdot\frac{dr}{dt} \qquad \frac{d}{dt}[xy] = \frac{dx}{dt}\cdot y + x\cdot\frac{dy}{dt}$$

**Similar triangles** (useful for cones, shadows, and ramps): if two triangles have the same shape (just different sizes), their corresponding sides are proportional — this lets you write one variable in terms of another *before* you differentiate, often simplifying a two-variable problem into a one-variable one.

## 3. Common mistakes

- **Substituting known numbers into the equation before differentiating.** This is the single most damaging mistake possible in this unit — it silently turns a changing quantity into a constant and wipes out all the rate information. Always differentiate first, plug in numbers second.
- **Forgetting a rate term for one of the variables.** Every variable that changes with time needs its own $\dfrac{d(\cdot)}{dt}$ when you differentiate — it's easy to accidentally treat one variable as if it were fixed.
- **Mixing up which rate is given and which is being asked for.** Write both down clearly before starting — it's easy to lose track partway through a multi-step problem.
- **Sign errors for quantities that are shrinking.** A rate of change for something *decreasing* (draining, sliding down, shrinking) should be written as a *negative* number when you plug it in.
- **Using the wrong geometric formula, or forgetting to relate two variables (like $r$ and $h$ in a cone) using similar triangles before differentiating**, when the problem only gives you a rate for one of them.
- **Forgetting units in the final answer.** A rate always has units attached (cm/s, ft/min, etc.) — always report them.

## 4. Problem Set

### 🟢 Warm-up

1. A circle's radius is increasing at $3$ cm/s. Find the rate of change of the area when $r=5$ cm.
2. A square's side length is increasing at $2$ cm/s. Find the rate of change of the area when the side is $4$ cm.
3. A sphere's radius is increasing at $4$ cm/s. Find the rate of change of the volume when $r=3$ cm.
4. A cube's side length is increasing at $1$ cm/s. Find the rate of change of the volume when the side is $5$ cm.
5. A circle's radius is decreasing at $2$ cm/s. Find the rate of change of the area when $r=6$ cm.
6. An equilateral triangle's side length is increasing at $3$ cm/s. Given $A=\dfrac{\sqrt3}{4}s^2$, find $\dfrac{dA}{dt}$ when $s=6$ cm.

### 🟡 Standard

7. A $10$-foot ladder leans against a wall. The bottom is sliding away from the wall at $2$ ft/s. Find how fast the top of the ladder is sliding down the wall when the bottom is $6$ feet from the wall.
8. A balloon rises straight up at $5$ ft/s from a point on the ground $100$ feet from an observer. Find how fast the distance between the observer and the balloon is changing when the balloon is $75$ feet high.
9. Water is poured into a cylindrical tank of fixed radius $3$ ft at a rate of $2$ ft³/min. Find how fast the water level is rising.
10. Two cars leave an intersection at the same time — one heading east, one heading north. The eastbound car travels at $40$ mph and the northbound car travels at $30$ mph. Find how fast the distance between them is changing at the moment the eastbound car is $3$ miles from the intersection and the northbound car is $4$ miles from the intersection.
11. A rectangle's length is increasing at $3$ cm/s while its width is decreasing at $2$ cm/s. Find the rate of change of the area at the moment the length is $10$ cm and the width is $6$ cm.
12. A person $6$ feet tall walks away from a $15$-foot lamp post at a rate of $5$ ft/s. Find the rate at which the length of their shadow is changing.
13. A rectangle has a fixed width of $4$ cm, while its length increases at $2$ cm/s. Find the rate of change of the diagonal when the length is $3$ cm.

### 🔴 Challenge

14. An inverted conical tank has a top radius of $4$ ft and a height of $10$ ft. Water drains out at a rate of $3$ ft³/min. Find how fast the water level is dropping when the water is $5$ ft deep. (You'll need similar triangles to relate the radius and height of the water's surface first.)
15. At noon, Ship A is $100$ km west of Ship B. Ship A sails east at $15$ km/h, and Ship B sails north at $20$ km/h. Find how fast the distance between the two ships is changing at 4:00 PM.
16. A kite flies at a constant height of $300$ ft. It moves horizontally away from the person flying it at $25$ ft/s. Find how fast string is being let out when $500$ ft of string has been let out.
17. A rectangular box's dimensions are all changing at once: length $l=4$ ft (growing at $2$ ft/min), width $w=3$ ft (shrinking at $1$ ft/min), and height $h=2$ ft (growing at $3$ ft/min). Find the rate of change of the volume at this instant.
18. A spotlight is fixed $50$ m from a straight running track. A runner moves along the track at $6$ m/s. Find how fast the angle between the spotlight's beam and the perpendicular line to the track is changing, at the moment the runner is $50$ m past the point on the track closest to the spotlight.

### 🌍 Applied

19. A company's revenue is $R=xp$, where $x$ is the number of units sold and $p$ is the price per unit. Currently $x=100$ units and $p=\$20$. Sales are growing at $5$ units per week, while the price is dropping at $\$0.50$ per week. Find the rate of change of revenue.
20. An oil spill spreads in a circle. When the radius is $20$ meters, it's growing at $0.5$ meters per minute. Find the rate of change of the spill's area at that moment.
21. A city's population is currently $5000$ people, growing at $200$ people per year. Its developed area is currently $25$ square miles, growing at $3$ square miles per year. Using $D=\dfrac{P}{A}$ for population density, find the rate of change of density at this moment.
22. A weather balloon is being filled with helium at a rate of $100$ ft³/min. Find the rate of change of the radius at the moment the radius is $5$ ft.
