# Unit 13: The Chain Rule — Full Solutions

### 🟢 Warm-up

**1.** $y=(x+3)^4$

Outer layer: something to the 4th power. Inner layer: $u=x+3$, so $u'=1$.

$$y' = 4(x+3)^3\cdot 1 = 4(x+3)^3$$

**2.** $y=(2x-1)^5$

Inner: $u=2x-1$, $u'=2$.

$$y' = 5(2x-1)^4\cdot 2 = 10(2x-1)^4$$

**3.** $y=(3x+2)^3$

Inner: $u=3x+2$, $u'=3$.

$$y' = 3(3x+2)^2\cdot 3 = 9(3x+2)^2$$

**4.** $y=(x^2+1)^3$

Inner: $u=x^2+1$, $u'=2x$.

$$y' = 3(x^2+1)^2\cdot 2x = 6x(x^2+1)^2$$

**5.** $y=(5-x)^4$

Inner: $u=5-x$, $u'=-1$.

$$y' = 4(5-x)^3\cdot(-1) = -4(5-x)^3$$

**6.** $y=(4x+7)^2$

Inner: $u=4x+7$, $u'=4$.

$$y' = 2(4x+7)\cdot 4 = 8(4x+7)$$

**7.** $y=(x^2-2x)^2$

Inner: $u=x^2-2x$, $u'=2x-2$.

$$y' = 2(x^2-2x)\cdot(2x-2)$$

We can factor this further: $x^2-2x = x(x-2)$ and $2x-2=2(x-1)$, so:

$$y' = 2\cdot x(x-2)\cdot 2(x-1) = 4x(x-1)(x-2)$$

**$y' = 4x(x-1)(x-2)$.**

---

### 🟡 Standard

**8.** $y=\sin(3x)$

Inner: $u=3x$, $u'=3$.

$$y' = \cos(3x)\cdot 3 = 3\cos(3x)$$

**9.** $y=\cos(x^2)$

Inner: $u=x^2$, $u'=2x$.

$$y' = -\sin(x^2)\cdot 2x = -2x\sin(x^2)$$

**10.** $y=(2x^2-3)^{-1}$

Inner: $u=2x^2-3$, $u'=4x$.

$$y' = -1\cdot(2x^2-3)^{-2}\cdot 4x = \frac{-4x}{(2x^2-3)^2}$$

**11.** $y=\sqrt{x^2+4} = (x^2+4)^{1/2}$

Inner: $u=x^2+4$, $u'=2x$.

$$y' = \frac{1}{2}(x^2+4)^{-1/2}\cdot 2x = x(x^2+4)^{-1/2} = \frac{x}{\sqrt{x^2+4}}$$

**12.** $y=\tan(2x)$

Inner: $u=2x$, $u'=2$.

$$y' = \sec^2(2x)\cdot 2 = 2\sec^2(2x)$$

**13.** $y=(3x-1)^{1/3}$

Inner: $u=3x-1$, $u'=3$.

$$y' = \frac{1}{3}(3x-1)^{-2/3}\cdot 3 = (3x-1)^{-2/3} = \frac{1}{(3x-1)^{2/3}}$$

**14.** $y=\sin^2 x = (\sin x)^2$

Inner: $u=\sin x$, $u'=\cos x$.

$$y' = 2(\sin x)^1\cdot\cos x = 2\sin x\cos x$$

---

### 🔴 Challenge

**15.** $y=\left(\dfrac{x^2}{2}+x-\dfrac{1}{x}\right)^4$

First, find the derivative of the inner expression. Rewrite $-\dfrac{1}{x}$ as $-x^{-1}$:

$$u = \frac{x^2}{2}+x-x^{-1}$$

$$u' = x + 1 - (-1)x^{-2} = x+1+x^{-2} = x+1+\frac{1}{x^2}$$

Now apply the power chain rule (outer power is $4$):

$$y' = 4\left(\frac{x^2}{2}+x-\frac{1}{x}\right)^3\cdot\left(x+1+\frac{1}{x^2}\right)$$

**$y' = 4\left(\dfrac{x^2}{2}+x-\dfrac{1}{x}\right)^3\left(x+1+\dfrac{1}{x^2}\right)$.**

**16.** $y=\sin^4 x = (\sin x)^4$

Inner: $u=\sin x$, $u'=\cos x$.

$$y' = 4(\sin x)^3\cdot\cos x = 4\sin^3 x\cos x$$

**17.** $y = x^2\sin^4 x + x\cos^{-2}x$

This has **two terms**, and each one needs the product rule (since each is a plain factor times a trig-composition factor).

**Term 1: $x^2\sin^4 x$.** Let $f=x^2$ ($f'=2x$) and $g=\sin^4 x$ (from Problem 16, $g'=4\sin^3x\cos x$).

$$\frac{d}{dx}\big[x^2\sin^4 x\big] = 2x\sin^4 x + x^2\cdot 4\sin^3x\cos x = 2x\sin^4 x + 4x^2\sin^3x\cos x$$

**Term 2: $x\cos^{-2}x$.** Let $f=x$ ($f'=1$) and $g=\cos^{-2}x = (\cos x)^{-2}$.

Find $g'$ using the power chain rule, with inner $u=\cos x$ ($u'=-\sin x$):

$$g' = -2(\cos x)^{-3}\cdot(-\sin x) = 2\sin x(\cos x)^{-3} = \frac{2\sin x}{\cos^3 x}$$

