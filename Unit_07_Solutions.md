# Unit 7: The Derivative at a Point — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2+5x$, find $f'(1)$.

$f(1) = 1+5 = 6$.

$f(1+h) = (1+h)^2+5(1+h) = 1+2h+h^2+5+5h = 6+7h+h^2$.

Subtract $f(1)=6$: $7h+h^2$.

Divide by $h$: $7+h$.

Let $h\to 0$: $7$.

**$f'(1) = 7$.**

**2.** $f(x)=3x^2-2$, find $f'(0)$.

$f(0) = -2$.

$f(0+h) = 3h^2-2$.

Subtract $f(0)=-2$: $3h^2$.

Divide by $h$: $3h$.

Let $h\to 0$: $0$.

**$f'(0) = 0$.**

**3.** $f(x)=-x^2+4x$, find $f'(2)$.

$f(2) = -4+8 = 4$.

$f(2+h) = -(2+h)^2+4(2+h) = -(4+4h+h^2)+8+4h = -4-4h-h^2+8+4h = 4-h^2$.

Subtract $f(2)=4$: $-h^2$.

Divide by $h$: $-h$.

Let $h\to 0$: $0$.

**$f'(2) = 0$.** (This makes sense: $-x^2+4x$ is a downward parabola with its peak exactly at $x=2$, and the tangent line at the very top of a hill is always flat.)

**4.** $f(x)=5x-x^2$, find $f'(-1)$.

$f(-1) = -5-1 = -6$.

$f(-1+h) = 5(-1+h)-(-1+h)^2 = -5+5h-(1-2h+h^2) = -5+5h-1+2h-h^2 = -6+7h-h^2$.

Subtract $f(-1)=-6$: $7h-h^2$.

Divide by $h$: $7-h$.

Let $h\to 0$: $7$.

**$f'(-1) = 7$.**

**5.** $f(x)=2x^2+3$, find $f'(3)$.

$f(3) = 18+3 = 21$.

$f(3+h) = 2(3+h)^2+3 = 2(9+6h+h^2)+3 = 18+12h+2h^2+3 = 21+12h+2h^2$.

Subtract $f(3)=21$: $12h+2h^2$.

Divide by $h$: $12+2h$.

Let $h\to 0$: $12$.

**$f'(3) = 12$.**

**6.** $f(x)=x^2-1$, find $f'(-2)$.

$f(-2) = 4-1 = 3$.

$f(-2+h) = (-2+h)^2-1 = 4-4h+h^2-1 = 3-4h+h^2$.

Subtract $f(-2)=3$: $-4h+h^2$.

Divide by $h$: $-4+h$.

Let $h\to 0$: $-4$.

**$f'(-2) = -4$.**

---

### 🟡 Standard

**7.** $f(x)=-2x^2$, find $f'(1)$ using the $x$-form definition.

$f(1) = -2$.

$$f'(1) = \lim_{x\to 1}\frac{f(x)-f(1)}{x-1} = \lim_{x\to 1}\frac{-2x^2-(-2)}{x-1} = \lim_{x\to 1}\frac{-2x^2+2}{x-1}$$

Factor: $-2x^2+2 = -2(x^2-1) = -2(x-1)(x+1)$.

$$\lim_{x\to 1}\frac{-2(x-1)(x+1)}{x-1} = \lim_{x\to 1}\big[-2(x+1)\big]$$

Plug in $x=1$: $-2(1+1) = -4$.

**$f'(1) = -4$.**

**8.** $f(x)=x^2-4x$, find $f'(3)$ using the $x$-form definition.

$f(3) = 9-12 = -3$.

$$f'(3) = \lim_{x\to 3}\frac{(x^2-4x)-(-3)}{x-3} = \lim_{x\to 3}\frac{x^2-4x+3}{x-3}$$

Factor the top: numbers multiplying to $3$, adding to $-4$: $-1$ and $-3$.

$$x^2-4x+3 = (x-1)(x-3)$$

$$\lim_{x\to 3}\frac{(x-1)(x-3)}{x-3} = \lim_{x\to 3}(x-1)$$

Plug in $x=3$: $3-1=2$.

**$f'(3) = 2$.**

**9.** $f(x)=x^2+1$, find $f'(1)$ using the $x$-form definition, then find the tangent and normal lines at $(1,2)$.

$f(1) = 2$.

$$f'(1) = \lim_{x\to 1}\frac{(x^2+1)-2}{x-1} = \lim_{x\to 1}\frac{x^2-1}{x-1} = \lim_{x\to 1}\frac{(x-1)(x+1)}{x-1} = \lim_{x\to 1}(x+1) = 2$$

