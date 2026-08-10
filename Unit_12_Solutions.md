# Unit 12: Derivatives of Trig Functions — Full Solutions

### 🟢 Warm-up

**1.** $y=\sin x+\cos x$

$$y' = \cos x + (-\sin x) = \cos x - \sin x$$

**2.** $y=3\sin x-2\cos x$

$$y' = 3\cos x - 2(-\sin x) = 3\cos x + 2\sin x$$

**3.** $y=\tan x+5$

$$y' = \sec^2 x + 0 = \sec^2 x$$

**4.** $y=4\cos x-x^2$

$$y' = 4(-\sin x) - 2x = -4\sin x - 2x$$

**5.** $y=\sec x+\cot x$

$$y' = \sec x\tan x + (-\csc^2 x) = \sec x\tan x - \csc^2 x$$

**6.** $y=2\csc x-3\tan x$

$$y' = 2(-\csc x\cot x) - 3\sec^2 x = -2\csc x\cot x - 3\sec^2 x$$

**7.** $y=x+\sin x$

$$y' = 1+\cos x$$

---

### 🟡 Standard

**8.** $y=x\sin x$

Let $f=x$ ($f'=1$), $g=\sin x$ ($g'=\cos x$).

$$y' = 1\cdot\sin x + x\cdot\cos x = \sin x + x\cos x$$

**9.** $y=x^2\cos x$

Let $f=x^2$ ($f'=2x$), $g=\cos x$ ($g'=-\sin x$).

$$y' = 2x\cos x + x^2(-\sin x) = 2x\cos x - x^2\sin x$$

**10.** $y=\dfrac{\sin x}{x}$

Let $f=\sin x$ ($f'=\cos x$), $g=x$ ($g'=1$).

$$y' = \frac{\cos x\cdot x - \sin x\cdot 1}{x^2} = \frac{x\cos x - \sin x}{x^2}$$

**11.** $y=(x+1)\cos x$

Let $f=x+1$ ($f'=1$), $g=\cos x$ ($g'=-\sin x$).

$$y' = 1\cdot\cos x + (x+1)(-\sin x) = \cos x - (x+1)\sin x$$

**12.** $y=\dfrac{\tan x}{x}$

Let $f=\tan x$ ($f'=\sec^2 x$), $g=x$ ($g'=1$).

$$y' = \frac{\sec^2 x\cdot x - \tan x\cdot 1}{x^2} = \frac{x\sec^2 x - \tan x}{x^2}$$

**13.** $y=\sin x\cos x$

Let $f=\sin x$ ($f'=\cos x$), $g=\cos x$ ($g'=-\sin x$).

$$y' = \cos x\cdot\cos x + \sin x\cdot(-\sin x) = \cos^2 x - \sin^2 x$$

**14.** $y=x\cos x-\sin x$

Differentiate the product $x\cos x$ using the product rule: $f=x$ ($f'=1$), $g=\cos x$ ($g'=-\sin x$).

$$\frac{d}{dx}[x\cos x] = 1\cdot\cos x + x(-\sin x) = \cos x - x\sin x$$

Differentiate the remaining term: $\dfrac{d}{dx}[-\sin x] = -\cos x$.

Add them together:

$$y' = (\cos x - x\sin x) + (-\cos x) = -x\sin x$$

**$y' = -x\sin x$.** (Notice the $\cos x$ terms cancelled out completely!)

---

### 🔴 Challenge

**15.** $y=(\sin x+\cos x)(x^2+2x)$

Let $f=\sin x+\cos x$ ($f'=\cos x-\sin x$), $g=x^2+2x$ ($g'=2x+2$).

$$y' = (\cos x - \sin x)(x^2+2x) + (\sin x+\cos x)(2x+2)$$

This is already a complete, correct answer. If you'd like to expand it fully, here's how it simplifies:

Expand the first piece: $(\cos x-\sin x)(x^2+2x) = x^2\cos x + 2x\cos x - x^2\sin x - 2x\sin x$.

Expand the second piece: $(\sin x+\cos x)(2x+2) = 2x\sin x + 2\sin x + 2x\cos x + 2\cos x$.

Add everything and combine like terms (the $-2x\sin x$ and $+2x\sin x$ cancel):

$$y' = x^2\cos x - x^2\sin x + 4x\cos x + 2\sin x + 2\cos x$$

**$y' = (\cos x-\sin x)(x^2+2x) + (\sin x+\cos x)(2x+2)$, which simplifies to $x^2\cos x - x^2\sin x + 4x\cos x + 2\cos x + 2\sin x$.**

**16.** $y=x^2\sin x+2x\cos x-2\sin x$

Differentiate each of the three terms separately.

**Term 1** ($x^2\sin x$, product rule with $f=x^2$, $f'=2x$, $g=\sin x$, $g'=\cos x$):

$$\frac{d}{dx}[x^2\sin x] = 2x\sin x + x^2\cos x$$

**Term 2** ($2x\cos x$, product rule with $f=2x$, $f'=2$, $g=\cos x$, $g'=-\sin x$):

$$\frac{d}{dx}[2x\cos x] = 2\cos x + 2x(-\sin x) = 2\cos x - 2x\sin x$$

