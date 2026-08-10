# Unit 38: Trigonometric Integrals — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int \sin^3x\,dx$

Odd power on sine. Write $\sin^3x = \sin^2x\cdot\sin x = (1-\cos^2x)\sin x$. Let $u=\cos x$, $du=-\sin x\,dx \Rightarrow \sin x\,dx = -du$.

$$\int (1-u^2)(-du) = -\int(1-u^2)\,du = -u+\frac{u^3}{3}+C = -\cos x+\frac{\cos^3x}{3}+C$$

**2.** $\displaystyle\int \cos^3x\,dx$

Odd power on cosine. Write $\cos^3x = (1-\sin^2x)\cos x$. Let $u=\sin x$, $du=\cos x\,dx$.

$$\int (1-u^2)\,du = u-\frac{u^3}{3}+C = \sin x - \frac{\sin^3x}{3}+C$$

**3.** $\displaystyle\int \sin x\cos^2x\,dx$

Let $u=\cos x$, $du=-\sin x\,dx \Rightarrow \sin x\,dx=-du$.

$$\int u^2(-du) = -\frac{u^3}{3}+C = -\frac{\cos^3x}{3}+C$$

**4.** $\displaystyle\int \sin^2x\cos x\,dx$

Let $u=\sin x$, $du=\cos x\,dx$.

$$\int u^2\,du = \frac{u^3}{3}+C = \frac{\sin^3x}{3}+C$$

**5.** $\displaystyle\int \cos^3x\sin x\,dx$

Let $u=\cos x$, $du=-\sin x\,dx \Rightarrow \sin x\,dx=-du$.

$$\int u^3(-du) = -\frac{u^4}{4}+C = -\frac{\cos^4x}{4}+C$$

**6.** $\displaystyle\int \sin^2x\,dx$

Power-reducing identity:

$$\int \frac{1-\cos(2x)}{2}\,dx = \frac12\left[x-\frac12\sin(2x)\right]+C = \frac{x}{2}-\frac{\sin(2x)}{4}+C$$

---

### 🟡 Standard

**7.** $\displaystyle\int \cos^2x\,dx$

$$\int \frac{1+\cos(2x)}{2}\,dx = \frac12\left[x+\frac12\sin(2x)\right]+C = \frac{x}{2}+\frac{\sin(2x)}{4}+C$$

**8.** $\displaystyle\int \sin^3x\cos^2x\,dx$

Odd power on sine. Write $\sin^3x = (1-\cos^2x)\sin x$.

$$\int (1-\cos^2x)\sin x\cos^2x\,dx = \int (\cos^2x-\cos^4x)\sin x\,dx$$

Let $u=\cos x$, $du=-\sin x\,dx \Rightarrow \sin x\,dx=-du$.

$$\int (u^2-u^4)(-du) = -\left[\frac{u^3}{3}-\frac{u^5}{5}\right]+C = -\frac{\cos^3x}{3}+\frac{\cos^5x}{5}+C$$

**9.** $\displaystyle\int \cos^3x\sin^4x\,dx$

Odd power on cosine. Write $\cos^3x = (1-\sin^2x)\cos x$.

$$\int (1-\sin^2x)\cos x\sin^4x\,dx = \int (\sin^4x-\sin^6x)\cos x\,dx$$

Let $u=\sin x$, $du=\cos x\,dx$.

$$\int (u^4-u^6)\,du = \frac{u^5}{5}-\frac{u^7}{7}+C = \frac{\sin^5x}{5}-\frac{\sin^7x}{7}+C$$

**10.** $\displaystyle\int \sin^4x\cos x\,dx$

Let $u=\sin x$, $du=\cos x\,dx$.

$$\int u^4\,du = \frac{u^5}{5}+C = \frac{\sin^5x}{5}+C$$

**11.** $\displaystyle\int \cos^5x\,dx$

Write $\cos^5x = (\cos^2x)^2\cos x = (1-\sin^2x)^2\cos x$. Let $u=\sin x$, $du=\cos x\,dx$.

