# Unit 39: Trigonometric Substitution — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int \frac{dx}{\sqrt{9-x^2}}$ — this matches $\sqrt{a^2-x^2}$ (with $a=3$), so use **$x=3\sin\theta$**.

**2.** $\displaystyle\int \frac{dx}{\sqrt{x^2+16}}$ — this matches $\sqrt{a^2+x^2}$ (with $a=4$), so use **$x=4\tan\theta$**.

**3.** $\displaystyle\int \frac{dx}{\sqrt{x^2-25}}$ — this matches $\sqrt{x^2-a^2}$ (with $a=5$), so use **$x=5\sec\theta$**.

**4.** $\displaystyle\int \frac{dx}{\sqrt{4-x^2}}$, $x=2\sin\theta$

$dx=2\cos\theta\,d\theta$, $\sqrt{4-x^2}=2\cos\theta$.

$$\int \frac{2\cos\theta\,d\theta}{2\cos\theta} = \int d\theta = \theta+C = \arcsin\left(\frac{x}{2}\right)+C$$

(This matches the direct arcsin formula from Unit 36 — good confirmation that trig substitution gives the same answer.)

**5.** $\displaystyle\int \frac{dx}{\sqrt{9-x^2}}$, $x=3\sin\theta$

$dx=3\cos\theta\,d\theta$, $\sqrt{9-x^2}=3\cos\theta$.

$$\int d\theta = \theta+C = \arcsin\left(\frac{x}{3}\right)+C$$

**6.** $\displaystyle\int \sqrt{1-x^2}\,dx$, $x=\sin\theta$

$dx=\cos\theta\,d\theta$, $\sqrt{1-x^2}=\cos\theta$.

$$\int \cos\theta\cdot\cos\theta\,d\theta = \int \cos^2\theta\,d\theta = \frac{\theta}{2}+\frac{\sin(2\theta)}{4}+C = \frac{\theta}{2}+\frac{\sin\theta\cos\theta}{2}+C$$

Convert: $\theta=\arcsin x$, $\sin\theta=x$, $\cos\theta=\sqrt{1-x^2}$.

$$= \frac12\arcsin x + \frac{x\sqrt{1-x^2}}{2}+C$$

---

### 🟡 Standard

**7.** $\displaystyle\int \frac{x^2}{\sqrt{4-x^2}}\,dx$, $x=2\sin\theta$

$x^2=4\sin^2\theta$, $\sqrt{4-x^2}=2\cos\theta$, $dx=2\cos\theta\,d\theta$.

$$\int \frac{4\sin^2\theta}{2\cos\theta}\cdot2\cos\theta\,d\theta = \int 4\sin^2\theta\,d\theta = 4\left(\frac{\theta}{2}-\frac{\sin(2\theta)}{4}\right) = 2\theta-\sin(2\theta)+C$$

Convert: $\theta=\arcsin\left(\frac x2\right)$, $\sin(2\theta)=2\sin\theta\cos\theta = 2\cdot\frac x2\cdot\frac{\sqrt{4-x^2}}{2} = \frac{x\sqrt{4-x^2}}{2}$.

$$= 2\arcsin\left(\frac{x}{2}\right) - \frac{x\sqrt{4-x^2}}{2}+C$$

**8.** $\displaystyle\int \frac{dx}{\sqrt{x^2+4}}$, $x=2\tan\theta$

$dx=2\sec^2\theta\,d\theta$, $\sqrt{x^2+4}=2\sec\theta$.

$$\int \frac{2\sec^2\theta\,d\theta}{2\sec\theta} = \int \sec\theta\,d\theta = \ln|\sec\theta+\tan\theta|+C$$

Convert: $\tan\theta=\frac x2$, $\sec\theta=\frac{\sqrt{x^2+4}}{2}$.

$$= \ln\left|\frac{\sqrt{x^2+4}+x}{2}\right|+C = \ln\big(\sqrt{x^2+4}+x\big)+C$$

(absorbing the constant $-\ln2$ into $C$).

**9.** $\displaystyle\int \frac{dx}{\sqrt{x^2+9}}$, $x=3\tan\theta$

$dx=3\sec^2\theta\,d\theta$, $\sqrt{x^2+9}=3\sec\theta$.

$$\int \sec\theta\,d\theta = \ln|\sec\theta+\tan\theta|+C$$

Convert: $\tan\theta=\frac x3$, $\sec\theta=\frac{\sqrt{x^2+9}}{3}$.

$$= \ln\big(\sqrt{x^2+9}+x\big)+C$$

**10.** $\displaystyle\int \frac{dx}{(x^2+4)^{3/2}}$, $x=2\tan\theta$

$dx=2\sec^2\theta\,d\theta$, $(x^2+4)^{3/2}=(4\sec^2\theta)^{3/2}=8\sec^3\theta$.

$$\int \frac{2\sec^2\theta\,d\theta}{8\sec^3\theta} = \frac14\int \cos\theta\,d\theta = \frac14\sin\theta+C$$

