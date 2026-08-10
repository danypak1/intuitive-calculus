# Unit 8: The Derivative as a Function — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2$

$$f(x+h) = (x+h)^2 = x^2+2xh+h^2$$

Subtract $f(x)=x^2$: $2xh+h^2$.

Divide by $h$: $2x+h$.

Let $h\to 0$: $2x$.

**$f'(x) = 2x$.**

**2.** $f(x)=3x+7$

$$f(x+h) = 3(x+h)+7 = 3x+3h+7$$

Subtract $f(x)=3x+7$: $3h$.

Divide by $h$: $3$.

Let $h\to 0$: $3$.

**$f'(x) = 3$.** (Makes sense — a straight line has the same slope everywhere.)

**3.** $f(x)=x^2-4x$

$$f(x+h) = (x+h)^2-4(x+h) = x^2+2xh+h^2-4x-4h$$

Subtract $f(x)=x^2-4x$: $2xh+h^2-4h$.

Divide by $h$: $2x+h-4$.

Let $h\to 0$: $2x-4$.

**$f'(x) = 2x-4$.**

**4.** $f(x)=5-2x^2$

$$f(x+h) = 5-2(x+h)^2 = 5-2(x^2+2xh+h^2) = 5-2x^2-4xh-2h^2$$

Subtract $f(x)=5-2x^2$: $-4xh-2h^2$.

Divide by $h$: $-4x-2h$.

Let $h\to 0$: $-4x$.

**$f'(x) = -4x$.**

**5.** $f(x)=x^2+3x-1$

$$f(x+h) = (x+h)^2+3(x+h)-1 = x^2+2xh+h^2+3x+3h-1$$

Subtract $f(x)=x^2+3x-1$: $2xh+h^2+3h$.

Divide by $h$: $2x+h+3$.

Let $h\to 0$: $2x+3$.

**$f'(x) = 2x+3$**, which we can also write as $\dfrac{dy}{dx} = 2x+3$.

**6.** $f(x)=7$

$$f(x+h) = 7$$

Subtract $f(x)=7$: $0$.

Divide by $h$: $0$.

Let $h\to 0$: $0$.

**$f'(x) = 0$ for every $x$.** In plain words: the graph of a constant function is a perfectly flat horizontal line everywhere. Since nothing about the height ever changes as $x$ changes, the slope — the rate of change — is always exactly $0$, at every single point.

---

### 🟡 Standard

**7.** $f(x)=x^2-6x+5$

$$f(x+h) = (x+h)^2-6(x+h)+5 = x^2+2xh+h^2-6x-6h+5$$

Subtract $f(x)=x^2-6x+5$: $2xh+h^2-6h$.

Divide by $h$: $2x+h-6$.

Let $h\to 0$: $2x-6$.

**$f'(x) = 2x-6$.**

$f'(0) = 2(0)-6 = -6$.

$f'(3) = 2(3)-6 = 0$.

$f'(6) = 2(6)-6 = 6$.

**In words:** at $x=0$, the slope is negative ($-6$), meaning the graph is heading downhill there. By $x=3$, the slope has climbed up to exactly $0$ — the graph has flattened out for a moment, which is the bottom of the dip (the minimum point). By $x=6$, the slope is positive ($6$), meaning the graph is now climbing back uphill. So overall: the function decreases, bottoms out at $x=3$, then increases.

**8.** $f(x)=-x^2+8x$

$$f(x+h) = -(x+h)^2+8(x+h) = -(x^2+2xh+h^2)+8x+8h = -x^2-2xh-h^2+8x+8h$$

Subtract $f(x)=-x^2+8x$: $-2xh-h^2+8h$.

Divide by $h$: $-2x-h+8$.

Let $h\to 0$: $-2x+8$.

**$f'(x) = -2x+8$** (or $8-2x$).

Set $f'(x)=0$: $8-2x=0 \Rightarrow x=4$.

**The horizontal tangent occurs at $x=4$.**

**9.** $f(x)=x^3$

$$f(x+h) = (x+h)^3 = x^3+3x^2h+3xh^2+h^3$$

(using the expansion pattern $(a+b)^3 = a^3+3a^2b+3ab^2+b^3$)

Subtract $f(x)=x^3$: $3x^2h+3xh^2+h^3$.

Divide by $h$: $3x^2+3xh+h^2$.

Let $h\to 0$: $3x^2$.

**$f'(x) = 3x^2$.**

**10.** Using $f'(x)=2x$ from Problem 1:

$f'(5) = 2(5) = 10$.

$f'(-3) = 2(-3) = -6$.

