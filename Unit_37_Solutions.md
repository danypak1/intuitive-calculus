# Unit 37: Integration by Parts — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int x\cos x\,dx$

Let $u=x$ ($du=dx$), $dv=\cos x\,dx$ ($v=\sin x$).

$$\int x\cos x\,dx = x\sin x - \int \sin x\,dx = x\sin x - (-\cos x) = x\sin x + \cos x + C$$

**2.** $\displaystyle\int xe^{2x}\,dx$

Let $u=x$ ($du=dx$), $dv=e^{2x}\,dx$ ($v=\frac12e^{2x}$).

$$\int xe^{2x}\,dx = \frac{x}{2}e^{2x} - \int \frac12e^{2x}\,dx = \frac{x}{2}e^{2x} - \frac14e^{2x}+C$$

**3.** $\displaystyle\int x\sin(2x)\,dx$

Let $u=x$ ($du=dx$), $dv=\sin(2x)\,dx$ ($v=-\frac12\cos(2x)$).

$$\int x\sin(2x)\,dx = -\frac{x}{2}\cos(2x) - \int\left(-\frac12\cos(2x)\right)dx = -\frac{x}{2}\cos(2x) + \frac12\int\cos(2x)\,dx$$

$$= -\frac{x}{2}\cos(2x) + \frac14\sin(2x) + C$$

**4.** $\displaystyle\int \ln x\,dx$

Let $u=\ln x$ ($du=\frac1x\,dx$), $dv=dx$ ($v=x$).

$$\int \ln x\,dx = x\ln x - \int x\cdot\frac1x\,dx = x\ln x - \int 1\,dx = x\ln x - x + C$$

**5.** $\displaystyle\int (x+1)e^x\,dx$

Let $u=x+1$ ($du=dx$), $dv=e^x\,dx$ ($v=e^x$).

$$\int (x+1)e^x\,dx = (x+1)e^x - \int e^x\,dx = (x+1)e^x - e^x + C = xe^x + e^x - e^x + C = xe^x+C$$

**6.** $\displaystyle\int xe^{-x}\,dx$

Let $u=x$ ($du=dx$), $dv=e^{-x}\,dx$ ($v=-e^{-x}$).

$$\int xe^{-x}\,dx = -xe^{-x} - \int(-e^{-x})\,dx = -xe^{-x} + \int e^{-x}\,dx = -xe^{-x} - e^{-x} + C = -e^{-x}(x+1)+C$$

---

### 🟡 Standard

**7.** $\displaystyle\int x\sin x\,dx$

Let $u=x$ ($du=dx$), $dv=\sin x\,dx$ ($v=-\cos x$).

$$\int x\sin x\,dx = -x\cos x - \int(-\cos x)\,dx = -x\cos x + \int \cos x\,dx = -x\cos x + \sin x + C$$

**8.** $\displaystyle\int x^5\ln x\,dx$

Let $u=\ln x$ ($du=\frac1x\,dx$), $dv=x^5\,dx$ ($v=\frac{x^6}{6}$).

$$\int x^5\ln x\,dx = \frac{x^6}{6}\ln x - \int \frac{x^6}{6}\cdot\frac1x\,dx = \frac{x^6}{6}\ln x - \frac16\int x^5\,dx$$

$$= \frac{x^6}{6}\ln x - \frac16\cdot\frac{x^6}{6} + C = \frac{x^6}{6}\ln x - \frac{x^6}{36}+C$$

**9.** $\displaystyle\int x^2e^x\,dx$

**Round 1:** $u=x^2$ ($du=2x\,dx$), $dv=e^x\,dx$ ($v=e^x$).

$$\int x^2e^x\,dx = x^2e^x - \int 2xe^x\,dx = x^2e^x - 2\int xe^x\,dx$$

**Round 2:** we need $\displaystyle\int xe^x\,dx$. Let $u=x$ ($du=dx$), $dv=e^x\,dx$ ($v=e^x$).

$$\int xe^x\,dx = xe^x - \int e^x\,dx = xe^x-e^x+C$$

**Combine:**

$$\int x^2e^x\,dx = x^2e^x - 2(xe^x-e^x) + C = x^2e^x-2xe^x+2e^x+C = e^x(x^2-2x+2)+C$$

**10.** $\displaystyle\int \ln(x^2)\,dx$

Simplify first: $\ln(x^2)=2\ln x$.

