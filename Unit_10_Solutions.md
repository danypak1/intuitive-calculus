# Unit 10: Product Rule & Quotient Rule — Full Solutions

### 🟢 Warm-up

**1.** $y=(x^2)(x+3)$

Let $f=x^2$ (so $f'=2x$) and $g=x+3$ (so $g'=1$).

$$y' = f'g + fg' = 2x(x+3) + x^2(1) = 2x^2+6x+x^2 = 3x^2+6x$$

**$y' = 3x^2+6x$.** (Double-check by expanding first: $x^2(x+3)=x^3+3x^2$, and its derivative is $3x^2+6x$ — matches!)

**2.** $y=(2x+1)(x-4)$

$f=2x+1$ ($f'=2$), $g=x-4$ ($g'=1$).

$$y' = 2(x-4) + (2x+1)(1) = 2x-8+2x+1 = 4x-7$$

**$y' = 4x-7$.**

**3.** $y=(x^2+1)(x-2)$

$f=x^2+1$ ($f'=2x$), $g=x-2$ ($g'=1$).

$$y' = 2x(x-2) + (x^2+1)(1) = 2x^2-4x+x^2+1 = 3x^2-4x+1$$

**$y' = 3x^2-4x+1$.**

**4.** $y=\dfrac{x+1}{x-1}$

$f=x+1$ ($f'=1$), $g=x-1$ ($g'=1$).

$$y' = \frac{1\cdot(x-1) - (x+1)\cdot 1}{(x-1)^2} = \frac{(x-1)-(x+1)}{(x-1)^2} = \frac{-2}{(x-1)^2}$$

**$y' = -\dfrac{2}{(x-1)^2}$.**

**5.** $y=\dfrac{3x-2}{x+5}$

$f=3x-2$ ($f'=3$), $g=x+5$ ($g'=1$).

$$y' = \frac{3(x+5) - (3x-2)(1)}{(x+5)^2} = \frac{3x+15-3x+2}{(x+5)^2} = \frac{17}{(x+5)^2}$$

**$y' = \dfrac{17}{(x+5)^2}$.**

**6.** $y=\dfrac{x^2}{x+1}$

$f=x^2$ ($f'=2x$), $g=x+1$ ($g'=1$).

$$y' = \frac{2x(x+1) - x^2(1)}{(x+1)^2} = \frac{2x^2+2x-x^2}{(x+1)^2} = \frac{x^2+2x}{(x+1)^2}$$

**$y' = \dfrac{x^2+2x}{(x+1)^2}$.**

**7.** $y=(x-3)(x^2+2)$

$f=x-3$ ($f'=1$), $g=x^2+2$ ($g'=2x$).

$$y' = 1\cdot(x^2+2) + (x-3)(2x) = x^2+2+2x^2-6x = 3x^2-6x+2$$

**$y' = 3x^2-6x+2$.**

---

### 🟡 Standard

**8.** $y=(x^2+1)\left(x+1+\dfrac{1}{x}\right)$

Rewrite the second factor using powers: $g = x+1+x^{-1}$, so $g' = 1-x^{-2}$.

Let $f=x^2+1$ ($f'=2x$).

$$y' = 2x\left(x+1+\frac{1}{x}\right) + (x^2+1)\left(1-\frac{1}{x^2}\right)$$

Expand the first piece: $2x\cdot x + 2x\cdot 1 + 2x\cdot\frac{1}{x} = 2x^2+2x+2$.

Expand the second piece: $(x^2+1)(1) - (x^2+1)\cdot\frac{1}{x^2} = x^2+1 - \left(1+\frac{1}{x^2}\right) = x^2+1-1-\frac{1}{x^2} = x^2-\frac{1}{x^2}$.

Add them together:

$$y' = \left(2x^2+2x+2\right) + \left(x^2-\frac{1}{x^2}\right) = 3x^2+2x+2-\frac{1}{x^2}$$

**$y' = 3x^2+2x+2-\dfrac{1}{x^2}$.**

**9.** $y=\dfrac{x+5}{3x+2}$

$f=x+5$ ($f'=1$), $g=3x+2$ ($g'=3$).

$$y' = \frac{1\cdot(3x+2) - (x+5)(3)}{(3x+2)^2} = \frac{3x+2-3x-15}{(3x+2)^2} = \frac{-13}{(3x+2)^2}$$

**$y' = -\dfrac{13}{(3x+2)^2}$.**

**10.** $y=\dfrac{x^2-3}{2x+1}$

$f=x^2-3$ ($f'=2x$), $g=2x+1$ ($g'=2$).

$$y' = \frac{2x(2x+1) - (x^2-3)(2)}{(2x+1)^2} = \frac{4x^2+2x - 2x^2+6}{(2x+1)^2} = \frac{2x^2+2x+6}{(2x+1)^2}$$

**$y' = \dfrac{2x^2+2x+6}{(2x+1)^2}$.**

**11.** $y=(x+2)(x^2-3x+1)$

$f=x+2$ ($f'=1$), $g=x^2-3x+1$ ($g'=2x-3$).

$$y' = 1\cdot(x^2-3x+1) + (x+2)(2x-3)$$

Expand $(x+2)(2x-3) = 2x^2-3x+4x-6 = 2x^2+x-6$.

$$y' = (x^2-3x+1) + (2x^2+x-6) = 3x^2-2x-5$$

**$y' = 3x^2-2x-5$.**

**12.** $y=\left(\dfrac{1}{x}\right)(x^2+4)$

Rewrite: $f=x^{-1}$ ($f'=-x^{-2}$), $g=x^2+4$ ($g'=2x$).

$$y' = -x^{-2}(x^2+4) + x^{-1}(2x)$$

Simplify each piece: $-x^{-2}(x^2+4) = -1-4x^{-2}$. And $x^{-1}(2x) = 2$.

$$y' = (-1-4x^{-2}) + 2 = 1-\frac{4}{x^2}$$

**$y' = 1-\dfrac{4}{x^2}$.** (Check: simplifying first, $y=\dfrac{x^2+4}{x}=x+4x^{-1}$, and $y'=1-4x^{-2}$ — matches!)