The slope of the tangent line at $x=5$ is just $f'(5)$ again.

**$f'(5)=10$, $f'(-3)=-6$, and the tangent slope at $x=5$ is $10$.** No new limit computation needed — that's the whole point of having the general formula.

**11.** $f(x)=2x^2+3x$

$$f(x+h) = 2(x+h)^2+3(x+h) = 2(x^2+2xh+h^2)+3x+3h = 2x^2+4xh+2h^2+3x+3h$$

Subtract $f(x)=2x^2+3x$: $4xh+2h^2+3h$.

Divide by $h$: $4x+2h+3$.

Let $h\to 0$: $4x+3$.

**$f'(x) = 4x+3$.**

Set $f'(x)=7$: $4x+3=7 \Rightarrow 4x=4 \Rightarrow x=1$.

**$f'(x)=7$ at $x=1$.**

**12.** Rises, peak, falls, valley, rises again.

- **While rising** (both the first climb and the final climb): $f'(x) > 0$.
- **While falling** (the middle section): $f'(x) < 0$.
- **At the peak** (where rising switches to falling) and **at the valley** (where falling switches back to rising): $f'(x) = 0$, since the tangent line is momentarily flat at each turning point.

---

### 🔴 Challenge

**13.** $f(x)=\dfrac{1}{x}$

$$\frac{f(x+h)-f(x)}{h} = \frac{\frac{1}{x+h}-\frac{1}{x}}{h}$$

Combine the top over a common denominator $x(x+h)$:

$$\frac{1}{x+h}-\frac{1}{x} = \frac{x-(x+h)}{x(x+h)} = \frac{-h}{x(x+h)}$$

So the whole expression becomes:

$$\frac{-h}{x(x+h)} \cdot \frac{1}{h} = \frac{-1}{x(x+h)}$$

Let $h\to 0$:

$$\frac{-1}{x\cdot x} = -\frac{1}{x^2}$$

**$f'(x) = -\dfrac{1}{x^2}$.**

**14.** $f(x)=\sqrt{x}$

$$\frac{f(x+h)-f(x)}{h} = \frac{\sqrt{x+h}-\sqrt{x}}{h}$$

Multiply top and bottom by the conjugate $\sqrt{x+h}+\sqrt{x}$:

$$\frac{(x+h)-x}{h\big(\sqrt{x+h}+\sqrt{x}\big)} = \frac{h}{h\big(\sqrt{x+h}+\sqrt{x}\big)} = \frac{1}{\sqrt{x+h}+\sqrt{x}}$$

Let $h\to 0$:

$$\frac{1}{\sqrt{x}+\sqrt{x}} = \frac{1}{2\sqrt{x}}$$

**$f'(x) = \dfrac{1}{2\sqrt{x}}$.**

**15.** $f(x) = \begin{cases} x+1, & x<2 \\ x^2, & x\ge 2\end{cases}$

**Check continuity at $x=2$ first:** $f(2) = 2^2 = 4$.

Left-hand limit: $2+1=3$. Right-hand limit: $4$.

Since $3\ne 4$, the two one-sided limits disagree — $f$ is **not continuous** at $x=2$ (it has a jump).

**Answer: since $f$ is not even continuous at $x=2$, it is automatically NOT differentiable there.** By the theorem (differentiable $\Rightarrow$ continuous), a function that fails continuity can never be differentiable at that same point — there's no need to compute any derivative limit at all.

**16.** $f(x) = \begin{cases} 3, & x\le 1 \\ 2x+1, & x>1\end{cases}$

**Check continuity at $x=1$:** $f(1)=3$ (from the first piece, since $x\le1$ includes $1$).

Left-hand limit: $3$. Right-hand limit: $2(1)+1=3$. Both match — **$f$ is continuous at $x=1$.**

Since continuity alone doesn't guarantee differentiability, we must check directly.

**Left-hand difference quotient** (using the constant piece, valid for $h<0$): $f(1+h)=3$, so

$$\frac{f(1+h)-f(1)}{h} = \frac{3-3}{h} = 0$$

As $h\to 0^-$: $0$.

**Right-hand difference quotient** (using $2x+1$, valid for $h>0$): $f(1+h) = 2(1+h)+1 = 3+2h$, so

$$\frac{f(1+h)-f(1)}{h} = \frac{(3+2h)-3}{h} = \frac{2h}{h} = 2$$

As $h\to 0^+$: $2$.

Since $0 \ne 2$, the two sides disagree.

**Answer: $f$ is continuous at $x=1$, but NOT differentiable there** — the two pieces meet at the same height but arrive with different slopes, creating a corner.

