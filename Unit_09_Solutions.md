# Unit 9: Power Rule & Basic Rules — Full Solutions

### 🟢 Warm-up

**1.** $y=x^5$

Bring the exponent $5$ down front as a multiplier, then subtract $1$ from the exponent:

$$y' = 5x^{5-1} = 5x^4$$

**2.** $y=x^{10}$

$$y' = 10x^{10-1} = 10x^9$$

**3.** $y=7x^3$

The $7$ just tags along; apply the power rule to $x^3$:

$$y' = 7\cdot 3x^{2} = 21x^2$$

**4.** $y=4x^2-3x+5$

Differentiate term by term. $4x^2 \to 8x$. $-3x \to -3$ (since $x=x^1$, and $1\cdot x^0=1$). $5 \to 0$ (constant).

$$y' = 8x - 3$$

**5.** $y=x^3-2x^2+x-9$

$x^3 \to 3x^2$. $-2x^2 \to -4x$. $x \to 1$. $-9 \to 0$.

$$y' = 3x^2-4x+1$$

**6.** $y=-3x^4+2x^2$

$-3x^4 \to -12x^3$. $2x^2 \to 4x$.

$$y' = -12x^3+4x$$

**7.** $y=10$

A plain constant, no $x$ attached — its derivative is $0$.

$$y' = 0$$

**8.** $y=6x$

Think of this as $6x^1$: bring down the $1$, then the exponent becomes $0$, and $x^0=1$.

$$y' = 6\cdot 1 \cdot x^0 = 6$$

---

### 🟡 Standard

**9.** $y=\sqrt{x}$

Rewrite as a power first: $y = x^{1/2}$.

$$y' = \frac{1}{2}x^{\frac12-1} = \frac{1}{2}x^{-1/2} = \frac{1}{2\sqrt{x}}$$

**10.** $y=\dfrac{1}{x^2}$

Rewrite: $y=x^{-2}$.

$$y' = -2x^{-2-1} = -2x^{-3} = -\frac{2}{x^3}$$

**11.** $y=\dfrac{1}{x^3}$

Rewrite: $y=x^{-3}$.

$$y' = -3x^{-3-1} = -3x^{-4} = -\frac{3}{x^4}$$

**12.** $y=3\sqrt{x}-\dfrac{2}{x}$

Rewrite: $y = 3x^{1/2} - 2x^{-1}$.

Differentiate each term: $3x^{1/2} \to 3\cdot\frac12 x^{-1/2} = \frac32 x^{-1/2}$. $-2x^{-1} \to -2\cdot(-1)x^{-2} = 2x^{-2}$.

$$y' = \frac{3}{2}x^{-1/2} + 2x^{-2} = \frac{3}{2\sqrt{x}} + \frac{2}{x^2}$$

**13.** $y=x^{3/2}$

$$y' = \frac{3}{2}x^{\frac32-1} = \frac{3}{2}x^{1/2} = \frac{3}{2}\sqrt{x}$$

**14.** $y=\dfrac{4}{\sqrt{x}}$

Rewrite: $y=4x^{-1/2}$.

$$y' = 4\cdot\left(-\frac12\right)x^{-1/2-1} = -2x^{-3/2} = -\frac{2}{x\sqrt{x}}$$

**15.** $y=2x^3-5\sqrt{x}+\dfrac{1}{x}$

Rewrite: $y=2x^3-5x^{1/2}+x^{-1}$.

Differentiate each term: $2x^3 \to 6x^2$. $-5x^{1/2} \to -5\cdot\frac12x^{-1/2}=-\frac52x^{-1/2}$. $x^{-1} \to -1\cdot x^{-2} = -x^{-2}$.

$$y' = 6x^2 - \frac{5}{2}x^{-1/2} - x^{-2} = 6x^2 - \frac{5}{2\sqrt{x}} - \frac{1}{x^2}$$

---

### 🔴 Challenge

**16.** $y=(x^2+1)^2$

Expand first: $(x^2+1)^2 = (x^2+1)(x^2+1) = x^4+2x^2+1$.

Now differentiate term by term: $x^4 \to 4x^3$. $2x^2 \to 4x$. $1 \to 0$.

$$y' = 4x^3+4x$$

**17.** $y=x(x^2-3)$

Expand first: $x(x^2-3) = x^3-3x$.

$$y' = 3x^2-3$$

**18.** $y=\dfrac{x^3+2x^2-5x}{x}$

Divide every term in the top by $x$ first (valid wherever $x\ne 0$):

$$\frac{x^3}{x}+\frac{2x^2}{x}-\frac{5x}{x} = x^2+2x-5$$

Now differentiate:

$$y' = 2x+2$$

**19.** $y=\dfrac{2x^4-3x^2+x}{x^2}$

Divide every term in the top by $x^2$ first:

$$\frac{2x^4}{x^2}-\frac{3x^2}{x^2}+\frac{x}{x^2} = 2x^2-3+x^{-1}$$

Now differentiate: $2x^2 \to 4x$. $-3 \to 0$. $x^{-1} \to -x^{-2}$.

$$y' = 4x - x^{-2} = 4x - \frac{1}{x^2}$$

**20.** $y=(2x-1)^2$

Expand first: $(2x-1)^2 = (2x-1)(2x-1) = 4x^2-4x+1$.

$$y' = 8x-4$$

**21.** Find all $x$ where the tangent to $y=x^3-3x$ is horizontal.

First find the derivative:

$$y' = 3x^2-3$$

A horizontal tangent happens where the slope is $0$:

$$3x^2-3 = 0$$

$$3x^2 = 3$$

$$x^2 = 1$$

$$x = \pm 1$$

**Answer: the tangent line is horizontal at $x=1$ and at $x=-1$.**

---

### 🌍 Applied

**22.** $s(t)=t^3-6t^2+9t$

Differentiate to get the velocity function:

$$v(t) = s'(t) = 3t^2-12t+9$$

Evaluate at $t=1$:

$$v(1) = 3(1)-12(1)+9 = 3-12+9 = 0$$

**Answer: $v(t)=3t^2-12t+9$, and $v(1)=0$.** At exactly $t=1$ second, the object has momentarily stopped moving — likely turning around at that instant.

**23.** $C(x)=0.01x^3-0.6x^2+13x+100$

Differentiate to get the marginal cost function:

$$C'(x) = 0.03x^2-1.2x+13$$

Evaluate at $x=10$:

$$C'(10) = 0.03(100)-1.2(10)+13 = 3-12+13 = 4$$

**Answer: $C'(x) = 0.03x^2-1.2x+13$, and $C'(10)=4$.** At a production level of $10$ units, each additional unit costs about $\$4$ more to make.

**24.** $A(x)=x(20-x)$

First expand: $A(x) = 20x-x^2$.

Differentiate:

$$\frac{dA}{dx} = 20-2x$$

Set it equal to $0$:

$$20-2x = 0$$

$$x = 10$$

**Answer: $\dfrac{dA}{dx}=20-2x$, and the area's rate of change is $0$ at $x=10$.** This is the value of $x$ that makes the flat tangent line occur on the area graph — meaning it's a candidate for the largest possible garden area (we'll build the full tools to confirm this is a true maximum in a later unit).

**25.** $R(x)=50x-0.02x^2$

Differentiate:

$$R'(x) = 50-0.04x$$

Evaluate at $x=100$:

$$R'(100) = 50-0.04(100) = 50-4 = 46$$

**Answer: $R'(x)=50-0.04x$, and $R'(100)=46$.** At a production level of $100$ units, selling one more unit adds about $\$46$ to total revenue.