**13.** $y=\dfrac{2x-1}{x^2+3}$

$f=2x-1$ ($f'=2$), $g=x^2+3$ ($g'=2x$).

$$y' = \frac{2(x^2+3) - (2x-1)(2x)}{(x^2+3)^2} = \frac{2x^2+6 - (4x^2-2x)}{(x^2+3)^2} = \frac{-2x^2+2x+6}{(x^2+3)^2}$$

**$y' = \dfrac{-2x^2+2x+6}{(x^2+3)^2}$.**

**14.** $y=(x^2+x)(3-x)$

$f=x^2+x$ ($f'=2x+1$), $g=3-x$ ($g'=-1$).

$$y' = (2x+1)(3-x) + (x^2+x)(-1)$$

Expand $(2x+1)(3-x) = 6x-2x^2+3-x = -2x^2+5x+3$.

$$y' = (-2x^2+5x+3) - (x^2+x) = -3x^2+4x+3$$

**$y' = -3x^2+4x+3$.**

---

### 🔴 Challenge

**15.** $y = \dfrac{(x^2+x)(x^2-x+1)}{x^4}$

This is much easier if we simplify first. Expand the numerator:

$$(x^2+x)(x^2-x+1) = x^2(x^2-x+1) + x(x^2-x+1)$$

$$= (x^4-x^3+x^2) + (x^3-x^2+x) = x^4-x^3+x^2+x^3-x^2+x$$

Notice the $-x^3$ and $+x^3$ cancel, and the $x^2$ and $-x^2$ cancel:

$$= x^4+x$$

So the whole function simplifies dramatically:

$$y = \frac{x^4+x}{x^4} = 1 + \frac{x}{x^4} = 1+x^{-3}$$

Now just differentiate:

$$y' = -3x^{-4} = -\frac{3}{x^4}$$

**$y' = -\dfrac{3}{x^4}$.** (This is a great example of why checking for simplification first can save you from a much messier quotient-rule computation!)

**16.** $y = \sqrt{x}\,(x^2-1)$

Rewrite: $f=x^{1/2}$ ($f' = \frac12 x^{-1/2}$), $g=x^2-1$ ($g'=2x$).

$$y' = \frac12 x^{-1/2}(x^2-1) + x^{1/2}(2x)$$

Write both pieces over a common denominator of $2\sqrt{x}$: the first piece is already $\dfrac{x^2-1}{2\sqrt{x}}$. The second piece, $2x\sqrt{x} = 2x^{3/2}$, can be rewritten as $\dfrac{4x^2}{2\sqrt{x}}$ (since $\frac{4x^2}{2\sqrt x} = 2x^2 x^{-1/2} = 2x^{3/2}$).

$$y' = \frac{(x^2-1) + 4x^2}{2\sqrt{x}} = \frac{5x^2-1}{2\sqrt{x}}$$

**$y' = \dfrac{5x^2-1}{2\sqrt{x}}$.**

**17.** $y = \dfrac{x^2-4}{\sqrt{x}}$

This is much easier if we simplify first by dividing each term by $\sqrt{x}=x^{1/2}$:

$$y = \frac{x^2}{x^{1/2}} - \frac{4}{x^{1/2}} = x^{3/2} - 4x^{-1/2}$$

Now differentiate:

$$y' = \frac{3}{2}x^{1/2} - 4\left(-\frac12\right)x^{-3/2} = \frac{3}{2}x^{1/2} + 2x^{-3/2}$$

**$y' = \dfrac{3}{2}\sqrt{x} + \dfrac{2}{x^{3/2}}$.** (Again, simplifying before differentiating was far cleaner than forcing the quotient rule here.)

**18.** $y = \left(x+\dfrac{1}{x}\right)(x^2-2)$

