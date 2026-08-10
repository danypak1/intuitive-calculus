# Unit 6: Limits Involving Infinity; Asymptotes — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\lim_{x\to\infty}\frac{3x+5}{2x-1}$

Top degree $=1$, bottom degree $=1$ — same degree. Divide every term by $x$ (the highest power in the denominator):

$$\frac{3+\frac{5}{x}}{2-\frac{1}{x}}$$

As $x\to\infty$, $\frac{5}{x}\to 0$ and $\frac{1}{x}\to 0$:

$$\frac{3+0}{2-0} = \frac{3}{2}$$

**Answer: $\dfrac{3}{2}$.**

**2.** $\displaystyle\lim_{x\to\infty}\frac{2x+1}{x^2+3}$

Top degree $=1$, bottom degree $=2$ — top is smaller. By the rule, the limit is $0$.

(To see it: divide by $x^2$: $\dfrac{\frac{2}{x}+\frac{1}{x^2}}{1+\frac{3}{x^2}} \to \dfrac{0+0}{1+0} = 0$.)

**Answer: $0$.**

**3.** $\displaystyle\lim_{x\to\infty}\frac{x^3+2}{5x^2-1}$

Top degree $=3$, bottom degree $=2$ — top is bigger. By the rule, this limit is $+\infty$ (grows without bound).

(To see it: divide by $x^2$: $\dfrac{x+\frac{2}{x^2}}{5-\frac{1}{x^2}} \to \dfrac{x+0}{5-0}$, and as $x\to\infty$ this keeps growing forever.)

**Answer: $+\infty$ (no finite limit — the fraction grows without bound).**

**4.** $\displaystyle\lim_{x\to-\infty}\frac{4x^2-3}{2x^2+7}$

Same degree top and bottom ($2$ and $2$). Divide by $x^2$:

$$\frac{4-\frac{3}{x^2}}{2+\frac{7}{x^2}} \to \frac{4-0}{2+0} = \frac{4}{2}=2$$

(Since $x^2$ is positive whether $x\to\infty$ or $x\to-\infty$, the answer is the same either direction.)

**Answer: $2$.**

**5.** $\displaystyle\lim_{x\to\infty}\frac{5}{x^3}$

This is exactly the basic pattern $\dfrac{c}{x^n}\to 0$.

**Answer: $0$.**

**6.** $\displaystyle\lim_{x\to\infty}\frac{7x^2-2x+1}{3x^2+4x-5}$

Same degree top and bottom ($2$ and $2$). Divide by $x^2$:

$$\frac{7-\frac{2}{x}+\frac{1}{x^2}}{3+\frac{4}{x}-\frac{5}{x^2}} \to \frac{7-0+0}{3+0-0} = \frac{7}{3}$$

**Answer: $\dfrac{7}{3}$.**

---

### 🟡 Standard

**7.** $\displaystyle\lim_{x\to\infty}\frac{5x^2+8x-3}{3x^2+2}$

Same degree top and bottom ($2$ and $2$). Divide by $x^2$:

$$\frac{5+\frac{8}{x}-\frac{3}{x^2}}{3+\frac{2}{x^2}} \to \frac{5+0-0}{3+0} = \frac{5}{3}$$

**Answer: $\dfrac{5}{3}$.**

**8.** $y=\dfrac{2x-7}{x+4}$

Top degree $=1$, bottom degree $=1$ — same degree, so the horizontal asymptote is the ratio of leading coefficients:

$$y = \frac{2}{1} = 2$$

**Answer: horizontal asymptote $y=2$.**

**9.** $y=\dfrac{3x^2+1}{x^2-5x+6}$

Same degree ($2$ and $2$), so the horizontal asymptote is the ratio of leading coefficients:

$$y = \frac{3}{1} = 3$$

**Answer: horizontal asymptote $y=3$.**

**10.** $y=\dfrac{x+2}{x^2-9}$

Top degree $=1$, bottom degree $=2$ — top is smaller, so the horizontal asymptote is $y=0$.

