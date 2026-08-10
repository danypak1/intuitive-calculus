# Unit 1: Rates of Change and Tangent Lines — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2$, from $x=1$ to $x=4$.

Compute the two values: $f(4) = 16$ and $f(1) = 1$.

$$\frac{f(4)-f(1)}{4-1} = \frac{16-1}{3} = \frac{15}{3} = 5$$

**Average rate of change $= 5$.**

**2.** $f(x)=3x+2$, from $x=-2$ to $x=5$.

$f(5) = 3(5)+2 = 17$. $f(-2) = 3(-2)+2 = -4$.

$$\frac{17-(-4)}{5-(-2)} = \frac{21}{7} = 3$$

**Average rate of change $= 3$.** Notice this is exactly the slope $3$ from $f(x)=3x+2$ — for a straight line, the average rate of change between *any* two points is always the same, and it's just the line's slope.

**3.** $f(x)=x^2-2x$ on $[0,3]$.

$f(3) = 9 - 6 = 3$. $f(0) = 0 - 0 = 0$.

$$\frac{3-0}{3-0} = 1$$

**Average rate of change $= 1$.**

**4.** $f(x)=\sqrt{x}$, from $x=1$ to $x=9$.

$f(9) = 3$. $f(1) = 1$.

$$\frac{3-1}{9-1} = \frac{2}{8} = \frac{1}{4}$$

**Average rate of change $= \frac{1}{4}$.**

**5.** Points $(2,5)$ and $(6,13)$.

Slope $= \dfrac{\text{change in }y}{\text{change in }x} = \dfrac{13-5}{6-2} = \dfrac{8}{4} = 2$.

**Slope of secant line $= 2$.**

**6.** $f(x)=x^3$, from $x=1$ to $x=2$.

$f(2) = 8$. $f(1) = 1$.

$$\frac{8-1}{2-1} = 7$$

**Slope of secant line $= 7$.**

**7.** $f(x)=\dfrac{1}{x}$ on $[1,2]$.

$f(2) = \dfrac{1}{2}$. $f(1) = 1$.

$$\frac{\frac{1}{2}-1}{2-1} = \frac{-\frac{1}{2}}{1} = -\frac{1}{2}$$

**Average rate of change $= -\dfrac{1}{2}$.**

---

### 🟡 Standard

**8.** $f(x)=x^2$, tangent slope at $x=3$.

Step 1 — write $f(3+h)$: $(3+h)^2 = 9 + 6h + h^2$.

Step 2 — subtract $f(3) = 9$: $9+6h+h^2 - 9 = 6h + h^2$.

