# Unit 35: Inverse Trigonometric Functions — Full Solutions

### 🟢 Warm-up

**1.** $\arcsin\left(\dfrac12\right) = \dfrac{\pi}{6}$

**2.** $\arccos(0) = \dfrac{\pi}{2}$

**3.** $\arctan(1) = \dfrac{\pi}{4}$

**4.** $\arcsin\left(-\dfrac{\sqrt2}{2}\right) = -\dfrac{\pi}{4}$

**5.** $\arccos(1) = 0$

**6.** $\dfrac{d}{dx}[\arcsin x] = \dfrac{1}{\sqrt{1-x^2}}$

**7.** $\dfrac{d}{dx}[\arctan x] = \dfrac{1}{1+x^2}$

---

### 🟡 Standard

**8.** $\sin\big(\arccos\left(\tfrac35\right)\big)$

Let $\theta=\arccos\left(\frac35\right)$, so $\cos\theta=\frac35=\frac{\text{adjacent}}{\text{hypotenuse}}$. Draw a right triangle with adjacent $=3$, hypotenuse $=5$. By the Pythagorean theorem, opposite $=\sqrt{25-9}=\sqrt{16}=4$.

$$\sin\theta = \frac{\text{opposite}}{\text{hypotenuse}} = \frac45$$

**Answer: $\dfrac45$.**

**9.** $\cos\big(\arcsin\left(\tfrac{5}{13}\right)\big)$

Let $\theta=\arcsin\left(\frac{5}{13}\right)$, so $\sin\theta=\frac{5}{13}=\frac{\text{opposite}}{\text{hypotenuse}}$. Opposite $=5$, hypotenuse $=13$. Adjacent $=\sqrt{169-25}=\sqrt{144}=12$.

$$\cos\theta = \frac{\text{adjacent}}{\text{hypotenuse}} = \frac{12}{13}$$

**Answer: $\dfrac{12}{13}$.**

**10.** $\tan\big(\arcsin\left(\tfrac13\right)\big)$

Let $\theta=\arcsin\left(\frac13\right)$: opposite $=1$, hypotenuse $=3$. Adjacent $=\sqrt{9-1}=\sqrt8=2\sqrt2$.

$$\tan\theta = \frac{\text{opposite}}{\text{adjacent}} = \frac{1}{2\sqrt2} = \frac{\sqrt2}{4}$$

**Answer: $\dfrac{\sqrt2}{4}$.**

**11.** $\dfrac{d}{dx}\big[\arcsin(2x)\big]$

Chain rule: $u=2x$, $u'=2$.

$$\frac{d}{dx}[\arcsin(2x)] = \frac{2}{\sqrt{1-4x^2}}$$

**12.** $\dfrac{d}{dx}\big[\arctan(x^2)\big]$

Chain rule: $u=x^2$, $u'=2x$.

$$\frac{d}{dx}[\arctan(x^2)] = \frac{2x}{1+x^4}$$

**13.** $\dfrac{d}{dx}\big[\arccos(3x)\big]$

Chain rule: $u=3x$, $u'=3$.

$$\frac{d}{dx}[\arccos(3x)] = \frac{-3}{\sqrt{1-9x^2}}$$

**14.** $\sec\big(\arctan(2)\big)$

Let $\theta=\arctan(2)$: opposite $=2$, adjacent $=1$, hypotenuse $=\sqrt{4+1}=\sqrt5$.

$$\sec\theta = \frac{\text{hypotenuse}}{\text{adjacent}} = \frac{\sqrt5}{1} = \sqrt5$$

**Answer: $\sqrt5$.**

---

### 🔴 Challenge

**15.** $y=\arctan(\sin x)$. Find $\dfrac{dy}{dx}$.

Chain rule: $u=\sin x$, $u'=\cos x$.

$$\frac{dy}{dx} = \frac{\cos x}{1+\sin^2x}$$

**16.** $\sin\left(\arccos\left(\dfrac{\sqrt2}{2}\right)\right)$

Recognize $\dfrac{\sqrt2}{2}$ as a standard cosine value: $\arccos\left(\dfrac{\sqrt2}{2}\right) = \dfrac{\pi}{4}$ (since $\cos\left(\frac{\pi}{4}\right)=\frac{\sqrt2}{2}$).

$$\sin\left(\frac{\pi}{4}\right) = \frac{\sqrt2}{2}$$

**Answer: $\dfrac{\sqrt2}{2}$.**

**17.** $\tan\left(\arcsin\left(-\dfrac12\right)\right)$