Rewrite: $f=x+x^{-1}$ ($f'=1-x^{-2}$), $g=x^2-2$ ($g'=2x$).

$$y' = (1-x^{-2})(x^2-2) + (x+x^{-1})(2x)$$

Expand the first piece: $(1)(x^2-2) - x^{-2}(x^2-2) = (x^2-2) - (1-2x^{-2}) = x^2-2-1+2x^{-2} = x^2-3+2x^{-2}$.

Expand the second piece: $2x\cdot x + 2x\cdot x^{-1} = 2x^2+2$.

Add them together:

$$y' = (x^2-3+2x^{-2}) + (2x^2+2) = 3x^2-1+\frac{2}{x^2}$$

**$y' = 3x^2-1+\dfrac{2}{x^2}$.**

**19.** $y = \dfrac{x^3-1}{x^2+1}$

$f=x^3-1$ ($f'=3x^2$), $g=x^2+1$ ($g'=2x$).

$$y' = \frac{3x^2(x^2+1) - (x^3-1)(2x)}{(x^2+1)^2} = \frac{3x^4+3x^2 - (2x^4-2x)}{(x^2+1)^2} = \frac{x^4+3x^2+2x}{(x^2+1)^2}$$

**$y' = \dfrac{x^4+3x^2+2x}{(x^2+1)^2}$.**

**20.** Find the tangent line to $y=(2x-1)(x+3)$ at $x=1$.

First, find the point: $y(1) = (2(1)-1)(1+3) = (1)(4) = 4$. So the point is $(1,4)$.

Next, find the derivative. Let $f=2x-1$ ($f'=2$), $g=x+3$ ($g'=1$).

$$y' = 2(x+3) + (2x-1)(1) = 2x+6+2x-1 = 4x+5$$

Evaluate at $x=1$: $y'(1) = 4(1)+5 = 9$.

Using point-slope form with point $(1,4)$ and slope $9$:

$$y-4 = 9(x-1)$$

$$y = 9x-9+4 = 9x-5$$

**Tangent line: $y=9x-5$.**

---

### 🌍 Applied

**21.** $R(x) = x\cdot(50-0.5x)$

Let $f=x$ ($f'=1$), $g=50-0.5x$ ($g'=-0.5$).

$$R'(x) = 1\cdot(50-0.5x) + x\cdot(-0.5) = 50-0.5x-0.5x = 50-x$$

Evaluate at $x=10$:

$$R'(10) = 50-10 = 40$$

**Answer: $R'(x)=50-x$, and $R'(10)=40$.** At a sales level of $10$ units, selling one more unit adds about $\$40$ to total revenue.

**22.** $\bar{A}(x) = \dfrac{C(x)}{x} = \dfrac{x^2+20x+100}{x}$

This is easier to simplify first by dividing each term by $x$:

$$\bar{A}(x) = x+20+\frac{100}{x} = x+20+100x^{-1}$$

Differentiate:

$$\bar{A}'(x) = 1-100x^{-2} = 1-\frac{100}{x^2}$$

Evaluate at $x=5$:

$$\bar{A}'(5) = 1-\frac{100}{25} = 1-4 = -3$$

**Answer: $\bar{A}'(x) = 1-\dfrac{100}{x^2}$, and $\bar{A}'(5)=-3$.** At $5$ units of production, the average cost per unit is currently decreasing at a rate of $\$3$ per unit as production increases.

**23.** $D(t) = \dfrac{P(t)}{A(t)} = \dfrac{t^2+5t}{t+2}$

$f=t^2+5t$ ($f'=2t+5$), $g=t+2$ ($g'=1$).

$$D'(t) = \frac{(2t+5)(t+2) - (t^2+5t)(1)}{(t+2)^2}$$

Expand $(2t+5)(t+2) = 2t^2+4t+5t+10 = 2t^2+9t+10$.

$$D'(t) = \frac{(2t^2+9t+10) - (t^2+5t)}{(t+2)^2} = \frac{t^2+4t+10}{(t+2)^2}$$

Evaluate at $t=3$:

$$D'(3) = \frac{9+12+10}{(5)^2} = \frac{31}{25}$$

**Answer: $D'(t) = \dfrac{t^2+4t+10}{(t+2)^2}$, and $D'(3) = \dfrac{31}{25}$.** At year $3$, the population density is increasing at a rate of $\dfrac{31}{25}$ (thousand people per square mile, per year).

**24.** $N(x) = (x+10)(50-2x)$

$f=x+10$ ($f'=1$), $g=50-2x$ ($g'=-2$).

$$N'(x) = 1\cdot(50-2x) + (x+10)(-2) = 50-2x-2x-20 = 30-4x$$

Evaluate at $x=5$:

$$N'(5) = 30-20 = 10$$

**Answer: $N'(x)=30-4x$, and $N'(5)=10$.** At $x=5$, the store's revenue is increasing at a rate of $\$10$ for each small increase in $x$.