Step 3 — divide by $h$: $\dfrac{6h+h^2}{h} = 6+h$ (we can cancel one $h$ from every term, since $h \ne 0$ while we're doing this step).

Step 4 — let $h \to 0$: $6 + 0 = 6$.

**Tangent slope at $x=3$ is $6$.**

**9.** $f(x)=x^2+1$, tangent slope at $(1,2)$.

$f(1+h) = (1+h)^2 + 1 = 1 + 2h + h^2 + 1 = 2 + 2h + h^2$.

Subtract $f(1)=2$: $2+2h+h^2 - 2 = 2h+h^2$.

Divide by $h$: $2+h$.

Let $h\to 0$: $2$.

**Tangent slope at $(1,2)$ is $2$.**

**10.** $f(x)=2x^2-3x$, tangent slope at $x=2$.

$f(2+h) = 2(2+h)^2 - 3(2+h)$.

Expand $(2+h)^2 = 4+4h+h^2$, so $2(2+h)^2 = 8+8h+2h^2$.

Expand $-3(2+h) = -6-3h$.

Add them: $8+8h+2h^2-6-3h = 2+5h+2h^2$.

$f(2) = 2(4)-3(2) = 8-6=2$.

Subtract: $2+5h+2h^2 - 2 = 5h+2h^2$.

Divide by $h$: $5+2h$.

Let $h\to 0$: $5$.

**Tangent slope at $x=2$ is $5$.**

**11.** $f(x)=x^2$, tangent line at $x=-1$.

First find the slope: $f(-1) = 1$.

$f(-1+h) = (-1+h)^2 = 1 - 2h + h^2$.

Subtract $f(-1)=1$: $1-2h+h^2-1 = -2h+h^2$.

Divide by $h$: $-2+h$.

Let $h\to 0$: $-2$. So the slope is $-2$.

Now use the point-slope formula with point $(-1, 1)$ and slope $-2$:

$$y - 1 = -2(x-(-1)) = -2(x+1)$$

$$y - 1 = -2x - 2$$

$$y = -2x - 1$$

**Tangent line: $y = -2x - 1$.**

**12.** $f(x)=-2x^2$, tangent slope and tangent line at $x=1$.

$f(1) = -2(1)^2 = -2$.

$f(1+h) = -2(1+h)^2 = -2(1+2h+h^2) = -2-4h-2h^2$.

Subtract $f(1)=-2$: $-2-4h-2h^2 - (-2) = -4h-2h^2$.

Divide by $h$: $-4-2h$.

Let $h\to 0$: $-4$. So the slope is $-4$.

Tangent line through $(1,-2)$ with slope $-4$:

$$y-(-2) = -4(x-1)$$

$$y+2 = -4x+4$$

$$y = -4x+2$$

**Tangent slope $=-4$; tangent line: $y=-4x+2$.**

**13.** $f(x)=x^3$, tangent slope at $x=1$.

$f(1) = 1$.

$f(1+h) = (1+h)^3 = 1+3h+3h^2+h^3$ (this comes from the pattern $(a+b)^3 = a^3+3a^2b+3ab^2+b^3$).

Subtract $f(1)=1$: $1+3h+3h^2+h^3-1 = 3h+3h^2+h^3$.

Divide by $h$: $3+3h+h^2$.

Let $h\to 0$: $3$.

**Tangent slope at $x=1$ is $3$.**

---

### 🔴 Challenge

**14.** $f(x)=x^2+1$, tangent and normal line at $(1,2)$.

From Problem 9, we already know the tangent slope at this point is $2$.

**Tangent line:** $y-2 = 2(x-1) \Rightarrow y = 2x$.

**Normal line:** the normal slope is the *negative reciprocal* of $2$, which is $-\dfrac{1}{2}$.

$$y - 2 = -\frac{1}{2}(x-1)$$

$$y = -\frac{1}{2}x + \frac{1}{2} + 2 = -\frac{1}{2}x + \frac{5}{2}$$

**Tangent line: $y=2x$. Normal line: $y = -\dfrac{1}{2}x + \dfrac{5}{2}$.**

**15.** $f(x)=x^2-4x+3$, find where the tangent is horizontal.

A horizontal line has slope $0$, so we need to find where the tangent slope equals $0$. Let's find a *general* formula for the slope at any point $x=a$, then set it to $0$.

$f(a) = a^2-4a+3$.

$f(a+h) = (a+h)^2 - 4(a+h) + 3 = a^2+2ah+h^2 - 4a-4h+3$.

Subtract $f(a)$: $(a^2+2ah+h^2-4a-4h+3) - (a^2-4a+3) = 2ah+h^2-4h$.

Divide by $h$: $2a+h-4$.

Let $h\to 0$: slope $= 2a-4$.

Set the slope to $0$: $2a-4=0 \Rightarrow a=2$.

Find the $y$-value there: $f(2) = 4-8+3 = -1$.

**The tangent line is horizontal at the point $(2,-1)$.**

**16.** $f(x)=x^2$, find where the tangent slope is $6$.

Using the same style as Problems 8 and 11, the general slope formula for $f(x)=x^2$ at any point $x=a$ works out to $2a$ (you can check: at $a=3$ we got slope $6$ matching $2(3)=6$ from Problem 8, and at $a=-1$ we got slope $-2$ matching $2(-1)=-2$ from Problem 11).

Set $2a = 6 \Rightarrow a=3$.

Find $y$: $f(3) = 9$.

**The tangent slope equals $6$ at the point $(3,9)$.**

**17.** $f(x)=\dfrac{1}{x}$, tangent slope at $x=2$.

$$\frac{f(2+h)-f(2)}{h} = \frac{\frac{1}{2+h} - \frac{1}{2}}{h}$$

To subtract the two fractions in the numerator, put them over a common denominator $2(2+h)$:

$$\frac{1}{2+h} - \frac{1}{2} = \frac{2 - (2+h)}{2(2+h)} = \frac{-h}{2(2+h)}$$

Now divide this whole thing by $h$ (which means multiplying by $\dfrac{1}{h}$):

$$\frac{-h}{2(2+h)} \cdot \frac{1}{h} = \frac{-1}{2(2+h)}$$

Now let $h\to 0$:

$$\frac{-1}{2(2+0)} = \frac{-1}{4}$$

**Tangent slope at $x=2$ is $-\dfrac{1}{4}$.**

**18.** $f(x)=\sqrt{x}$, tangent slope at $x=4$.

$$\frac{f(4+h)-f(4)}{h} = \frac{\sqrt{4+h}-\sqrt{4}}{h} = \frac{\sqrt{4+h}-2}{h}$$

Here, plugging in $h=0$ directly gives $\frac{0}{0}$, and there's no obvious factor of $h$ to cancel — so we use a special trick: multiply top and bottom by the **conjugate** $\sqrt{4+h}+2$. This works because $(\sqrt{4+h}-2)(\sqrt{4+h}+2) = (4+h) - 4 = h$, which clears out the square root.

$$\frac{\sqrt{4+h}-2}{h} \cdot \frac{\sqrt{4+h}+2}{\sqrt{4+h}+2} = \frac{(4+h)-4}{h(\sqrt{4+h}+2)} = \frac{h}{h(\sqrt{4+h}+2)}$$

Cancel the $h$:

$$\frac{1}{\sqrt{4+h}+2}$$

Now let $h\to 0$:

$$\frac{1}{\sqrt{4}+2} = \frac{1}{2+2} = \frac{1}{4}$$

**Tangent slope at $x=4$ is $\dfrac{1}{4}$.**

---

### 🌍 Applied

**19.** $h(t) = 20t-5t^2$, average velocity from $t=1$ to $t=3$.

$h(3) = 20(3)-5(9) = 60-45 = 15$.

$h(1) = 20(1)-5(1) = 20-5=15$.

$$\frac{h(3)-h(1)}{3-1} = \frac{15-15}{2} = 0$$

**Average velocity $= 0$ m/s.** This makes sense: the ball is at the same height ($15$ m) at both times — it went up and came back down to that same height, so its *net* change in position over that interval is zero, even though it was clearly moving the whole time.

**20.** Instantaneous velocity at $t=1$ for $h(t)=20t-5t^2$.

We'll use $k$ as our tiny step (to avoid confusing it with the function's name $h$).

