# Unit 36: Using Basic Integration Formulas — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int \frac{dx}{\sqrt{1-x^2}} = \arcsin x + C$

**2.** $\displaystyle\int \frac{dx}{1+x^2} = \arctan x + C$

**3.** $\displaystyle\int x^4\,dx = \frac{x^5}{5}+C$

**4.** $\displaystyle\int e^{5x}\,dx = \frac15e^{5x}+C$

**5.** $\displaystyle\int \cos(4x)\,dx = \frac14\sin(4x)+C$

**6.** $\displaystyle\int \frac{dx}{\sqrt{4-x^2}}$

Using $\displaystyle\int\frac{dx}{\sqrt{a^2-x^2}}=\arcsin\left(\frac xa\right)+C$ with $a=2$:

$$= \arcsin\left(\frac{x}{2}\right)+C$$

---

### 🟡 Standard

**7.** $\displaystyle\int \frac{dx}{9+x^2}$

Using $\displaystyle\int\frac{dx}{a^2+x^2}=\frac1a\arctan\left(\frac xa\right)+C$ with $a=3$:

$$= \frac13\arctan\left(\frac{x}{3}\right)+C$$

**8.** $\displaystyle\int \frac{dx}{\sqrt{16-x^2}}$

With $a=4$:

$$= \arcsin\left(\frac{x}{4}\right)+C$$

**9.** $\displaystyle\int \frac{3\,dx}{x^2+4}$

With $a=2$:

$$= 3\cdot\frac12\arctan\left(\frac{x}{2}\right)+C = \frac32\arctan\left(\frac{x}{2}\right)+C$$

**10.** $\displaystyle\int \frac{dx}{\sqrt{9-4x^2}}$

Let $u=2x$, $du=2\,dx \Rightarrow dx=\dfrac{du}{2}$. Rewrite $9-4x^2 = 9-u^2$.

$$\int \frac{1}{\sqrt{9-u^2}}\cdot\frac{du}{2} = \frac12\arcsin\left(\frac u3\right)+C = \frac12\arcsin\left(\frac{2x}{3}\right)+C$$

**11.** Complete the square: $x^2-6x+13$.

Take half of $-6$ (giving $-3$), square it (giving $9$):

$$x^2-6x+13 = (x^2-6x+9)-9+13 = (x-3)^2+4$$

**12.** $\displaystyle\int \frac{dx}{x^2-6x+13}$

Using the result from Problem 11: $x^2-6x+13=(x-3)^2+4$. Let $u=x-3$, $du=dx$.

$$\int \frac{du}{u^2+4} = \frac12\arctan\left(\frac u2\right)+C = \frac12\arctan\left(\frac{x-3}{2}\right)+C$$

**13.** $\displaystyle\int \frac{dx}{\sqrt{-x^2+2x+3}}$

Complete the square: $-x^2+2x+3 = -(x^2-2x)+3 = -(x^2-2x+1-1)+3 = -(x-1)^2+1+3 = 4-(x-1)^2$.

Let $u=x-1$, $du=dx$.

$$\int \frac{du}{\sqrt{4-u^2}} = \arcsin\left(\frac u2\right)+C = \arcsin\left(\frac{x-1}{2}\right)+C$$

---

### 🔴 Challenge

**14.** $\displaystyle\int \frac{dx}{\sqrt{-x^2+4x-3}}$

Complete the square: $-x^2+4x-3 = -(x^2-4x)-3 = -(x^2-4x+4-4)-3 = -(x-2)^2+4-3 = 1-(x-2)^2$.

Let $u=x-2$, $du=dx$.

$$\int \frac{du}{\sqrt{1-u^2}} = \arcsin(u)+C = \arcsin(x-2)+C$$

**15.** $\displaystyle\int \frac{dx}{x^2+4x+13}$

Complete the square: $x^2+4x+13 = (x^2+4x+4)-4+13 = (x+2)^2+9$.