**$f'(1) = 2$.**

**Tangent line:** $y-2 = 2(x-1) \Rightarrow y = 2x$.

**Normal line:** slope is $-\dfrac{1}{2}$: $y-2 = -\dfrac{1}{2}(x-1) \Rightarrow y = -\dfrac{1}{2}x+\dfrac{1}{2}+2 = -\dfrac{1}{2}x+\dfrac{5}{2}$.

**Tangent line: $y=2x$. Normal line: $y=-\dfrac{1}{2}x+\dfrac{5}{2}$.**

**10.** $f(x)=3x^2-x$, find $f'(2)$ and the tangent line.

$f(2) = 12-2 = 10$.

$f(2+h) = 3(2+h)^2-(2+h) = 3(4+4h+h^2)-2-h = 12+12h+3h^2-2-h = 10+11h+3h^2$.

Subtract $f(2)=10$: $11h+3h^2$.

Divide by $h$: $11+3h$.

Let $h\to 0$: $11$.

**$f'(2) = 11$.**

**Tangent line:** $y-10 = 11(x-2) \Rightarrow y = 11x-22+10 = 11x-12$.

**11.** $f(x)=-x^2+2x+1$, find $f'(0)$ and the tangent line.

$f(0) = 1$.

$f(0+h) = -h^2+2h+1$.

Subtract $f(0)=1$: $-h^2+2h$.

Divide by $h$: $-h+2$.

Let $h\to 0$: $2$.

**$f'(0) = 2$.**

**Tangent line:** $y-1 = 2(x-0) \Rightarrow y=2x+1$.

**12.** $f(x)=2x^2-5x$, find $f'(1)$ and both the tangent and normal lines.

$f(1) = 2-5 = -3$.

$f(1+h) = 2(1+h)^2-5(1+h) = 2(1+2h+h^2)-5-5h = 2+4h+2h^2-5-5h = -3-h+2h^2$.

Subtract $f(1)=-3$: $-h+2h^2$.

Divide by $h$: $-1+2h$.

Let $h\to 0$: $-1$.

**$f'(1) = -1$.**

**Tangent line:** $y-(-3) = -1(x-1) \Rightarrow y+3 = -x+1 \Rightarrow y = -x-2$.

**Normal line:** slope is $-\dfrac{1}{-1} = 1$: $y+3 = 1(x-1) \Rightarrow y = x-1-3 = x-4$.

**Tangent line: $y=-x-2$. Normal line: $y=x-4$.**

---

### 🔴 Challenge

**13.** $f(x)=\dfrac{1}{x+1}$, find $f'(1)$.

$f(1) = \dfrac{1}{2}$.

$$\frac{f(1+h)-f(1)}{h} = \frac{\frac{1}{2+h}-\frac{1}{2}}{h}$$

Combine the top over a common denominator $2(2+h)$:

$$\frac{1}{2+h}-\frac{1}{2} = \frac{2-(2+h)}{2(2+h)} = \frac{-h}{2(2+h)}$$

So the whole expression is:

$$\frac{-h}{2(2+h)}\cdot\frac{1}{h} = \frac{-1}{2(2+h)}$$

Let $h\to 0$: $\dfrac{-1}{2(2)} = -\dfrac{1}{4}$.

**$f'(1) = -\dfrac{1}{4}$.**

**14.** $f(x)=\sqrt{x+5}$, find $f'(4)$.

$f(4) = \sqrt{9} = 3$.

$$\frac{f(4+h)-f(4)}{h} = \frac{\sqrt{9+h}-3}{h}$$

Multiply top and bottom by the conjugate $\sqrt{9+h}+3$:

$$\frac{(9+h)-9}{h\big(\sqrt{9+h}+3\big)} = \frac{h}{h\big(\sqrt{9+h}+3\big)} = \frac{1}{\sqrt{9+h}+3}$$

Let $h\to 0$: $\dfrac{1}{\sqrt{9}+3} = \dfrac{1}{3+3} = \dfrac{1}{6}$.

**$f'(4) = \dfrac{1}{6}$.**

**15.** $f(x)=x^3-x$, find $f'(-1)$ using the $x$-form definition.

$f(-1) = (-1)^3-(-1) = -1+1 = 0$.

$$f'(-1) = \lim_{x\to -1}\frac{(x^3-x)-0}{x-(-1)} = \lim_{x\to -1}\frac{x^3-x}{x+1}$$

Factor the top: $x^3-x = x(x^2-1) = x(x-1)(x+1)$.

$$\lim_{x\to -1}\frac{x(x-1)(x+1)}{x+1} = \lim_{x\to -1}\big[x(x-1)\big]$$