$$(1-u^2)^2 = 1-2u^2+u^4$$

$$\int (1-2u^2+u^4)\,du = u-\frac{2u^3}{3}+\frac{u^5}{5}+C = \sin x - \frac23\sin^3x + \frac15\sin^5x+C$$

**12.** $\displaystyle\int \sin^4x\,dx$

Both powers even. Write $\sin^4x = (\sin^2x)^2 = \left(\dfrac{1-\cos(2x)}{2}\right)^2 = \dfrac{1-2\cos(2x)+\cos^2(2x)}{4}$.

Reduce the leftover $\cos^2(2x)$ term using the identity again: $\cos^2(2x) = \dfrac{1+\cos(4x)}{2}$.

$$\sin^4x = \frac{1-2\cos(2x)+\frac{1+\cos(4x)}{2}}{4} = \frac{3-4\cos(2x)+\cos(4x)}{8}$$

$$\int \sin^4x\,dx = \frac18\int \big[3-4\cos(2x)+\cos(4x)\big]\,dx = \frac18\left[3x-2\sin(2x)+\frac14\sin(4x)\right]+C$$

$$= \frac{3x}{8}-\frac{\sin(2x)}{4}+\frac{\sin(4x)}{32}+C$$

---

### 🔴 Challenge

**13.** $\displaystyle\int \sin^5x\,dx$

Write $\sin^5x = (\sin^2x)^2\sin x = (1-\cos^2x)^2\sin x$. Let $u=\cos x$, $du=-\sin x\,dx \Rightarrow \sin x\,dx=-du$.

$$(1-u^2)^2 = 1-2u^2+u^4$$

$$\int (1-2u^2+u^4)(-du) = -\left[u-\frac{2u^3}{3}+\frac{u^5}{5}\right]+C = -\cos x+\frac23\cos^3x-\frac15\cos^5x+C$$

**14.** $\displaystyle\int \sin^6x\cos^3x\,dx$

Odd power on cosine. Write $\cos^3x = (1-\sin^2x)\cos x$.

$$\int \sin^6x(1-\sin^2x)\cos x\,dx = \int (\sin^6x-\sin^8x)\cos x\,dx$$

Let $u=\sin x$, $du=\cos x\,dx$.

$$\int (u^6-u^8)\,du = \frac{u^7}{7}-\frac{u^9}{9}+C = \frac{\sin^7x}{7}-\frac{\sin^9x}{9}+C$$

**15.** $\displaystyle\int \cos^2x\sin^2x\,dx$

Both even. Use the identity $\sin x\cos x = \dfrac12\sin(2x)$, so $\sin^2x\cos^2x = \dfrac14\sin^2(2x)$.

$$\int \frac14\sin^2(2x)\,dx = \frac14\int \sin^2(2x)\,dx$$

Apply the power-reducing identity to $\sin^2(2x) = \dfrac{1-\cos(4x)}{2}$:

$$\frac14\int \frac{1-\cos(4x)}{2}\,dx = \frac18\int \big[1-\cos(4x)\big]\,dx = \frac18\left[x-\frac14\sin(4x)\right]+C$$

$$= \frac{x}{8}-\frac{\sin(4x)}{32}+C$$

**16.** $\displaystyle\int_0^{\pi/2} \sqrt{1+\cos(2x)}\,dx$

Using the identity $1+\cos(2x)=2\cos^2x$:

$$\sqrt{1+\cos(2x)} = \sqrt{2\cos^2x} = \sqrt2\,|\cos x|$$

On $\left[0,\frac{\pi}{2}\right]$, $\cos x\ge0$, so $|\cos x|=\cos x$.

$$\int_0^{\pi/2} \sqrt2\cos x\,dx = \sqrt2\Big[\sin x\Big]_0^{\pi/2} = \sqrt2(1-0) = \sqrt2$$

**Answer: $\sqrt2$.**

**17.** $\displaystyle\int_{-\pi/4}^{\pi/4} \sqrt{1-\cos(2x)}\,dx$

