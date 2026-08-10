# Unit 2: Limit of a Function and Limit Laws — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\lim_{x\to 3}(2x+1)$

This is a straight line — no division, no square roots, nothing tricky. Just plug in $x=3$:

$$2(3)+1 = 7$$

**Answer: $7$.**

**2.** $\displaystyle\lim_{x\to -2}(x^2-3x+4)$

Plug in $x=-2$ directly:

$$(-2)^2 - 3(-2) + 4 = 4 + 6 + 4 = 14$$

**Answer: $14$.**

**3.** $\displaystyle\lim_{x\to 1}(3x^2-2x+5)$

Plug in $x=1$:

$$3(1)^2 - 2(1) + 5 = 3-2+5 = 6$$

**Answer: $6$.**

**4.** $\displaystyle\lim_{x\to 0}(x^3+2x^2-1)$

Plug in $x=0$:

$$0 + 0 - 1 = -1$$

**Answer: $-1$.**

**5.** $\displaystyle\lim_{x\to 4}\sqrt{x+5}$

Plug in $x=4$:

$$\sqrt{4+5} = \sqrt{9} = 3$$

**Answer: $3$.**

**6.** $\displaystyle\lim_{x\to 2}\frac{x^2+1}{x+3}$

The denominator at $x=2$ is $2+3=5$, which is not zero, so we can just plug straight in:

$$\frac{2^2+1}{2+3} = \frac{5}{5} = 1$$

**Answer: $1$.**

**7.** $\displaystyle\lim_{x\to 5}\frac{x+5}{x^2-20}$

The denominator at $x=5$ is $25-20=5$, not zero, so direct substitution works:

$$\frac{5+5}{25-20} = \frac{10}{5} = 2$$

**Answer: $2$.**

---

### 🟡 Standard

**8.** $\displaystyle\lim_{x\to 2}\frac{x^2-7x+10}{x-2}$

Plugging in $x=2$ gives $\frac{4-14+10}{0} = \frac{0}{0}$ — a signal to factor.

Factor the top: we need two numbers that multiply to $10$ and add to $-7$: those are $-2$ and $-5$.

$$x^2-7x+10 = (x-2)(x-5)$$

So the fraction becomes:

$$\frac{(x-2)(x-5)}{x-2}$$

