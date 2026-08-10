# Unit 30: Inverse Functions and Their Derivatives — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=2x+3$

$y=2x+3$. Swap: $x=2y+3$. Solve: $2y=x-3 \Rightarrow y=\dfrac{x-3}{2}$.

**$f^{-1}(x)=\dfrac{x-3}{2}$.**

**2.** $f(x)=5x-2$

$y=5x-2$. Swap: $x=5y-2$. Solve: $5y=x+2 \Rightarrow y=\dfrac{x+2}{5}$.

**$f^{-1}(x)=\dfrac{x+2}{5}$.**

**3.** $f(x)=4x$

$y=4x$. Swap: $x=4y$. Solve: $y=\dfrac{x}{4}$.

**$f^{-1}(x)=\dfrac{x}{4}$.**

**4.** $f(x)=\dfrac{x}{2}+1$

$y=\dfrac{x}{2}+1$. Swap: $x=\dfrac{y}{2}+1$. Solve: $x-1=\dfrac{y}{2} \Rightarrow y=2(x-1)=2x-2$.

**$f^{-1}(x)=2x-2$.**

**5.** Verify $f(x)=3x-6$ and $g(x)=\dfrac{x+6}{3}$ are inverses.

$$f(g(x)) = 3\left(\frac{x+6}{3}\right)-6 = (x+6)-6 = x$$

**Confirmed: $g(x)=f^{-1}(x)$.**

**6.** $f(x)=-2x+7$

$y=-2x+7$. Swap: $x=-2y+7$. Solve: $2y=7-x \Rightarrow y=\dfrac{7-x}{2}$.

**$f^{-1}(x)=\dfrac{7-x}{2}$.**

---

### 🟡 Standard

**7.** $f(x)=x^3$

$y=x^3$. Swap: $x=y^3$. Solve: $y=\sqrt[3]{x}$.

**$f^{-1}(x)=\sqrt[3]{x}$.**

**8.** $f(x)=\sqrt{x-2}$, $x\ge2$

$y=\sqrt{x-2}$. Swap: $x=\sqrt{y-2}$. Solve: $x^2=y-2 \Rightarrow y=x^2+2$.

**$f^{-1}(x)=x^2+2$, with domain $x\ge0$** (matching the range of the original function, since $\sqrt{x-2}\ge0$ always).

**9.** $f(x)=x^2+3$, $x\ge0$

$y=x^2+3$. Swap: $x=y^2+3$. Solve: $y^2=x-3 \Rightarrow y=\sqrt{x-3}$ (taking the positive root, since the original domain restricts to $x\ge0$).

**$f^{-1}(x)=\sqrt{x-3}$, with domain $x\ge3$.**

**10.** $f(x)=2x+1$

**(a)** $y=2x+1$. Swap: $x=2y+1$. Solve: $y=\dfrac{x-1}{2}$. So $f^{-1}(x)=\dfrac{x-1}{2}$, and

$$(f^{-1})'(x) = \frac12$$

**(b)** $f'(x)=2$. Using the formula:

$$(f^{-1})'(a) = \frac{1}{f'(f^{-1}(a))} = \frac{1}{2}$$

(since $f'(x)=2$ regardless of the input). **Both methods agree: $(f^{-1})'(x)=\dfrac12$.**

**11.** $f(x)=x^3$, find $(f^{-1})'(8)$.

First find $f^{-1}(8)$: we need $x$ such that $x^3=8$, so $x=2$.

$f'(x)=3x^2$, so $f'(2)=3(4)=12$.

$$(f^{-1})'(8) = \frac{1}{f'(2)} = \frac{1}{12}$$

**Answer: $\dfrac{1}{12}$.**

**12.** $f(x)=x^2+1$, $x\ge0$, $f(2)=5$.

Since $f(2)=5$, we know $f^{-1}(5)=2$.

$f'(x)=2x$, so $f'(2)=4$.

$$(f^{-1})'(5) = \frac{1}{f'(2)} = \frac14$$

**Answer: $\dfrac14$.**

---

### 🔴 Challenge

**13.** $f(x)=6x-1$

$y=6x-1$. Swap: $x=6y-1$. Solve: $6y=x+1 \Rightarrow y=\dfrac{x+1}{6}$.