**Answer: horizontal asymptote $y=0$.**

**11.** $y=\dfrac{x+1}{x^2-4}$

Factor the denominator: $x^2-4 = (x-2)(x+2)$, which is zero at $x=2$ and $x=-2$.

Check the numerator at these values: at $x=2$, $2+1=3\ne 0$; at $x=-2$, $-2+1=-1\ne0$. Neither factor cancels.

**Answer: vertical asymptotes at $x=2$ and $x=-2$.**

**12.** $y=\dfrac{2x}{x^2+x-6}$

Factor the denominator: we need two numbers multiplying to $-6$ and adding to $1$: those are $3$ and $-2$.

$$x^2+x-6 = (x+3)(x-2)$$

Zero at $x=-3$ and $x=2$.

Check the numerator ($2x$) at these values: at $x=-3$, $2(-3)=-6\ne0$; at $x=2$, $2(2)=4\ne0$. Neither cancels.

**Answer: vertical asymptotes at $x=-3$ and $x=2$.**

---

### 🔴 Challenge

**13.** $y = \dfrac{(x+3)(x+1)}{(x+2)(x-1)}$

**Horizontal asymptote:** if you multiplied everything out, the top would be $x^2+\dots$ and the bottom would be $x^2+\dots$ — same degree ($2$ and $2$), both with leading coefficient $1$. So the horizontal asymptote is:

$$y = \frac{1}{1} = 1$$

**Vertical asymptotes:** the denominator is zero at $x=-2$ and $x=1$. Check whether either factor also makes the numerator zero:

At $x=-2$: numerator $=(-2+3)(-2+1) = (1)(-1) = -1 \ne 0$.

At $x=1$: numerator $=(1+3)(1+1) = (4)(2) = 8 \ne 0$.

Neither cancels.

**Answer: horizontal asymptote $y=1$; vertical asymptotes at $x=-2$ and $x=1$.**

**14.** $y = \dfrac{(x-2)(x+5)}{(x-2)(x+3)}$

Notice the factor $(x-2)$ appears in **both** the top and bottom — it cancels!

$$y = \frac{(x-2)(x+5)}{(x-2)(x+3)} = \frac{x+5}{x+3} \quad (\text{for } x\ne 2)$$

**Vertical asymptote:** using the simplified form, the denominator is zero at $x=-3$. Check the (simplified) numerator there: $-3+5=2\ne0$, so this is a genuine vertical asymptote.

At $x=2$: since the $(x-2)$ factor canceled, this is **not** a vertical asymptote — it's a **removable hole** in the graph instead.

**Horizontal asymptote:** using the simplified form $\dfrac{x+5}{x+3}$, same degree top and bottom, leading coefficients both $1$:

$$y = 1$$

**Answer: horizontal asymptote $y=1$; vertical asymptote at $x=-3$; removable hole (not an asymptote) at $x=2$.**

**15.** $y = \dfrac{x^2-1}{x^2-4x+3}$

Factor the top (difference of squares): $x^2-1=(x-1)(x+1)$.

Factor the bottom: numbers multiplying to $3$, adding to $-4$: $-1$ and $-3$.

$$x^2-4x+3 = (x-1)(x-3)$$

The factor $(x-1)$ cancels:

$$y = \frac{(x-1)(x+1)}{(x-1)(x-3)} = \frac{x+1}{x-3} \quad (\text{for } x\ne 1)$$

**Vertical asymptote:** using the simplified form, the denominator is zero at $x=3$. Check the numerator there: $3+1=4\ne 0$, so this is genuine.

At $x=1$: since $(x-1)$ canceled, this is a **removable hole**, not a vertical asymptote.

**Horizontal asymptote:** simplified form $\dfrac{x+1}{x-3}$, same degree, leading coefficients both $1$:

$$y=1$$

**Answer: horizontal asymptote $y=1$; vertical asymptote at $x=3$; removable hole (not an asymptote) at $x=1$.**

**16.** $y = \dfrac{3x^2-12}{x^2-x-2}$