Plug in $x=-1$: $(-1)(-1-1) = (-1)(-2) = 2$.

**$f'(-1) = 2$.**

**16.** Show $f(x)=|x-2|$ is not differentiable at $x=2$.

We compute the difference quotient at $a=2$: since $f(2)=|2-2|=0$,

$$\frac{f(2+h)-f(2)}{h} = \frac{|h|-0}{h} = \frac{|h|}{h}$$

**As $h\to 0^+$** (small positive $h$): $|h|=h$, so $\dfrac{|h|}{h} = \dfrac{h}{h}=1$.

**As $h\to 0^-$** (small negative $h$): $|h|=-h$, so $\dfrac{|h|}{h} = \dfrac{-h}{h}=-1$.

Since $1 \ne -1$, the left-hand and right-hand versions of the limit disagree.

**Answer: $f'(2)$ does not exist — $f(x)=|x-2|$ is not differentiable at $x=2$.** This matches the picture: the graph of $|x-2|$ has a sharp corner (a "V" shape) at $x=2$, and a sharp corner never has one single well-defined tangent slope.

**17.** $f(x) = \begin{cases} x^2, & x<1 \\ 2x-1, & x\ge 1\end{cases}$, is this differentiable at $x=1$?

First, note $f(1) = 2(1)-1 = 1$ (from the second piece).

**Left-hand difference quotient** (using the piece valid for $x<1$, so $h<0$ meaning $1+h<1$): with $f(1+h) = (1+h)^2 = 1+2h+h^2$,

$$\frac{f(1+h)-f(1)}{h} = \frac{(1+2h+h^2)-1}{h} = \frac{2h+h^2}{h} = 2+h$$

As $h\to 0^-$: $2$.

**Right-hand difference quotient** (using the piece valid for $x\ge 1$, so $h>0$): with $f(1+h) = 2(1+h)-1 = 1+2h$,

$$\frac{f(1+h)-f(1)}{h} = \frac{(1+2h)-1}{h} = \frac{2h}{h} = 2$$

As $h\to 0^+$: $2$.

Both sides give $2$.

**Answer: $f'(1) = 2$ — $f$ IS differentiable at $x=1$.** The two pieces don't just meet at the same height (which made it continuous, as you found in an earlier unit) — they also arrive with the exact same slope, so they blend together smoothly with no corner at all.

---

### 🌍 Applied

**18.** $h(t)=-5t^2+30t$, find $h'(1)$.

$h(1) = -5+30 = 25$.

$h(1+k) = -5(1+k)^2+30(1+k) = -5(1+2k+k^2)+30+30k = -5-10k-5k^2+30+30k = 25+20k-5k^2$.

Subtract $h(1)=25$: $20k-5k^2$.

Divide by $k$: $20-5k$.

Let $k\to 0$: $20$.

**$h'(1) = 20$.** This means at exactly $t=1$ second, the ball is rising at an instantaneous speed of $20$ meters per second.

**19.** $C(x)=0.5x^2+10x$, find $C'(4)$.

$C(4) = 0.5(16)+40 = 8+40 = 48$.

$C(4+k) = 0.5(4+k)^2+10(4+k) = 0.5(16+8k+k^2)+40+10k = 8+4k+0.5k^2+40+10k = 48+14k+0.5k^2$.

Subtract $C(4)=48$: $14k+0.5k^2$.

Divide by $k$: $14+0.5k$.

Let $k\to 0$: $14$.

**$C'(4) = 14$.** This means when the company is producing around $4$ units, each additional unit costs about $\$14$ more to produce — this is called the **marginal cost** at that production level.

**20.** $P(t)=t^2+50t$, find $P'(3)$.

$P(3) = 9+150 = 159$.

$P(3+k) = (3+k)^2+50(3+k) = 9+6k+k^2+150+50k = 159+56k+k^2$.

Subtract $P(3)=159$: $56k+k^2$.

Divide by $k$: $56+k$.

Let $k\to 0$: $56$.

**$P'(3) = 56$.** This means at year $3$, the population is growing at an instantaneous rate of $56$ people per year.

**21.** $s(t)=4t^2-2t$, find $s'(2)$.

$s(2) = 16-4 = 12$.

$s(2+k) = 4(2+k)^2-2(2+k) = 4(4+4k+k^2)-4-2k = 16+16k+4k^2-4-2k = 12+14k+4k^2$.

Subtract $s(2)=12$: $14k+4k^2$.

Divide by $k$: $14+4k$.

Let $k\to 0$: $14$.

**$s'(2) = 14$.** This means at exactly $t=2$ seconds, the object's instantaneous speed is $14$ meters per second.