Convert: from the triangle (opposite $=x$, adjacent $=2$, hypotenuse $=\sqrt{x^2+4}$), $\sin\theta=\dfrac{x}{\sqrt{x^2+4}}$.

$$= \frac{x}{4\sqrt{x^2+4}}+C$$

**11.** $\displaystyle\int \frac{dx}{\sqrt{x^2-4}}$, $x=2\sec\theta$

$dx=2\sec\theta\tan\theta\,d\theta$, $\sqrt{x^2-4}=2\tan\theta$.

$$\int \frac{2\sec\theta\tan\theta\,d\theta}{2\tan\theta} = \int \sec\theta\,d\theta = \ln|\sec\theta+\tan\theta|+C$$

Convert: $\sec\theta=\frac x2$, $\tan\theta=\frac{\sqrt{x^2-4}}{2}$.

$$= \ln\big(x+\sqrt{x^2-4}\big)+C$$

**12.** $\displaystyle\int \frac{dx}{x^2\sqrt{x^2-9}}$, $x=3\sec\theta$

$dx=3\sec\theta\tan\theta\,d\theta$, $\sqrt{x^2-9}=3\tan\theta$, $x^2=9\sec^2\theta$.

$$\int \frac{3\sec\theta\tan\theta\,d\theta}{9\sec^2\theta\cdot3\tan\theta} = \int \frac{d\theta}{9\sec\theta} = \frac19\int \cos\theta\,d\theta = \frac19\sin\theta+C$$

Convert: from the triangle (adjacent $=3$, hypotenuse $=x$, opposite $=\sqrt{x^2-9}$), $\sin\theta=\dfrac{\sqrt{x^2-9}}{x}$.

$$= \frac{\sqrt{x^2-9}}{9x}+C$$

---

### 🔴 Challenge

**13.** $\displaystyle\int \sqrt{9-x^2}\,dx$, $x=3\sin\theta$

$dx=3\cos\theta\,d\theta$, $\sqrt{9-x^2}=3\cos\theta$.

$$\int 3\cos\theta\cdot3\cos\theta\,d\theta = 9\int \cos^2\theta\,d\theta = 9\left(\frac{\theta}{2}+\frac{\sin\theta\cos\theta}{2}\right)+C$$

Convert: $\theta=\arcsin\left(\frac x3\right)$, $\sin\theta=\frac x3$, $\cos\theta=\frac{\sqrt{9-x^2}}{3}$.

$$= \frac{9}{2}\arcsin\left(\frac{x}{3}\right) + \frac{9}{2}\cdot\frac{x}{3}\cdot\frac{\sqrt{9-x^2}}{3} + C = \frac{9}{2}\arcsin\left(\frac{x}{3}\right) + \frac{x\sqrt{9-x^2}}{2} + C$$

**14.** $\displaystyle\int x^2\sqrt{9-x^2}\,dx$, $x=3\sin\theta$

$x^2=9\sin^2\theta$, $\sqrt{9-x^2}=3\cos\theta$, $dx=3\cos\theta\,d\theta$.

$$\int 9\sin^2\theta\cdot3\cos\theta\cdot3\cos\theta\,d\theta = 81\int \sin^2\theta\cos^2\theta\,d\theta$$

Using the Unit 38 technique, $\sin^2\theta\cos^2\theta = \dfrac14\sin^2(2\theta)$:

$$81\cdot\frac14\int \sin^2(2\theta)\,d\theta = \frac{81}{4}\int \frac{1-\cos(4\theta)}{2}\,d\theta = \frac{81}{8}\left[\theta - \frac{\sin(4\theta)}{4}\right]+C$$

$$= \frac{81\theta}{8} - \frac{81}{32}\sin(4\theta) + C$$

Convert: $\theta=\arcsin\left(\frac x3\right)$. We need $\sin(4\theta) = 2\sin(2\theta)\cos(2\theta)$.

$\sin(2\theta)=2\sin\theta\cos\theta = 2\cdot\frac x3\cdot\frac{\sqrt{9-x^2}}{3} = \dfrac{2x\sqrt{9-x^2}}{9}$.

$\cos(2\theta)=1-2\sin^2\theta = 1-\dfrac{2x^2}{9} = \dfrac{9-2x^2}{9}$.

$$\sin(4\theta) = 2\cdot\frac{2x\sqrt{9-x^2}}{9}\cdot\frac{9-2x^2}{9} = \frac{4x\sqrt{9-x^2}(9-2x^2)}{81}$$

Substituting back:

$$\frac{81}{32}\sin(4\theta) = \frac{81}{32}\cdot\frac{4x\sqrt{9-x^2}(9-2x^2)}{81} = \frac{x\sqrt{9-x^2}(9-2x^2)}{8}$$

**Final answer:**

$$\int x^2\sqrt{9-x^2}\,dx = \frac{81}{8}\arcsin\left(\frac{x}{3}\right) - \frac{x(9-2x^2)\sqrt{9-x^2}}{8} + C$$

**15.** $\displaystyle\int \frac{dx}{\sqrt{x^2+16}}$, $x=4\tan\theta$

$dx=4\sec^2\theta\,d\theta$, $\sqrt{x^2+16}=4\sec\theta$.