Factor the top: $3x^2-12 = 3(x^2-4) = 3(x-2)(x+2)$.

Factor the bottom: numbers multiplying to $-2$, adding to $-1$: $-2$ and $1$.

$$x^2-x-2 = (x-2)(x+1)$$

The factor $(x-2)$ cancels:

$$y = \frac{3(x-2)(x+2)}{(x-2)(x+1)} = \frac{3(x+2)}{x+1} \quad (\text{for } x\ne 2)$$

**Vertical asymptote:** using the simplified form, the denominator is zero at $x=-1$. Check the numerator there: $3(-1+2) = 3(1) = 3 \ne 0$, so this is genuine.

At $x=2$: since $(x-2)$ canceled, this is a **removable hole**, not a vertical asymptote.

**Horizontal asymptote:** from the original (or simplified) form, comparing leading coefficients of the top ($3$) and bottom ($1$) of the same degree:

$$y = 3$$

**Answer: horizontal asymptote $y=3$; vertical asymptote at $x=-1$; removable hole (not an asymptote) at $x=2$.**

**17.** $y = \dfrac{1}{x-2}$

**Horizontal asymptote:** top degree $0$ (a constant), bottom degree $1$ — top is smaller, so:

$$y = 0$$

**As $x\to 2^+$** (values just a bit bigger than $2$, like $2.001$): $x-2$ is a very small **positive** number, so $\dfrac{1}{x-2}$ is a very large **positive** number.

$$\lim_{x\to 2^+}\frac{1}{x-2} = +\infty$$

**As $x\to 2^-$** (values just a bit smaller than $2$, like $1.999$): $x-2$ is a very small **negative** number, so $\dfrac{1}{x-2}$ is a very large **negative** number.

$$\lim_{x\to 2^-}\frac{1}{x-2} = -\infty$$

**Answer: horizontal asymptote $y=0$. As $x\to2^+$, $y\to+\infty$; as $x\to2^-$, $y\to-\infty$.** (There's a vertical asymptote at $x=2$, and the graph shoots off in opposite directions on each side of it.)

---

### 🌍 Applied

**18.** $C(x) = \dfrac{500+3x}{x}$, find the horizontal asymptote as $x\to\infty$.

Rewrite it as two separate fractions: $C(x) = \dfrac{500}{x} + 3$.

As $x\to\infty$, $\dfrac{500}{x}\to 0$, so:

$$C(x) \to 0+3 = 3$$

**Answer: horizontal asymptote $y=3$.** This means that as the company produces more and more units, the average cost per unit gets closer and closer to $\$3$ — the fixed cost of $\$500$ gets "spread out" over so many units that it barely affects the per-unit average anymore, leaving just the $\$3$ variable cost per unit.

**19.** $C(t) = \dfrac{50t}{t^2+25}$, find the horizontal asymptote as $t\to\infty$.

Top degree $=1$, bottom degree $=2$ — top is smaller, so the limit is $0$.

**Answer: horizontal asymptote $y=0$.** This means that over a very long time, the drug concentration in the bloodstream approaches $0$ — the body eventually clears the drug out almost entirely.

**20.** $P(t) = \dfrac{200t+500}{t+2}$, find the horizontal asymptote as $t\to\infty$.

Same degree top and bottom ($1$ and $1$), so the horizontal asymptote is the ratio of leading coefficients:

$$y = \frac{200}{1} = 200$$

**Answer: horizontal asymptote $y=200$.** This suggests that in the very long run, the city's population levels off and approaches about $200$ thousand people, rather than growing forever.

**21.** $R(x) = \dfrac{10x}{x+5}$, find the horizontal asymptote as $x\to\infty$.

Same degree top and bottom ($1$ and $1$):

$$y = \frac{10}{1} = 10$$

**Answer: horizontal asymptote $y=10$.** This means that no matter how many resources the factory has available, the production rate can never exceed (and gets closer and closer to) $10$ units per hour — there's a built-in ceiling on how fast the factory can produce, even with unlimited resources.