Recognize $-\dfrac12$ as a standard sine value: $\arcsin\left(-\dfrac12\right) = -\dfrac{\pi}{6}$ (since $\sin\left(-\frac{\pi}{6}\right)=-\frac12$, and this angle lies within $\arcsin$'s range).

$$\tan\left(-\frac{\pi}{6}\right) = -\tan\left(\frac{\pi}{6}\right) = -\frac{1}{\sqrt3} = -\frac{\sqrt3}{3}$$

**Answer: $-\dfrac{\sqrt3}{3}$.**

**18.** $\dfrac{d}{dx}\Big[x\arcsin(x) + \sqrt{1-x^2}\Big]$

**First term** ($x\arcsin x$), product rule: $f=x$ ($f'=1$), $g=\arcsin x$ ($g'=\frac{1}{\sqrt{1-x^2}}$).

$$\frac{d}{dx}[x\arcsin x] = \arcsin x + \frac{x}{\sqrt{1-x^2}}$$

**Second term** ($\sqrt{1-x^2}=(1-x^2)^{1/2}$), chain rule: inner $u=1-x^2$ ($u'=-2x$).

$$\frac{d}{dx}\left[(1-x^2)^{1/2}\right] = \frac12(1-x^2)^{-1/2}(-2x) = \frac{-x}{\sqrt{1-x^2}}$$

**Combine both terms:**

$$\left(\arcsin x + \frac{x}{\sqrt{1-x^2}}\right) + \left(\frac{-x}{\sqrt{1-x^2}}\right) = \arcsin x$$

The two fraction terms cancel exactly.

**$\dfrac{d}{dx}\Big[x\arcsin(x) + \sqrt{1-x^2}\Big] = \arcsin x$.**

**19.** $\cos\big(\arctan\left(\tfrac34\right)\big)$

Let $\theta=\arctan\left(\frac34\right)$: opposite $=3$, adjacent $=4$, hypotenuse $=\sqrt{9+16}=\sqrt{25}=5$.

$$\cos\theta = \frac{\text{adjacent}}{\text{hypotenuse}} = \frac45$$

**Answer: $\dfrac45$.**

---

### 🌍 Applied

**20.** $\theta = \arctan\left(\dfrac{15}{8}\right)$

Note that $8$-$15$-$17$ is a Pythagorean triple ($8^2+15^2=64+225=289=17^2$), so this angle isn't one of the standard "nice" angles, but we can still evaluate it numerically:

$$\theta = \arctan(1.875) \approx 1.081 \text{ radians} \approx 61.93°$$

**Answer: $\theta \approx 61.93°$.**

**21.** $\theta(t)=\arctan\left(\dfrac{x(t)}{50}\right)$, with $x=30$, $\dfrac{dx}{dt}=10$.

Using the chain rule (treating $\frac{x}{50}$ as the "$u$" inside $\arctan$):

$$\frac{d\theta}{dt} = \frac{1}{1+\left(\frac{x}{50}\right)^2}\cdot\frac{1}{50}\cdot\frac{dx}{dt}$$

Plug in $x=30$: $\dfrac{x}{50}=\dfrac{30}{50}=0.6$, so $1+(0.6)^2 = 1+0.36=1.36$.

$$\frac{d\theta}{dt} = \frac{1}{1.36}\cdot\frac{1}{50}\cdot10 = \frac{1}{1.36}\cdot\frac{10}{50} = \frac{1}{1.36}\cdot0.2$$

Working with exact fractions instead: $\dfrac{x}{50}=\dfrac35$, so $1+\left(\dfrac35\right)^2 = 1+\dfrac{9}{25}=\dfrac{34}{25}$.

$$\frac{d\theta}{dt} = \frac{1}{\frac{34}{25}}\cdot\frac{1}{50}\cdot10 = \frac{25}{34}\cdot\frac{10}{50} = \frac{25}{34}\cdot\frac15 = \frac{5}{34}$$

**Answer: $\dfrac{d\theta}{dt} = \dfrac{5}{34} \approx 0.147$ rad/s.**

**22.** $\theta = \arcsin\left(\dfrac{x}{10}\right)$

Chain rule: $u=\dfrac{x}{10}$, $u'=\dfrac{1}{10}$.

$$\frac{d\theta}{dx} = \frac{1/10}{\sqrt{1-\left(\frac{x}{10}\right)^2}} = \frac{1}{10\sqrt{1-\frac{x^2}{100}}} = \frac{1}{\sqrt{100-x^2}}$$

(simplifying by pulling the $10$ inside the square root: $10\sqrt{\frac{100-x^2}{100}} = \sqrt{100-x^2}$).

At $x=6$:

$$\frac{d\theta}{dx}\bigg|_{x=6} = \frac{1}{\sqrt{100-36}} = \frac{1}{\sqrt{64}} = \frac18$$

**Answer: $\dfrac{d\theta}{dx}=\dfrac{1}{\sqrt{100-x^2}}$, and at $x=6$, this equals $\dfrac18$.**

**23.** $\theta = \arccos\left(\dfrac35\right)$

This is the same triangle as Problem 8 (a $3$-$4$-$5$ triangle):

$$\theta = \arccos(0.6) \approx 53.13°$$

**Answer: $\theta \approx 53.13°$.**