$$\frac{d}{dx}\big[x\cos^{-2}x\big] = 1\cdot\cos^{-2}x + x\cdot\frac{2\sin x}{\cos^3 x} = \sec^2 x + \frac{2x\sin x}{\cos^3 x}$$

Note $\dfrac{2x\sin x}{\cos^3 x} = 2x\left(\dfrac{\sin x}{\cos x}\right)\left(\dfrac{1}{\cos^2 x}\right) = 2x\tan x\sec^2 x$.

**Adding both terms together:**

$$y' = \big(2x\sin^4 x + 4x^2\sin^3x\cos x\big) + \big(\sec^2 x + 2x\tan x\sec^2 x\big)$$

**$y' = 2x\sin^4 x + 4x^2\sin^3x\cos x + \sec^2 x + 2x\tan x\sec^2 x$.**

**18.** $y = (x^2+1)^3(x-1)^2$

Let $f=(x^2+1)^3$. Using the power chain rule (inner $u=x^2+1$, $u'=2x$):

$$f' = 3(x^2+1)^2\cdot 2x = 6x(x^2+1)^2$$

Let $g=(x-1)^2$, so $g'=2(x-1)$.

Apply the product rule:

$$y' = f'g+fg' = 6x(x^2+1)^2(x-1)^2 + (x^2+1)^3\cdot 2(x-1)$$

Both terms share a common factor of $(x^2+1)^2(x-1)$. Factor it out:

$$y' = (x^2+1)^2(x-1)\Big[6x(x-1) + 2(x^2+1)\Big]$$

Simplify inside the brackets: $6x(x-1) = 6x^2-6x$, and adding $2(x^2+1)=2x^2+2$ gives $6x^2-6x+2x^2+2 = 8x^2-6x+2$.

$$y' = (x^2+1)^2(x-1)(8x^2-6x+2)$$

We can factor out a $2$ from the last piece:

$$y' = 2(x^2+1)^2(x-1)(4x^2-3x+1)$$

**$y' = 2(x^2+1)^2(x-1)(4x^2-3x+1)$.**

**19.** $y = \sqrt{\sin x} = (\sin x)^{1/2}$

Inner: $u=\sin x$, $u'=\cos x$.

$$y' = \frac{1}{2}(\sin x)^{-1/2}\cdot\cos x = \frac{\cos x}{2\sqrt{\sin x}}$$

**20.** $y = (1+\cos x)^3$

Inner: $u=1+\cos x$, $u'=-\sin x$.

$$y' = 3(1+\cos x)^2\cdot(-\sin x) = -3\sin x(1+\cos x)^2$$

---

### 🌍 Applied

**21.** $V(r)=\dfrac{4}{3}\pi r^3$, where $r(t)=2t$.

Using the chain rule, $\dfrac{dV}{dt} = \dfrac{dV}{dr}\cdot\dfrac{dr}{dt}$.

$$\frac{dV}{dr} = 4\pi r^2 \qquad \frac{dr}{dt} = 2$$

$$\frac{dV}{dt} = 4\pi r^2 \cdot 2 = 8\pi r^2$$

At $t=1$: $r(1) = 2(1) = 2$, so:

$$\frac{dV}{dt}\Big|_{t=1} = 8\pi(2)^2 = 8\pi(4) = 32\pi$$

**Answer: $\dfrac{dV}{dt} = 8\pi r^2$, and at $t=1$, $\dfrac{dV}{dt} = 32\pi$ cubic cm per unit time.**

**22.** $h(t)=3\sin(2t)$

Inner: $u=2t$, $u'=2$.

$$h'(t) = 3\cos(2t)\cdot 2 = 6\cos(2t)$$

$$h'(0) = 6\cos(0) = 6(1) = 6$$

**Answer: $h'(t)=6\cos(2t)$, and $h'(0)=6$.** At $t=0$, the wave height is increasing at a rate of $6$ cm per unit time.

**23.** $C(x)=\sqrt{x^2+50}$, where $x(t)=10t$.

Using the chain rule, $\dfrac{dC}{dt} = \dfrac{dC}{dx}\cdot\dfrac{dx}{dt}$.

$$\frac{dC}{dx} = \frac{1}{2}(x^2+50)^{-1/2}\cdot 2x = \frac{x}{\sqrt{x^2+50}} \qquad \frac{dx}{dt} = 10$$

$$\frac{dC}{dt} = \frac{x}{\sqrt{x^2+50}}\cdot 10$$

At $t=2$: $x(2) = 10(2) = 20$.

$$\sqrt{20^2+50} = \sqrt{400+50} = \sqrt{450} = \sqrt{225\cdot 2} = 15\sqrt{2}$$

$$\frac{dC}{dt}\Big|_{t=2} = \frac{20}{15\sqrt{2}}\cdot 10 = \frac{200}{15\sqrt{2}} = \frac{40}{3\sqrt{2}} = \frac{40\sqrt{2}}{6} = \frac{20\sqrt{2}}{3}$$

**Answer: at $t=2$, $\dfrac{dC}{dt} = \dfrac{20\sqrt{2}}{3} \approx 9.43$ dollars per unit time.**

**24.** $T(t) = (t+2)^3-5$

Inner: $u=t+2$, $u'=1$.

$$T'(t) = 3(t+2)^2\cdot 1 = 3(t+2)^2$$

$$T'(1) = 3(1+2)^2 = 3(9) = 27$$

**Answer: $T'(t)=3(t+2)^2$, and $T'(1)=27$.** At $t=1$, the greenhouse temperature is increasing at a rate of $27°F$ per unit time.