Cancel the common factor $(x-2)$ (allowed since we're looking at values *near*, not *at*, $x=2$):

$$x-5$$

Now plug in $x=2$: $2-5 = -3$.

**Answer: $-3$.**

**9.** $\displaystyle\lim_{x\to 3}\frac{x^2-9}{x-3}$

Plugging in gives $\frac{0}{0}$. Factor the top as a difference of squares:

$$x^2-9 = (x-3)(x+3)$$

Cancel $(x-3)$:

$$x+3$$

Plug in $x=3$: $3+3=6$.

**Answer: $6$.**

**10.** $\displaystyle\lim_{x\to -1}\frac{x^2+3x+2}{x+1}$

Plugging in gives $\frac{0}{0}$. Factor the top: need two numbers multiplying to $2$, adding to $3$: those are $1$ and $2$.

$$x^2+3x+2 = (x+1)(x+2)$$

Cancel $(x+1)$:

$$x+2$$

Plug in $x=-1$: $-1+2=1$.

**Answer: $1$.**

**11.** $\displaystyle\lim_{x\to 4}\frac{x^2-16}{x-4}$

Plugging in gives $\frac{0}{0}$. Factor as difference of squares:

$$x^2-16 = (x-4)(x+4)$$

Cancel $(x-4)$:

$$x+4$$

Plug in $x=4$: $4+4=8$.

**Answer: $8$.**

**12.** $\displaystyle\lim_{x\to 1}\frac{x^3-1}{x-1}$

Plugging in gives $\frac{0}{0}$. Use the "difference of cubes" pattern: $a^3-b^3=(a-b)(a^2+ab+b^2)$, with $a=x$, $b=1$:

$$x^3-1 = (x-1)(x^2+x+1)$$

Cancel $(x-1)$:

$$x^2+x+1$$

Plug in $x=1$: $1+1+1=3$.

**Answer: $3$.**

**13.** $\displaystyle\lim_{x\to 2}\frac{x^2-5x+6}{x^2-4}$

Plugging in gives $\frac{4-10+6}{4-4} = \frac{0}{0}$.

Factor the top: numbers multiplying to $6$, adding to $-5$: $-2$ and $-3$.

$$x^2-5x+6 = (x-2)(x-3)$$

Factor the bottom as a difference of squares:

$$x^2-4 = (x-2)(x+2)$$

So the fraction is:

$$\frac{(x-2)(x-3)}{(x-2)(x+2)}$$

Cancel $(x-2)$:

$$\frac{x-3}{x+2}$$

Plug in $x=2$: $\dfrac{2-3}{2+2} = \dfrac{-1}{4}$.

**Answer: $-\dfrac{1}{4}$.**

**14.** $\displaystyle\lim_{x\to 3}\frac{x^2-2x-3}{x^2-9}$

Plugging in gives $\frac{9-6-3}{0} = \frac{0}{0}$.

Factor the top: numbers multiplying to $-3$, adding to $-2$: $-3$ and $1$.

$$x^2-2x-3 = (x-3)(x+1)$$

Factor the bottom:

$$x^2-9 = (x-3)(x+3)$$

Cancel $(x-3)$:

$$\frac{x+1}{x+3}$$

Plug in $x=3$: $\dfrac{3+1}{3+3} = \dfrac{4}{6} = \dfrac{2}{3}$.

**Answer: $\dfrac{2}{3}$.**

---

### 🔴 Challenge

**15.** $\displaystyle\lim_{x\to 4}\frac{x-4}{\sqrt{x}-2}$

Plugging in gives $\frac{0}{0}$. There's a square root in the denominator, so we rationalize by multiplying top and bottom by the conjugate $\sqrt{x}+2$:

$$\frac{x-4}{\sqrt{x}-2}\cdot\frac{\sqrt{x}+2}{\sqrt{x}+2} = \frac{(x-4)(\sqrt{x}+2)}{(\sqrt{x}-2)(\sqrt{x}+2)}$$

The denominator becomes $(\sqrt{x})^2 - 2^2 = x-4$ (this is exactly why we picked the conjugate — it clears the square root).

$$\frac{(x-4)(\sqrt{x}+2)}{x-4}$$

Cancel $(x-4)$:

$$\sqrt{x}+2$$

Plug in $x=4$: $\sqrt{4}+2 = 2+2=4$.

**Answer: $4$.**

**16.** $\displaystyle\lim_{x\to 2}\frac{\sqrt{x^2+12}-4}{x-2}$

Plugging in gives $\frac{0}{0}$. Rationalize by multiplying by the conjugate $\sqrt{x^2+12}+4$:

$$\frac{\sqrt{x^2+12}-4}{x-2}\cdot\frac{\sqrt{x^2+12}+4}{\sqrt{x^2+12}+4} = \frac{(x^2+12)-16}{(x-2)\big(\sqrt{x^2+12}+4\big)}$$

Simplify the top: $x^2+12-16 = x^2-4 = (x-2)(x+2)$.

$$\frac{(x-2)(x+2)}{(x-2)\big(\sqrt{x^2+12}+4\big)}$$

Cancel $(x-2)$:

$$\frac{x+2}{\sqrt{x^2+12}+4}$$

Plug in $x=2$: $\dfrac{2+2}{\sqrt{4+12}+4} = \dfrac{4}{\sqrt{16}+4} = \dfrac{4}{4+4} = \dfrac{4}{8} = \dfrac{1}{2}$.

**Answer: $\dfrac{1}{2}$.**

**17.** $\displaystyle\lim_{x\to 0}\frac{\sqrt{x+9}-3}{x}$

Plugging in gives $\frac{0}{0}$. Rationalize with the conjugate $\sqrt{x+9}+3$:

$$\frac{\sqrt{x+9}-3}{x}\cdot\frac{\sqrt{x+9}+3}{\sqrt{x+9}+3} = \frac{(x+9)-9}{x\big(\sqrt{x+9}+3\big)} = \frac{x}{x\big(\sqrt{x+9}+3\big)}$$

Cancel $x$:

$$\frac{1}{\sqrt{x+9}+3}$$

Plug in $x=0$: $\dfrac{1}{\sqrt{9}+3} = \dfrac{1}{3+3} = \dfrac{1}{6}$.

**Answer: $\dfrac{1}{6}$.**

**18.** $\displaystyle\lim_{x\to 9}\frac{x-9}{\sqrt{x}-3}$

Plugging in gives $\frac{0}{0}$. Rationalize with the conjugate $\sqrt{x}+3$:

$$\frac{x-9}{\sqrt{x}-3}\cdot\frac{\sqrt{x}+3}{\sqrt{x}+3} = \frac{(x-9)(\sqrt{x}+3)}{x-9}$$

Cancel $(x-9)$:

$$\sqrt{x}+3$$

Plug in $x=9$: $\sqrt{9}+3 = 3+3=6$.

**Answer: $6$.**

**19.** $\displaystyle\lim_{h\to 0}\frac{(2+h)^2-4}{h}$

Expand the top: $(2+h)^2 = 4+4h+h^2$, so the top becomes $4+4h+h^2-4 = 4h+h^2$.

$$\frac{4h+h^2}{h}$$

Cancel one $h$ from each term:

$$4+h$$

Let $h\to 0$: $4+0=4$.

**Answer: $4$.** (This is the exact same style of computation you used in Unit 1 to find a tangent slope — that's not a coincidence; it's the same skill in a new outfit.)

**20.** $\displaystyle\lim_{x\to 1}\frac{\frac{1}{x}-1}{x-1}$

The top is itself a small fraction problem. Combine $\dfrac{1}{x}-1$ into a single fraction using a common denominator of $x$:

$$\frac{1}{x}-1 = \frac{1-x}{x}$$

So the whole expression becomes:

$$\frac{\frac{1-x}{x}}{x-1} = \frac{1-x}{x(x-1)}$$

Notice that $1-x = -(x-1)$. Rewrite the top that way:

$$\frac{-(x-1)}{x(x-1)}$$

Cancel $(x-1)$:

$$\frac{-1}{x}$$

Plug in $x=1$: $\dfrac{-1}{1} = -1$.

**Answer: $-1$.**

---

### 🌍 Applied

**21.** $R(x) = 5x-0.01x^2$, find $\displaystyle\lim_{x\to 10}R(x)$.

This is a polynomial, so direct substitution works — no tricks needed:

$$R(10) = 5(10) - 0.01(10)^2 = 50 - 0.01(100) = 50-1 = 49$$

**Answer: $49$.** This means that as production gets closer and closer to $10$ units, the revenue gets closer and closer to $\$49$.

**22.** $C(x)=200+3x$. Find $\displaystyle\lim_{x\to 50}\dfrac{C(x)}{x}$.

At $x=50$, the denominator is $50$, which isn't zero, so direct substitution works:

$$\frac{C(50)}{50} = \frac{200+3(50)}{50} = \frac{200+150}{50} = \frac{350}{50} = 7$$

**Answer: $7$.** As production nears $50$ items, the average cost per item approaches $\$7$.

**23.** $P(t) = \dfrac{100t}{t+5}$. Find $\displaystyle\lim_{t\to 5}P(t)$.

At $t=5$, the denominator is $10$, which isn't zero, so direct substitution works:

$$\frac{100(5)}{5+5} = \frac{500}{10} = 50$$

**Answer: $50$ (thousand bacteria).** As time nears $5$ hours, the population approaches $50{,}000$ bacteria.

**24.** $v(t) = \dfrac{t^2-4}{t-2}$. Find $\displaystyle\lim_{t\to 2}v(t)$.

Plugging in $t=2$ directly gives $\frac{0}{0}$, confirming the model formula itself breaks down at $t=2$. But we can still find what it's approaching by factoring:

$$t^2-4 = (t-2)(t+2)$$

$$\frac{(t-2)(t+2)}{t-2}$$

Cancel $(t-2)$:

$$t+2$$

Plug in $t=2$: $2+2=4$.

**Answer: $4$.** Even though the formula for $v(t)$ doesn't technically produce a value right at $t=2$ (it's a $\frac{0}{0}$ gap in the model), the velocity is clearly heading toward $4$ as $t$ gets closer and closer to $2$ from either side — so it's very reasonable to say the object's velocity is essentially $4$ at that moment.