$$\int \sec\theta\,d\theta = \ln|\sec\theta+\tan\theta|+C$$

Convert: $\tan\theta=\frac x4$, $\sec\theta=\frac{\sqrt{x^2+16}}{4}$.

$$= \ln\big(\sqrt{x^2+16}+x\big)+C$$

**16.** $\displaystyle\int \frac{dx}{(x^2+9)^{3/2}}$, $x=3\tan\theta$

$dx=3\sec^2\theta\,d\theta$, $(x^2+9)^{3/2}=(9\sec^2\theta)^{3/2}=27\sec^3\theta$.

$$\int \frac{3\sec^2\theta\,d\theta}{27\sec^3\theta} = \frac19\int \cos\theta\,d\theta = \frac19\sin\theta+C$$

Convert: $\sin\theta=\dfrac{x}{\sqrt{x^2+9}}$.

$$= \frac{x}{9\sqrt{x^2+9}}+C$$

**17.** $\displaystyle\int \frac{dx}{x^2\sqrt{x^2-4}}$, $x=2\sec\theta$

$dx=2\sec\theta\tan\theta\,d\theta$, $\sqrt{x^2-4}=2\tan\theta$, $x^2=4\sec^2\theta$.

$$\int \frac{2\sec\theta\tan\theta\,d\theta}{4\sec^2\theta\cdot2\tan\theta} = \int \frac{d\theta}{4\sec\theta} = \frac14\int \cos\theta\,d\theta = \frac14\sin\theta+C$$

Convert: from the triangle (adjacent $=2$, hypotenuse $=x$, opposite $=\sqrt{x^2-4}$), $\sin\theta=\dfrac{\sqrt{x^2-4}}{x}$.

$$= \frac{\sqrt{x^2-4}}{4x}+C$$

---

### 🌍 Applied

**18.** $\displaystyle\int_{-2}^{2} \sqrt{4-x^2}\,dx$

Following the same steps as Problem 13 (scaled to $a=2$ instead of $a=3$), the antiderivative is:

$$2\arcsin\left(\frac{x}{2}\right) + \frac{x\sqrt{4-x^2}}{2}$$

Evaluate at $x=2$: $2\arcsin(1) + \dfrac{2\cdot0}{2} = 2\cdot\dfrac{\pi}{2}+0 = \pi$.

Evaluate at $x=-2$: $2\arcsin(-1) + \dfrac{-2\cdot0}{2} = -\pi+0 = -\pi$.

$$\pi - (-\pi) = 2\pi$$

**Answer: $2\pi$.** This matches the known area of a semicircle of radius $2$: $\dfrac12\pi r^2 = \dfrac12\pi(4) = 2\pi$ — confirmed!

**19.** $\displaystyle\int_0^3 x^2\sqrt{9-x^2}\,dx$

Using the antiderivative from Problem 14: $\dfrac{81}{8}\arcsin\left(\dfrac x3\right) - \dfrac{x(9-2x^2)\sqrt{9-x^2}}{8}$.

At $x=3$: $\arcsin(1)=\dfrac{\pi}{2}$; the second term has a factor of $\sqrt{9-9}=0$, so it vanishes. Value $=\dfrac{81}{8}\cdot\dfrac{\pi}{2} = \dfrac{81\pi}{16}$.

At $x=0$: both terms are $0$.

$$\frac{81\pi}{16} - 0 = \frac{81\pi}{16}$$

**Answer: $\dfrac{81\pi}{16}$.**

**20.** $\displaystyle\int_0^4 \frac{dx}{\sqrt{x^2+16}}$

Using the antiderivative from Problem 15: $\ln\big(\sqrt{x^2+16}+x\big)$.

At $x=4$: $\ln\big(\sqrt{32}+4\big) = \ln\big(4\sqrt2+4\big) = \ln\big(4(\sqrt2+1)\big) = \ln4+\ln(\sqrt2+1)$.

At $x=0$: $\ln\big(\sqrt{16}+0\big) = \ln4$.

$$\big[\ln4+\ln(\sqrt2+1)\big] - \ln4 = \ln(\sqrt2+1)$$

**Answer: $\ln(\sqrt2+1) \approx 0.881$.**

**21.** $\displaystyle\int_3^{3\sqrt2} \frac{dx}{x^2\sqrt{x^2-9}}$

Following the same steps as Problem 12 (with $a=3$), the antiderivative is $\dfrac{\sqrt{x^2-9}}{9x}$.

At $x=3\sqrt2$: $\sqrt{(3\sqrt2)^2-9} = \sqrt{18-9}=\sqrt9=3$. Value $=\dfrac{3}{9(3\sqrt2)} = \dfrac{3}{27\sqrt2} = \dfrac{1}{9\sqrt2} = \dfrac{\sqrt2}{18}$.

At $x=3$: $\sqrt{9-9}=0$. Value $=0$.

$$\frac{\sqrt2}{18} - 0 = \frac{\sqrt2}{18}$$

**Answer: $\dfrac{\sqrt2}{18}$.**
