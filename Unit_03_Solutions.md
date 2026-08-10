# Unit 3: The Precise Definition of a Limit — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=2x$, $a=3$, $L=6$, $\varepsilon=0.4$.

Here the slope is $m=2$. Using the shortcut $\delta = \dfrac{\varepsilon}{|m|}$:

$$\delta = \frac{0.4}{2} = 0.2$$

**Answer: $\delta = 0.2$.** (As long as $x$ stays within $0.2$ of $3$, $f(x)$ stays within $0.4$ of $6$.)

**2.** $f(x)=5x$, $a=2$, $L=10$, $\varepsilon=1$.

Slope $m=5$.

$$\delta = \frac{1}{5} = 0.2$$

**Answer: $\delta = 0.2$.**

**3.** $f(x)=-3x$, $a=1$, $L=-3$, $\varepsilon=0.6$.

Slope $m=-3$, so $|m|=3$ (the sign doesn't matter here, only the size).

$$\delta = \frac{0.6}{3} = 0.2$$

**Answer: $\delta = 0.2$.**

**4.** $f(x)=x+4$, $a=5$, $L=9$, $\varepsilon=0.3$.

Slope $m=1$.

$$\delta = \frac{0.3}{1} = 0.3$$

**Answer: $\delta = 0.3$.** (When the slope is exactly $1$, delta and epsilon always match.)

**5.** Which line needs the smaller delta if both have the same epsilon, but one is steeper?

**The steeper line (larger $|m|$) needs the *smaller* delta.** Here's why: a steep line takes a small change in $x$ and stretches it into a much bigger change in $y$ — think of it like a lever that amplifies a small push into a big swing. So to keep the *output* change small (within $\varepsilon$), you have to control the *input* change even more tightly. That's exactly why $\delta = \varepsilon/|m|$ has $|m|$ on the bottom: a bigger $|m|$ makes $\delta$ smaller.

**6.** If someone tightens epsilon, what happens to delta?

**Delta must also get smaller (or stay the same at most).** Since $\delta = \varepsilon/|m|$, shrinking $\varepsilon$ directly shrinks $\delta$ (for a fixed slope). This makes sense with the tolerance-game picture: if someone demands a narrower target band on the output, you have to squeeze your input window tighter to still guarantee landing inside it.

---

### 🟡 Standard

**7.** $f(x)=4x-1$, $a=2$, $L=7$, $\varepsilon=0.8$.

Slope $m=4$.

$$\delta = \frac{0.8}{4} = 0.2$$

**Answer: $\delta = 0.2$.**

**8.** $f(x)=-2x+5$, $a=3$, $L=-1$, $\varepsilon=0.5$.

Slope $m=-2$, so $|m|=2$.

$$\delta = \frac{0.5}{2} = 0.25$$

**Answer: $\delta = 0.25$.**

**9.** $f(x)=6x+2$, $a=-1$, $L=-4$, $\varepsilon=1.2$.

Slope $m=6$.

$$\delta = \frac{1.2}{6} = 0.2$$

**Answer: $\delta = 0.2$.**

**10.** $f(x)=3x$, $a=0$, $\varepsilon=0.09$.

Slope $m=3$.

$$\delta = \frac{0.09}{3} = 0.03$$

**Answer: $\delta = 0.03$.**

**11.** $f(x)=2x+1$, $a=4$, $\delta=0.15$. Find the resulting $\varepsilon$.

Here we work backward using $\varepsilon = |m|\cdot\delta$, with slope $m=2$:

$$\varepsilon = 2 \times 0.15 = 0.3$$

First find $L$: $L = f(4) = 2(4)+1 = 9$.

**Answer: $\varepsilon = 0.3$.** In words: whenever $x$ stays within $0.15$ of $4$, $f(x)$ is guaranteed to stay within $0.3$ of $9$ — that is, $f(x)$ stays strictly between $8.7$ and $9.3$.

**12.** $f(x)=-4x+3$, $a=1$, $\delta=0.1$. Find the resulting $\varepsilon$.

Slope $m=-4$, so $|m|=4$.

$$\varepsilon = 4 \times 0.1 = 0.4$$

Find $L$: $L=f(1) = -4(1)+3 = -1$.

**Answer: $\varepsilon = 0.4$.** In words: whenever $x$ stays within $0.1$ of $1$, $f(x)$ is guaranteed to stay within $0.4$ of $-1$ — that is, $f(x)$ stays strictly between $-1.4$ and $-0.6$.

---

### 🔴 Challenge

**13.** $f(x)=7x-3$, $a=2$, $\varepsilon=0.35$.

Slope $m=7$.

$$\delta = \frac{0.35}{7} = 0.05$$

Find $L$: $L = f(2) = 14-3 = 11$.

**Check at $x = a+\delta = 2.05$:**

$$f(2.05) = 7(2.05)-3 = 14.35-3 = 11.35$$

$$|11.35 - 11| = 0.35 \quad \checkmark \text{ (right at the edge of the band, as expected)}$$

**Check at $x = a-\delta = 1.95$:**

$$f(1.95) = 7(1.95)-3 = 13.65-3 = 10.65$$

$$|10.65-11| = 0.35 \quad \checkmark \text{ (also right at the edge)}$$

**Answer: $\delta=0.05$**, and both boundary checks confirm $f(x)$ lands exactly on the edge of the $\pm 0.35$ tolerance band around $L=11$ — any $x$ *strictly* inside the $\delta$-window gives an $f(x)$ *strictly* inside the band, exactly as promised.

**14.** $f(x)=3x+1$, $a=2$, $L=7$, $\varepsilon=0.6$, with an extra requirement that $x$ stay within $0.15$ of $a$.

First, the shortcut formula's delta: slope $m=3$,

$$\delta_{\text{formula}} = \frac{0.6}{3} = 0.2$$

But we're also told $x$ must stay within $0.15$ of $a=2$ for a separate reason. We have two requirements:

- Requirement 1 (epsilon-matching): $\delta \le 0.2$
- Requirement 2 (physical constraint): $\delta \le 0.15$

**Answer: use $\delta = 0.15$**, the *smaller* of the two. This is because whatever delta you pick has to satisfy *both* requirements at once — picking the larger one ($0.2$) would violate the physical constraint. When you have more than one condition to satisfy, you always take the tightest (smallest) delta among them, since a smaller delta automatically still satisfies any looser requirement.

**15.** $f(x)=-5x+2$, $a=-2$, $\varepsilon=0.25$.

First find $L$: $L = f(-2) = -5(-2)+2 = 10+2=12$.

Slope $m=-5$, so $|m|=5$.

$$\delta = \frac{0.25}{5} = 0.05$$

**Is $\delta=0.02$ also valid?**

**Yes.** Since $0.02 < 0.05$, using $\delta=0.02$ means we're restricting $x$ to an *even tighter* window around $a=-2$ than we strictly needed to. A tighter input window can only make $f(x)$ land even closer to $L$, never farther — so any delta smaller than the one given by the shortcut formula still works. There's no single "correct" delta; $0.05$ is just the largest one that's guaranteed to work.

**16.** $f(x)=2x$ near $a=3$, with $f(x)$ required to stay strictly between $5.7$ and $6.3$.

First, find $L$: since the band is symmetric, $L$ is the midpoint:

$$L = \frac{5.7+6.3}{2} = \frac{12}{2} = 6$$

(This matches $f(3) = 2(3) = 6$, as expected.)

Find $\varepsilon$: it's the distance from $L$ to either edge:

$$\varepsilon = 6.3 - 6 = 0.3 \quad \text{(or equivalently } 6 - 5.7 = 0.3\text{)}$$

Now find the matching $\delta$, using slope $m=2$:

$$\delta = \frac{0.3}{2} = 0.15$$

**Answer: $\varepsilon = 0.3$ and $\delta = 0.15$.**

---

### 🌍 Applied

**17.** Rod-cutting: $f(x)=2x$, target $L=6$ m at $a=3$, tolerance $\varepsilon=0.02$ m.

Slope $m=2$.

$$\delta = \frac{0.02}{2} = 0.01$$

**Answer: the dial must be set within $0.01$ units of $3$** to guarantee the rod comes out within $0.02$ m of the $6$ m target.

**18.** Thermostat: $T(x)=3x+65$, target $L=71°F$ at $a=2$, tolerance $\varepsilon=0.9°F$.

Slope $m=3$.

$$\delta = \frac{0.9}{3} = 0.3$$

**Answer: the dial must be set within $0.3$ units of $2$** to guarantee the room stays within $0.9°F$ of $71°F$.

**19.** Pharmacist: $C(x)=4x+10$, target $L=26$ mg/mL at $a=4$, tolerance $\varepsilon=0.5$ mg/mL.

Slope $m=4$.

$$\delta = \frac{0.5}{4} = 0.125$$

**Answer: $x$ must be measured within $0.125$ mL of $4$ mL** to guarantee the concentration stays within $0.5$ mg/mL of $26$ mg/mL.

**20.** Drone: $h(x)=10x$, target $L=50$ m at $a=5$, tolerance $\varepsilon=2$ m.

Slope $m=10$.

$$\delta = \frac{2}{10} = 0.2$$

**Answer: the throttle setting must be controlled within $0.2$ units of $5$** to guarantee the altitude stays within $2$ m of $50$ m, keeping the drone clear of the restricted zone.