**$f^{-1}(x)=\dfrac{x+1}{6}$.**

**14.** $f(x)=x^3+x^2+6x+1$, $x\ge0$, find $(f^{-1})'(1)$ where $a=1=f(0)$.

Since $f(0)=0+0+0+1=1$, we know $f^{-1}(1)=0$.

$f'(x)=3x^2+2x+6$, so $f'(0)=0+0+6=6$.

$$(f^{-1})'(1) = \frac{1}{f'(0)} = \frac16$$

**Answer: $\dfrac16$.**

**15.** $f(x)=x^5+2x+1$

**Why explicit inversion is hard:** this is a degree-5 (quintic) polynomial. Unlike quadratics, cubics, or quartics, there is no general algebraic formula (using only basic operations and roots) for solving a general fifth-degree equation for $x$ in terms of $y$ — this is a famous result in algebra. So writing down $f^{-1}(x)$ explicitly isn't practical here, which is exactly why the derivative formula (which sidesteps needing the explicit inverse) is so valuable.

Since $f(1)=1+2+1=4$, we know $f^{-1}(4)=1$.

$f'(x)=5x^4+2$, so $f'(1)=5+2=7$.

$$(f^{-1})'(4) = \frac{1}{f'(1)} = \frac17$$

**Answer: $\dfrac17$.**

**16.** $f(x)=x^3+x$

**Checking one-to-one:** $f'(x)=3x^2+1$. Since $3x^2\ge0$ always, $f'(x)\ge1>0$ for every $x$ — meaning $f$ is strictly increasing everywhere, so it's one-to-one and has a valid inverse.

Since $f(1)=1+1=2$, we know $f^{-1}(2)=1$.

$f'(1)=3(1)+1=4$.

$$(f^{-1})'(2) = \frac{1}{f'(1)} = \frac14$$

**Answer: $\dfrac14$.**

**17.** $f(x)=2x^5+x^3+1$, $f(1)=4$.

Since $f(1)=2+1+1=4$, we know $f^{-1}(4)=1$.

$f'(x)=10x^4+3x^2$, so $f'(1)=10+3=13$.

$$(f^{-1})'(4) = \frac{1}{f'(1)} = \frac{1}{13}$$

**Answer: $\dfrac{1}{13}$.**

---

### 🌍 Applied

**18.** $f(C)=1.8C+32$

$F=1.8C+32$. Solve for $C$: $F-32=1.8C \Rightarrow C=\dfrac{F-32}{1.8}$.

**$f^{-1}(F)=\dfrac{F-32}{1.8}$.**

Convert $98.6°F$:

$$C = \frac{98.6-32}{1.8} = \frac{66.6}{1.8} = 37°C$$

**Answer: $98.6°F = 37°C$.**

**19.** $C(x)=50x+200$

Solve for $x$: $\text{cost}-200=50x \Rightarrow x = \dfrac{\text{cost}-200}{50}$.

**Inverse function: $x=\dfrac{\text{cost}-200}{50}$.**

For a budget of $\$1200$:

$$x = \frac{1200-200}{50} = \frac{1000}{50} = 20$$

**Answer: $20$ units can be produced with a $\$1200$ budget.**

**20.** $p(q)=100-2q$

Solve for $q$: $p=100-2q \Rightarrow 2q=100-p \Rightarrow q=\dfrac{100-p}{2} = 50-\dfrac{p}{2}$.

**$q(p)=50-\dfrac{p}{2}$.** This inverse function tells you the quantity consumers will demand at a given price $p$ — it's the same relationship as the original demand function, just viewed with price as the input and quantity as the output instead of the other way around.

**21.** $h(x)=x^3+2x$, $x\ge0$, $h(2)=12$.

Since $h(2)=8+4=12$, we know $h^{-1}(12)=2$.

$h'(x)=3x^2+2$, so $h'(2)=12+2=14$.

$$(h^{-1})'(12) = \frac{1}{h'(2)} = \frac{1}{14}$$

**Answer: $(h^{-1})'(12)=\dfrac{1}{14}$.** This means that at the point where the rocket has burned $2$ tons of fuel and reached $12$ meters, roughly $\dfrac{1}{14}$ of a ton of additional fuel is needed to climb one more meter at that instant — the local "fuel cost per meter of altitude" at that specific point in the flight.