$h(1) = 15$ (from Problem 19).

$$h(1+k) = 20(1+k) - 5(1+k)^2 = 20+20k - 5(1+2k+k^2) = 20+20k-5-10k-5k^2$$

$$= 15+10k-5k^2$$

Subtract $h(1)=15$: $10k-5k^2$.

Divide by $k$: $10-5k$.

Let $k \to 0$: $10$.

**Instantaneous velocity at $t=1$ is $10$ m/s.**

**21.** $s(t)=t^2+2t$, average speed on $[0,2]$ and instantaneous speed at $t=2$.

**Average speed:** $s(2) = 4+4=8$. $s(0)=0$.

$$\frac{8-0}{2-0}=4$$

**Average speed $=4$ mph.**

**Instantaneous speed at $t=2$:**

$$s(2+k) = (2+k)^2+2(2+k) = 4+4k+k^2+4+2k = 8+6k+k^2$$

Subtract $s(2)=8$: $6k+k^2$.

Divide by $k$: $6+k$.

Let $k\to 0$: $6$.

**Instantaneous speed at $t=2$ is $6$ mph.**

**22.** $T(x) = -0.1x^2+2x+50$. Average rate of change from $x=2$ to $x=8$, and instantaneous rate at $x=5$.

**Average rate of change:**

$T(8) = -0.1(64)+2(8)+50 = -6.4+16+50 = 59.6$.

$T(2) = -0.1(4)+2(2)+50 = -0.4+4+50=53.6$.

$$\frac{59.6-53.6}{8-2} = \frac{6}{6} = 1$$

**Average rate of change $= 1\text{°F per hour}$.**

**Instantaneous rate at $x=5$:**

$$T(5+k) = -0.1(5+k)^2 + 2(5+k) + 50$$

Expand $(5+k)^2 = 25+10k+k^2$, so $-0.1(5+k)^2 = -2.5-k-0.1k^2$.

Expand $2(5+k) = 10+2k$.

Add everything: $-2.5-k-0.1k^2+10+2k+50 = 57.5+k-0.1k^2$.

$T(5) = -0.1(25)+10+50 = -2.5+10+50 = 57.5$.

Subtract: $k-0.1k^2$.

Divide by $k$: $1-0.1k$.

Let $k\to 0$: $1$.

**Instantaneous rate of change at hour 5 is $1\text{°F per hour}$.**
