# Cheat Sheet: Related Rates vs. Optimization

## Why these two get confused

Both topics show up as word problems with geometry (rectangles, cones, ladders, boxes), both use derivatives, and both can *sound* similar on a quick read. But they're asking fundamentally different questions, and mixing up the approach wastes a lot of time. This sheet is a fast way to sort a problem into the right bucket before you start solving.

---

## The one-question test

**Ask: is something changing over time, with a rate already given to you?**

- **Yes, and I need to find a *different* rate at a specific instant** $\rightarrow$ **Related Rates**
- **No — I just need to find the single best (biggest/smallest/cheapest/optimal) value, no rates involved** $\rightarrow$ **Optimization**

---

## Related Rates — the signals

- The problem gives you at least one rate already (a $\dfrac{dx}{dt}$ or $\dfrac{dr}{dt}$, phrased as "increasing at," "decreasing at," "moving at").
- It asks "how fast is [something] changing" or "at what rate."
- Multiple quantities are all changing **at the same time**, tied together by a geometric or physical equation.
- The final answer is a **rate** — it has "per unit time" in its units (ft/s, gal/min, rad/s, etc.).

**Example phrasing:** *"A ladder is sliding down a wall... the bottom is moving away at 2 ft/s... how fast is the top sliding down when..."*

**The approach:** find an equation connecting the variables, differentiate both sides with respect to $t$ (implicit differentiation in disguise), then plug in the specific instant's values — **never plug in numbers before differentiating.**

---

## Optimization — the signals

- The problem asks you to **maximize** or **minimize** something — biggest area, smallest cost, least material, greatest volume, highest profit.
- There's usually a **constraint** (a fixed amount of fencing, a fixed budget, a fixed volume) tying two variables together.
- Nothing is described as changing over time — you're looking for one best, unchanging value.
- The final answer is a **value** — a dimension, a price, an amount — not a rate.

**Example phrasing:** *"A farmer has 400 m of fencing... find the dimensions that give the largest possible area."*

**The approach:** write the objective as a function of one variable (using the constraint to eliminate the other variable), differentiate, set the derivative to $0$, and confirm it's actually a max or min.

---

## The trap: when "time" language shows up in an optimization problem

Some optimization problems still mention $t$ (time) as the single variable — for example, "find the time $t$ that minimizes cost." **This is still optimization, not related rates**, because there's only **one** quantity varying (cost, as a function of $t$), not multiple linked rates. The test still applies: are you given a rate and asked for another rate (related rates), or are you finding one best value (optimization)? If it's the second, treat $t$ just like any other variable and optimize normally.

---

## Side-by-side comparison

| | Related Rates | Optimization |
|---|---|---|
| What's given | A known rate at some instant | A fixed constraint (budget, material, etc.) |
| What's asked | A different rate, at that same instant | The single best value of some quantity |
| Key tool | Implicit differentiation w.r.t. $t$ | Setting $f'(x)=0$, then confirming max/min |
| When to plug in numbers | **After** differentiating, never before | After finding the critical point |
| Answer's units | Rate (per unit time) | A plain value (length, dollars, etc.) |