$$\int 2\ln x\,dx = 2\int \ln x\,dx = 2(x\ln x - x)+C = 2x\ln x - 2x + C$$

**11.** $\displaystyle\int x\cos(3x)\,dx$

Let $u=x$ ($du=dx$), $dv=\cos(3x)\,dx$ ($v=\frac13\sin(3x)$).

$$\int x\cos(3x)\,dx = \frac{x}{3}\sin(3x) - \int \frac13\sin(3x)\,dx = \frac{x}{3}\sin(3x) - \frac13\left(-\frac13\cos(3x)\right)+C$$

$$= \frac{x}{3}\sin(3x) + \frac19\cos(3x) + C$$

**12.** $\displaystyle\int \arctan(x)\,dx$

Let $u=\arctan x$ ($du=\frac{1}{1+x^2}\,dx$), $dv=dx$ ($v=x$).

$$\int \arctan(x)\,dx = x\arctan x - \int \frac{x}{1+x^2}\,dx$$

For the remaining integral, let $w=1+x^2$, $dw=2x\,dx$:

$$\int \frac{x}{1+x^2}\,dx = \frac12\int \frac{dw}{w} = \frac12\ln(1+x^2)$$

**Combine:**

$$\int \arctan(x)\,dx = x\arctan x - \frac12\ln(1+x^2) + C$$

**13.** $\displaystyle\int x^3\ln x\,dx$

Let $u=\ln x$ ($du=\frac1x\,dx$), $dv=x^3\,dx$ ($v=\frac{x^4}{4}$).

$$\int x^3\ln x\,dx = \frac{x^4}{4}\ln x - \int \frac{x^4}{4}\cdot\frac1x\,dx = \frac{x^4}{4}\ln x - \frac14\int x^3\,dx$$

$$= \frac{x^4}{4}\ln x - \frac14\cdot\frac{x^4}{4} + C = \frac{x^4}{4}\ln x - \frac{x^4}{16}+C$$

---

### 🔴 Challenge

**14.** $\displaystyle\int xe^x\,dx$

Let $u=x$ ($du=dx$), $dv=e^x\,dx$ ($v=e^x$).

$$\int xe^x\,dx = xe^x - \int e^x\,dx = xe^x - e^x + C$$

**15.** $\displaystyle\int e^x\cos x\,dx$

Let $I = \displaystyle\int e^x\cos x\,dx$.

**Round 1:** $u=e^x$ ($du=e^x\,dx$), $dv=\cos x\,dx$ ($v=\sin x$).

$$I = e^x\sin x - \int e^x\sin x\,dx$$

**Round 2:** for $\displaystyle\int e^x\sin x\,dx$, let $u=e^x$ ($du=e^x\,dx$), $dv=\sin x\,dx$ ($v=-\cos x$).

$$\int e^x\sin x\,dx = -e^x\cos x - \int(-\cos x)(e^x\,dx) = -e^x\cos x + \int e^x\cos x\,dx = -e^x\cos x + I$$

**Substitute back into the Round 1 result:**

$$I = e^x\sin x - \big(-e^x\cos x + I\big) = e^x\sin x + e^x\cos x - I$$

**Solve for $I$ algebraically:**

$$I + I = e^x\sin x + e^x\cos x$$

$$2I = e^x(\sin x + \cos x)$$

$$I = \frac{e^x(\sin x+\cos x)}{2} + C$$

**16.** $\displaystyle\int e^{2x}\sin x\,dx$

Let $I = \displaystyle\int e^{2x}\sin x\,dx$.

**Round 1:** $u=e^{2x}$ ($du=2e^{2x}\,dx$), $dv=\sin x\,dx$ ($v=-\cos x$).

$$I = -e^{2x}\cos x + \int 2e^{2x}\cos x\,dx = -e^{2x}\cos x + 2\int e^{2x}\cos x\,dx$$

**Round 2:** let $J=\displaystyle\int e^{2x}\cos x\,dx$. Using $u=e^{2x}$ ($du=2e^{2x}\,dx$), $dv=\cos x\,dx$ ($v=\sin x$):

$$J = e^{2x}\sin x - \int 2e^{2x}\sin x\,dx = e^{2x}\sin x - 2I$$

**Substitute back:**

$$I = -e^{2x}\cos x + 2\big(e^{2x}\sin x - 2I\big) = -e^{2x}\cos x + 2e^{2x}\sin x - 4I$$

**Solve for $I$:**

$$I + 4I = -e^{2x}\cos x + 2e^{2x}\sin x$$