Using the identity $1-\cos(2x)=2\sin^2x$:

$$\sqrt{1-\cos(2x)} = \sqrt2\,|\sin x|$$

On $\left[-\frac{\pi}{4},\frac{\pi}{4}\right]$, $\sin x$ is **negative** on $\left[-\frac{\pi}{4},0\right)$ and **positive** on $\left(0,\frac{\pi}{4}\right]$ — so we must split the integral at $x=0$.

$$\int_{-\pi/4}^{0} \sqrt2(-\sin x)\,dx + \int_0^{\pi/4} \sqrt2\sin x\,dx$$

**First piece:** $\sqrt2\Big[\cos x\Big]_{-\pi/4}^{0} = \sqrt2\left(\cos0-\cos\left(-\frac{\pi}{4}\right)\right) = \sqrt2\left(1-\frac{\sqrt2}{2}\right) = \sqrt2-1$.

**Second piece:** $\sqrt2\Big[-\cos x\Big]_0^{\pi/4} = \sqrt2\left(-\cos\frac{\pi}{4}-(-\cos0)\right) = \sqrt2\left(-\frac{\sqrt2}{2}+1\right) = \sqrt2-1$.

$$\text{Total} = (\sqrt2-1)+(\sqrt2-1) = 2\sqrt2-2$$

**Answer: $2\sqrt2-2 \approx 0.828$.** (You can double-check this using symmetry: since $\sqrt{1-\cos(2x)}$ is an even function of $x$, the integral equals twice the integral from $0$ to $\frac{\pi}{4}$, which is $2(\sqrt2-1)=2\sqrt2-2$ — matching exactly.)

---

### 🌍 Applied

**18.** $\displaystyle\int_0^{2\pi} \sin^2x\,dx$

Using the antiderivative from Problem 6: $\dfrac{x}{2}-\dfrac{\sin(2x)}{4}$.

$$\left[\frac{x}{2}-\frac{\sin(2x)}{4}\right]_0^{2\pi} = \left(\pi - \frac{\sin(4\pi)}{4}\right) - (0-0) = \pi - 0 = \pi$$

**Answer: $\pi$.**

**19.** $\displaystyle\int_0^{\pi} \cos^2x\sin x\,dx$

Let $u=\cos x$, $du=-\sin x\,dx \Rightarrow \sin x\,dx=-du$. When $x=0$, $u=1$; when $x=\pi$, $u=-1$.

$$\int_1^{-1} u^2(-du) = \int_{-1}^{1} u^2\,du = \left[\frac{u^3}{3}\right]_{-1}^{1} = \frac13-\left(-\frac13\right) = \frac23$$

**Answer: $\dfrac23$.**

**20.** $\displaystyle\int_0^{\pi} \sin^3x\,dx$

Using the antiderivative from Problem 1: $-\cos x+\dfrac{\cos^3x}{3}$.

$$\left[-\cos x+\frac{\cos^3x}{3}\right]_0^{\pi} = \left(-\cos\pi+\frac{\cos^3\pi}{3}\right) - \left(-\cos0+\frac{\cos^30}{3}\right)$$

$$= \left(1+\frac{-1}{3}\right) - \left(-1+\frac13\right) = \frac23 - \left(-\frac23\right) = \frac43$$

**Answer: $\dfrac43$.**

**21.** Average value $\dfrac1\pi\displaystyle\int_0^{\pi} \sin^2x\cos^2x\,dx$

Using the antiderivative from Problem 15: $\dfrac{x}{8}-\dfrac{\sin(4x)}{32}$.

$$\int_0^\pi \sin^2x\cos^2x\,dx = \left[\frac{x}{8}-\frac{\sin(4x)}{32}\right]_0^\pi = \left(\frac{\pi}{8}-\frac{\sin(4\pi)}{32}\right) - 0 = \frac{\pi}{8}$$

Average value:

$$\frac1\pi\cdot\frac{\pi}{8} = \frac18$$

**Answer: $\dfrac18$.**
