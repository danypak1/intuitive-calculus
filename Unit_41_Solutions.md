# Unit 41: Improper Integrals — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int_1^\infty \frac{1}{x^2}\,dx$

$$\lim_{b\to\infty}\int_1^b x^{-2}\,dx = \lim_{b\to\infty}\Big[-x^{-1}\Big]_1^b = \lim_{b\to\infty}\left(-\frac1b+1\right) = 0+1 = 1$$

**Converges to $1$.**

**2.** $\displaystyle\int_1^\infty \frac{1}{x}\,dx$

$$\lim_{b\to\infty}\Big[\ln x\Big]_1^b = \lim_{b\to\infty}(\ln b - 0) = \infty$$

**Diverges.**

**3.** $\displaystyle\int_0^\infty e^{-x}\,dx$

$$\lim_{b\to\infty}\Big[-e^{-x}\Big]_0^b = \lim_{b\to\infty}\big(-e^{-b}+1\big) = 0+1 = 1$$

**Converges to $1$.**

**4.** $\displaystyle\int_{-\infty}^0 e^{x}\,dx$

$$\lim_{a\to-\infty}\Big[e^{x}\Big]_a^0 = \lim_{a\to-\infty}\big(1-e^{a}\big) = 1-0 = 1$$

**Converges to $1$.**

**5.** $\displaystyle\int_1^\infty \frac{1}{x^3}\,dx$

$$\lim_{b\to\infty}\left[-\frac{1}{2x^2}\right]_1^b = \lim_{b\to\infty}\left(-\frac{1}{2b^2}+\frac12\right) = 0+\frac12 = \frac12$$

**Converges to $\dfrac12$.**

**6.** $\displaystyle\int_4^\infty \frac{1}{x^{3/2}}\,dx$

$$\lim_{b\to\infty}\Big[-2x^{-1/2}\Big]_4^b = \lim_{b\to\infty}\left(-\frac{2}{\sqrt b}+\frac{2}{\sqrt4}\right) = 0+1 = 1$$

**Converges to $1$.**

---

### 🟡 Standard

**7.** $\displaystyle\int_0^1 \frac{1}{x}\,dx$

Discontinuity at $x=0$.

$$\lim_{a\to0^+}\Big[\ln x\Big]_a^1 = \lim_{a\to0^+}(0-\ln a) = \infty$$

**Diverges.**

**8.** $\displaystyle\int_0^1 \frac{1}{x^2}\,dx$

$$\lim_{a\to0^+}\Big[-x^{-1}\Big]_a^1 = \lim_{a\to0^+}\left(-1+\frac1a\right) = \infty$$

**Diverges.**

**9.** $\displaystyle\int_0^4 \frac{1}{\sqrt{x}}\,dx$

$$\lim_{a\to0^+}\Big[2x^{1/2}\Big]_a^4 = \lim_{a\to0^+}\big(4-2\sqrt a\big) = 4-0 = 4$$

**Converges to $4$.**

**10.** $\displaystyle\int_{-\infty}^{\infty} \frac{1}{1+x^2}\,dx$

Split at $0$.

$$\int_0^\infty \frac{dx}{1+x^2} = \lim_{b\to\infty}\Big[\arctan x\Big]_0^b = \frac{\pi}{2}-0 = \frac{\pi}{2}$$

$$\int_{-\infty}^0 \frac{dx}{1+x^2} = \lim_{a\to-\infty}\Big[\arctan x\Big]_a^0 = 0-\left(-\frac{\pi}{2}\right) = \frac{\pi}{2}$$

Both converge, so the total:

$$\frac{\pi}{2}+\frac{\pi}{2} = \pi$$

**Converges to $\pi$.**

**11.** $\displaystyle\int_2^\infty \frac{1}{(x-1)^2}\,dx$

No discontinuity on $[2,\infty)$ (since $x-1\ge1>0$ throughout).

$$\lim_{b\to\infty}\left[-\frac{1}{x-1}\right]_2^b = \lim_{b\to\infty}\left(-\frac{1}{b-1}+1\right) = 0+1 = 1$$

**Converges to $1$.**

**12.** $\displaystyle\int_0^3 \frac{1}{3-x}\,dx$

Discontinuity at $x=3$ (upper endpoint). Antiderivative: $-\ln|3-x|$.

$$\lim_{b\to3^-}\Big[-\ln|3-x|\Big]_0^b = \lim_{b\to3^-}\big(-\ln(3-b)+\ln3\big)$$

As $b\to3^-$, $(3-b)\to0^+$, so $\ln(3-b)\to-\infty$, meaning $-\ln(3-b)\to+\infty$.

**Diverges.**

---