$$5I = e^{2x}(2\sin x - \cos x)$$

$$I = \frac{e^{2x}(2\sin x-\cos x)}{5} + C$$

**17.** $\displaystyle\int x^2\sin x\,dx$

**Round 1:** $u=x^2$ ($du=2x\,dx$), $dv=\sin x\,dx$ ($v=-\cos x$).

$$\int x^2\sin x\,dx = -x^2\cos x - \int(-\cos x)(2x\,dx) = -x^2\cos x + 2\int x\cos x\,dx$$

**Round 2:** from Problem 1, $\displaystyle\int x\cos x\,dx = x\sin x+\cos x+C$.

**Combine:**

$$\int x^2\sin x\,dx = -x^2\cos x + 2(x\sin x+\cos x) + C = -x^2\cos x + 2x\sin x + 2\cos x + C$$

**18.** $\displaystyle\int x(\ln x)^2\,dx$

**Round 1:** let $u=(\ln x)^2$ ($du = 2\ln x\cdot\frac1x\,dx$), $dv=x\,dx$ ($v=\frac{x^2}{2}$).

$$\int x(\ln x)^2\,dx = \frac{x^2}{2}(\ln x)^2 - \int \frac{x^2}{2}\cdot\frac{2\ln x}{x}\,dx = \frac{x^2}{2}(\ln x)^2 - \int x\ln x\,dx$$

**Round 2:** for $\displaystyle\int x\ln x\,dx$, let $u=\ln x$ ($du=\frac1x\,dx$), $dv=x\,dx$ ($v=\frac{x^2}{2}$).

$$\int x\ln x\,dx = \frac{x^2}{2}\ln x - \int \frac{x^2}{2}\cdot\frac1x\,dx = \frac{x^2}{2}\ln x - \frac12\int x\,dx = \frac{x^2}{2}\ln x - \frac{x^2}{4}$$

**Combine:**

$$\int x(\ln x)^2\,dx = \frac{x^2}{2}(\ln x)^2 - \left(\frac{x^2}{2}\ln x - \frac{x^2}{4}\right) + C = \frac{x^2}{2}(\ln x)^2 - \frac{x^2}{2}\ln x + \frac{x^2}{4} + C$$

---

### 🌍 Applied

**19.** $\displaystyle\int_0^\pi x\sin x\,dx$

Using the antiderivative from Problem 7: $-x\cos x+\sin x$.

$$\Big[-x\cos x+\sin x\Big]_0^\pi = \big(-\pi\cos\pi+\sin\pi\big) - \big(0+0\big) = -\pi(-1)+0 = \pi$$

**Answer: total work done $=\pi$ (Newton-meters).**

**20.** $\displaystyle\int_0^{10} te^{-t}\,dt$

Using the antiderivative pattern from Problem 6: $-e^{-t}(t+1)$.

$$\Big[-e^{-t}(t+1)\Big]_0^{10} = -e^{-10}(11) - \big(-e^0(1)\big) = -11e^{-10}+1 = 1-11e^{-10}$$

Since $e^{-10}$ is extremely small ($\approx0.0000454$):

$$\approx 1 - 0.0005 \approx 0.9995$$

**Answer: total present value $= 1-11e^{-10} \approx 0.9995$.**

**21.** $\displaystyle\int_1^e x\ln x\,dx$

Using the antiderivative from Unit's earlier work (Problem 18's Round 2): $\dfrac{x^2}{2}\ln x - \dfrac{x^2}{4}$.

At $x=e$: $\dfrac{e^2}{2}(1) - \dfrac{e^2}{4} = \dfrac{e^2}{2}-\dfrac{e^2}{4} = \dfrac{e^2}{4}$.

At $x=1$: $\dfrac{1}{2}(0) - \dfrac14 = -\dfrac14$.

$$\frac{e^2}{4} - \left(-\frac14\right) = \frac{e^2+1}{4}$$

**Answer: $\dfrac{e^2+1}{4} \approx 2.097$.**

**22.** $\displaystyle\int_0^{\pi/2} x\cos x\,dx$

Using the antiderivative from Problem 1: $x\sin x+\cos x$.

$$\left[x\sin x+\cos x\right]_0^{\pi/2} = \left(\frac{\pi}{2}\cdot1+0\right) - (0+1) = \frac{\pi}{2}-1$$

**Answer: $\dfrac{\pi}{2}-1 \approx 0.571$.**