**17.** $f(x) = |x|+x^2$, differentiability at $x=0$.

$f(0) = 0+0 = 0$.

$$\frac{f(0+h)-f(0)}{h} = \frac{|h|+h^2-0}{h} = \frac{|h|}{h} + h$$

**As $h\to 0^+$:** $|h|=h$, so $\dfrac{|h|}{h}=1$. The whole expression is $1+h \to 1$.

**As $h\to 0^-$:** $|h|=-h$, so $\dfrac{|h|}{h}=-1$. The whole expression is $-1+h \to -1$.

Since $1 \ne -1$, the two sides disagree.

**Answer: $f$ is NOT differentiable at $x=0$.** Even though we added a perfectly smooth term ($x^2$) on top of $|x|$, the sharp corner from $|x|$ still shows through, since $x^2$ contributes a slope of $0$ at $x=0$ and doesn't smooth out the mismatch coming from the absolute value part.

---

### 🌍 Applied

**18.** $h(t) = -5t^2+20t+2$

$$h(t+k) = -5(t+k)^2+20(t+k)+2 = -5(t^2+2tk+k^2)+20t+20k+2$$

$$= -5t^2-10tk-5k^2+20t+20k+2$$

Subtract $h(t)=-5t^2+20t+2$: $-10tk-5k^2+20k$.

Divide by $k$: $-10t-5k+20$.

Let $k\to 0$: $-10t+20$.

**$v(t) = h'(t) = 20-10t$.**

$v(0) = 20$. $v(1) = 20-10=10$. $v(2) = 20-20=0$.

**In words:** at $t=0$ (the moment of release), the ball is moving upward at $20$ m/s. By $t=1$ second, it has slowed to $10$ m/s (still rising, but decelerating due to gravity). At $t=2$ seconds, the velocity is exactly $0$ — this is the instant the ball reaches its peak height, momentarily pausing before it starts to fall back down.

**19.** $R(x) = 100x-0.5x^2$

$$R(x+k) = 100(x+k)-0.5(x+k)^2 = 100x+100k-0.5(x^2+2xk+k^2)$$

$$= 100x+100k-0.5x^2-xk-0.5k^2$$

Subtract $R(x)=100x-0.5x^2$: $100k-xk-0.5k^2$.

Divide by $k$: $100-x-0.5k$.

Let $k\to 0$: $100-x$.

**$R'(x) = 100-x$.**

$R'(50) = 50$. $R'(100) = 0$. $R'(150) = -50$.

**Trend:** the marginal revenue starts out solidly positive (at $50$ units, each additional sale still adds about $\$50$ to revenue), drops to exactly $0$ at $x=100$ (this is the revenue-maximizing production level — selling one more unit right around here adds essentially nothing more), and turns negative beyond that (past $100$ units, selling additional units actually starts to *decrease* total revenue, likely because prices have to be cut too much to move the extra volume).

**20.** $N(t) = 200t-4t^2$

$$N(t+k) = 200(t+k)-4(t+k)^2 = 200t+200k-4(t^2+2tk+k^2)$$

$$= 200t+200k-4t^2-8tk-4k^2$$

Subtract $N(t)=200t-4t^2$: $200k-8tk-4k^2$.

Divide by $k$: $200-8t-4k$.

Let $k\to 0$: $200-8t$.

**$N'(t) = 200-8t$.**

$N'(10) = 200-80=120$. $N'(25) = 200-200=0$.

**In words:** on day $10$, the rumor is picking up new listeners at a rate of $120$ people per day. By day $25$, that rate has dropped all the way to $0$ — the rumor has reached its peak audience size and, at that exact moment, has stopped gaining any new people at all (it may begin to shrink after this, depending on how the model continues).

**21.** $s(t) = t^3-3t$

$$s(t+k) = (t+k)^3-3(t+k) = t^3+3t^2k+3tk^2+k^3-3t-3k$$

Subtract $s(t)=t^3-3t$: $3t^2k+3tk^2+k^3-3k$.

Divide by $k$: $3t^2+3tk+k^2-3$.

Let $k\to 0$: $3t^2-3$.

**$s'(t) = 3t^2-3$.**

$s'(0) = -3$. $s'(1) = 3-3=0$. $s'(2) = 12-3=9$.

**In words:** at $t=0$, the object has velocity $-3$ m/s, meaning it's moving in the negative direction. At $t=1$ second, the velocity is exactly $0$ — the object has momentarily stopped, likely about to reverse direction. By $t=2$ seconds, the velocity is $+9$ m/s, meaning the object is now moving quickly in the positive direction — so somewhere around $t=1$, the object turned around.