**Term 3** ($-2\sin x$):

$$\frac{d}{dx}[-2\sin x] = -2\cos x$$

Add all three results together:

$$y' = \big(2x\sin x + x^2\cos x\big) + \big(2\cos x - 2x\sin x\big) + \big(-2\cos x\big)$$

Combine like terms: the $2x\sin x$ and $-2x\sin x$ cancel; the $2\cos x$ and $-2\cos x$ cancel.

$$y' = x^2\cos x$$

**$y' = x^2\cos x$.** Everything else cancelled out beautifully.

**17.** Deriving $\dfrac{d}{dx}[\tan x]$ from $\tan x = \dfrac{\sin x}{\cos x}$.

Let $f=\sin x$ ($f'=\cos x$) and $g=\cos x$ ($g'=-\sin x$). Apply the quotient rule:

$$\frac{d}{dx}\left[\frac{\sin x}{\cos x}\right] = \frac{\cos x\cdot\cos x - \sin x\cdot(-\sin x)}{(\cos x)^2}$$

Simplify the top:

$$\cos x\cdot\cos x - \sin x\cdot(-\sin x) = \cos^2 x + \sin^2 x$$

By the Pythagorean identity, $\sin^2 x + \cos^2 x = 1$, so the top simplifies to just $1$:

$$\frac{1}{\cos^2 x}$$

Since $\dfrac{1}{\cos x} = \sec x$, we have $\dfrac{1}{\cos^2 x} = \sec^2 x$.

**Answer: $\dfrac{d}{dx}[\tan x] = \sec^2 x$** — confirming the formula from the toolbox, built entirely from the quotient rule and one identity.

**18.** $y=\sec x\tan x$

Let $f=\sec x$ ($f'=\sec x\tan x$), $g=\tan x$ ($g'=\sec^2 x$).

$$y' = (\sec x\tan x)(\tan x) + (\sec x)(\sec^2 x) = \sec x\tan^2 x + \sec^3 x$$

**$y' = \sec x\tan^2 x + \sec^3 x$.** (This can also be rewritten using $\tan^2 x = \sec^2 x - 1$ as $2\sec^3 x - \sec x$, but either form is a correct final answer.)

**19.** $y=\dfrac{x\sin x}{\cos x}$

Simplify first, using $\dfrac{\sin x}{\cos x} = \tan x$:

$$y = x\cdot\frac{\sin x}{\cos x} = x\tan x$$

Now apply the product rule with $f=x$ ($f'=1$), $g=\tan x$ ($g'=\sec^2 x$):

$$y' = 1\cdot\tan x + x\cdot\sec^2 x = \tan x + x\sec^2 x$$

**$y' = \tan x + x\sec^2 x$.** (Simplifying first turned a messy quotient-rule problem into a quick product-rule one.)

**20.** $y=\csc x\cot x$

Let $f=\csc x$ ($f'=-\csc x\cot x$), $g=\cot x$ ($g'=-\csc^2 x$).

$$y' = (-\csc x\cot x)(\cot x) + (\csc x)(-\csc^2 x) = -\csc x\cot^2 x - \csc^3 x$$

**$y' = -\csc x\cot^2 x - \csc^3 x$.**

---

### 🌍 Applied

**21.** $x(t)=5\sin t$

$$v(t) = x'(t) = 5\cos t$$

$v(0) = 5\cos(0) = 5(1) = 5$.

$v\left(\dfrac{\pi}{2}\right) = 5\cos\left(\dfrac{\pi}{2}\right) = 5(0) = 0$.

**In words:** at $t=0$, the pendulum is passing through the center of its swing (where $x(0)=0$) at its **maximum speed** of $5$ cm/s. At $t=\dfrac{\pi}{2}$, the pendulum is momentarily at rest ($v=0$) — this is the instant it reaches the far edge of its swing (where $x\left(\frac{\pi}{2}\right)=5\sin\left(\frac{\pi}{2}\right)=5$, its maximum displacement), right before it swings back.

**22.** $I(t)=100+20\cos t$

$$I'(t) = -20\sin t$$

$$I'\left(\frac{\pi}{2}\right) = -20\sin\left(\frac{\pi}{2}\right) = -20(1) = -20$$

**Answer: $I'(t) = -20\sin t$, and $I'\left(\dfrac{\pi}{2}\right) = -20$.** This means that at $t=\dfrac{\pi}{2}$ hours, sunlight intensity is decreasing at a rate of $20$ units per hour.

**23.** $h(t)=10+8\sin t$

$$h'(t) = 8\cos t$$

$$h'(0) = 8\cos(0) = 8(1) = 8$$

**Answer: $h'(t)=8\cos t$, and $h'(0)=8$.** Since $h'(0)=8$ is positive, **the rider is rising** at $t=0$, moving upward at a rate of $8$ meters per unit of time.

**24.** $V(t)=5\cos t+2\sin t$

$$V'(t) = -5\sin t + 2\cos t$$

$$V'(0) = -5\sin(0)+2\cos(0) = 0+2(1) = 2$$

**Answer: $V'(t)=-5\sin t+2\cos t$, and $V'(0)=2$.** This means that at $t=0$, the voltage is increasing at a rate of $2$ volts per unit of time.