Let $u=x+2$, $du=dx$.

$$\int \frac{du}{u^2+9} = \frac13\arctan\left(\frac u3\right)+C = \frac13\arctan\left(\frac{x+2}{3}\right)+C$$

**16.** $\displaystyle\int \frac{dx}{\sqrt{8-2x-x^2}}$

Complete the square: $8-2x-x^2 = -(x^2+2x)+8 = -(x^2+2x+1-1)+8 = -(x+1)^2+1+8 = 9-(x+1)^2$.

Let $u=x+1$, $du=dx$.

$$\int \frac{du}{\sqrt{9-u^2}} = \arcsin\left(\frac u3\right)+C = \arcsin\left(\frac{x+1}{3}\right)+C$$

**17.** $\displaystyle\int \frac{(2x+3)\,dx}{x^2+4}$

Split into two separate integrals:

$$\int \frac{2x}{x^2+4}\,dx + \int \frac{3}{x^2+4}\,dx$$

**First piece:** let $w=x^2+4$, $dw=2x\,dx$.

$$\int \frac{dw}{w} = \ln|w|+C = \ln(x^2+4)+C \quad (\text{no absolute value needed, since } x^2+4>0 \text{ always})$$

**Second piece:** using $a=2$:

$$3\cdot\frac12\arctan\left(\frac x2\right)+C = \frac32\arctan\left(\frac x2\right)+C$$

**Combine:**

$$\int \frac{(2x+3)\,dx}{x^2+4} = \ln(x^2+4) + \frac32\arctan\left(\frac{x}{2}\right)+C$$

**18.** $\displaystyle\int \frac{dx}{\sqrt{3-2x-x^2}}$

Complete the square: $3-2x-x^2 = -(x^2+2x)+3 = -(x^2+2x+1-1)+3 = -(x+1)^2+1+3 = 4-(x+1)^2$.

Let $u=x+1$, $du=dx$.

$$\int \frac{du}{\sqrt{4-u^2}} = \arcsin\left(\frac u2\right)+C = \arcsin\left(\frac{x+1}{2}\right)+C$$

---

### 🌍 Applied

**19.** $v(t)=\dfrac{1}{\sqrt{4-t^2}}$, $s(0)=0$.

$$s(t) = \int \frac{dt}{\sqrt{4-t^2}} = \arcsin\left(\frac t2\right)+C$$

Apply $s(0)=0$: $\arcsin(0)+C=0 \Rightarrow C=0$.

**$s(t)=\arcsin\left(\dfrac{t}{2}\right)$.**

**20.** $I(x)=\dfrac{1}{x^2+9}$, find $\displaystyle\int_0^3 I(x)\,dx$.

$$\int_0^3 \frac{dx}{x^2+9} = \left[\frac13\arctan\left(\frac x3\right)\right]_0^3 = \frac13\arctan(1) - \frac13\arctan(0)$$

$$= \frac13\cdot\frac{\pi}{4} - 0 = \frac{\pi}{12}$$

**Answer: $\dfrac{\pi}{12}$.**

**21.** $\displaystyle\int \frac{dx}{\sqrt{-x^2+6x-5}}$

Complete the square: $-x^2+6x-5 = -(x^2-6x)-5 = -(x^2-6x+9-9)-5 = -(x-3)^2+9-5 = 4-(x-3)^2$.

Let $u=x-3$, $du=dx$.

$$\int \frac{du}{\sqrt{4-u^2}} = \arcsin\left(\frac u2\right)+C = \arcsin\left(\frac{x-3}{2}\right)+C$$

**22.** $\displaystyle\int_{-2}^{2} \frac{dx}{\sqrt{4-x^2}}$

$$\left[\arcsin\left(\frac x2\right)\right]_{-2}^{2} = \arcsin(1) - \arcsin(-1) = \frac{\pi}{2} - \left(-\frac{\pi}{2}\right) = \pi$$

**Answer: $\pi$.**