### 🔴 Challenge

**13.** $\displaystyle\int_0^\infty \frac{1}{1+x^2}\,dx$

$$\lim_{b\to\infty}\Big[\arctan x\Big]_0^b = \lim_{b\to\infty}\arctan b - 0 = \frac{\pi}{2}$$

**Converges to $\dfrac{\pi}{2}$.**

**14.** $\displaystyle\int_1^\infty \frac{1}{x^{3/2}}\,dx$

$$\lim_{b\to\infty}\Big[-2x^{-1/2}\Big]_1^b = \lim_{b\to\infty}\left(-\frac{2}{\sqrt b}+2\right) = 0+2 = 2$$

**Converges to $2$.**

**15.** $\displaystyle\int_0^1 \frac{1}{\sqrt{x}}\,dx$

$$\lim_{a\to0^+}\Big[2x^{1/2}\Big]_a^1 = \lim_{a\to0^+}\big(2-2\sqrt a\big) = 2-0 = 2$$

**Converges to $2$.**

**16.** $\displaystyle\int_{-1}^{1} \frac{1}{x^{3/4}}\,dx$

**A note on interpretation:** $x^{3/4}$ is not real-valued for negative $x$ under the standard definition. Reading this integral as intended to be evaluated over the full symmetric interval $[-1,1]$, we interpret the integrand as $\dfrac{1}{|x|^{3/4}}$, which is real-valued and even.

Since the integrand is even, and there's a discontinuity at $x=0$:

$$\int_{-1}^1 \frac{dx}{|x|^{3/4}} = 2\int_0^1 x^{-3/4}\,dx$$

$$= 2\lim_{a\to0^+}\Big[4x^{1/4}\Big]_a^1 = 2\lim_{a\to0^+}\big(4-4a^{1/4}\big) = 2(4-0) = 8$$

**Converges to $8$** (under the $|x|^{3/4}$ interpretation).

**17.** $\displaystyle\int_{-2}^2 \frac{1}{x^2}\,dx$

**This interval has a hidden discontinuity at the interior point $x=0$** — easy to miss since $0$ isn't an endpoint! We must split there:

$$\int_0^2 \frac{dx}{x^2} = \lim_{a\to0^+}\int_a^2 x^{-2}\,dx = \lim_{a\to0^+}\left[-x^{-1}\right]_a^2 = \lim_{a\to0^+}\left(-\frac12+\frac1a\right) = \infty$$

Since this piece alone already diverges, **the entire original integral diverges** — there's no need to even check the other half (though by symmetry, it would diverge too).

**Diverges.**

---

### 🌍 Applied

**18.** $D(t)=D_0e^{-kt}$

$$\int_0^\infty D_0e^{-kt}\,dt = \lim_{b\to\infty}\left[-\frac{D_0}{k}e^{-kt}\right]_0^b = \lim_{b\to\infty}\left(-\frac{D_0}{k}e^{-kb}+\frac{D_0}{k}\right) = 0+\frac{D_0}{k} = \frac{D_0}{k}$$

**General formula: $\dfrac{D_0}{k}$.**

With $D_0=100$, $k=0.2$:

$$\frac{100}{0.2} = 500$$

**Answer: total accumulated dose $=500$ mg.**

**19.** $\displaystyle\int_0^\infty 2e^{-2x}\,dx$

$$\lim_{b\to\infty}\Big[-e^{-2x}\Big]_0^b = \lim_{b\to\infty}\big(-e^{-2b}+1\big) = 0+1 = 1$$

**Confirmed: the integral equals exactly $1$**, verifying this is a valid total-probability distribution.

**20.** $\displaystyle\int_0^\infty 500e^{-0.05t}\,dt$

Using the same pattern as Problem 18, with $D_0=500$, $k=0.05$:

$$\frac{500}{0.05} = 10{,}000$$

**Answer: present value $=\$10{,}000$.**

**21.** $\displaystyle\int_0^1 \frac{1}{\sqrt{1-x}}\,dx$

Discontinuity at $x=1$ (upper endpoint). Let $u=1-x$, $du=-dx$:

$$\int \frac{1}{\sqrt{1-x}}\,dx = \int u^{-1/2}(-du) = -2u^{1/2}+C = -2\sqrt{1-x}+C$$

$$\lim_{b\to1^-}\Big[-2\sqrt{1-x}\Big]_0^b = \lim_{b\to1^-}\big(-2\sqrt{1-b}+2\big)$$

As $b\to1^-$, $(1-b)\to0^+$, so $\sqrt{1-b}\to0$:

$$= 0+2 = 2$$

**Answer: total work $=2$ (converges, despite the force growing without bound at $x=1$).**
