# Unit 28: Indefinite Integrals and the Substitution Method — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int (x^2+1)^3(2x)\,dx$

Let $u=x^2+1$, so $du=2x\,dx$ — this matches exactly what's left over.

$$\int u^3\,du = \frac{u^4}{4}+C = \frac{(x^2+1)^4}{4}+C$$

**2.** $\displaystyle\int (3x+1)^4\,dx$

Let $u=3x+1$, so $du=3\,dx \Rightarrow dx=\dfrac{du}{3}$.

$$\int u^4\cdot\frac{du}{3} = \frac13\cdot\frac{u^5}{5}+C = \frac{u^5}{15}+C = \frac{(3x+1)^5}{15}+C$$

**3.** $\displaystyle\int 2x\sqrt{x^2+4}\,dx$

Let $u=x^2+4$, so $du=2x\,dx$.

$$\int \sqrt{u}\,du = \int u^{1/2}\,du = \frac23u^{3/2}+C = \frac23(x^2+4)^{3/2}+C$$

**4.** $\displaystyle\int (x^3+2)^2(3x^2)\,dx$

Let $u=x^3+2$, so $du=3x^2\,dx$.

$$\int u^2\,du = \frac{u^3}{3}+C = \frac{(x^3+2)^3}{3}+C$$

**5.** $\displaystyle\int (2x-5)^6\,dx$

Let $u=2x-5$, so $du=2\,dx \Rightarrow dx=\dfrac{du}{2}$.

$$\int u^6\cdot\frac{du}{2} = \frac12\cdot\frac{u^7}{7}+C = \frac{u^7}{14}+C = \frac{(2x-5)^7}{14}+C$$

**6.** $\displaystyle\int x(x^2+3)^5\,dx$

Let $u=x^2+3$, so $du=2x\,dx \Rightarrow x\,dx = \dfrac{du}{2}$.

$$\int u^5\cdot\frac{du}{2} = \frac12\cdot\frac{u^6}{6}+C = \frac{u^6}{12}+C = \frac{(x^2+3)^6}{12}+C$$

**7.** $\displaystyle\int \sin(3x)\,dx$

Let $u=3x$, so $du=3\,dx \Rightarrow dx=\dfrac{du}{3}$.

$$\int \sin u\cdot\frac{du}{3} = \frac13(-\cos u)+C = -\frac13\cos(3x)+C$$

---

### 🟡 Standard

**8.** $\displaystyle\int \frac{4x}{\sqrt{2x^2+1}}\,dx$

Let $u=2x^2+1$, so $du=4x\,dx$ — matches the numerator exactly.

$$\int \frac{1}{\sqrt{u}}\,du = \int u^{-1/2}\,du = 2u^{1/2}+C = 2\sqrt{2x^2+1}+C$$

**9.** $\displaystyle\int x^2(x^3+1)^4\,dx$

Let $u=x^3+1$, so $du=3x^2\,dx \Rightarrow x^2\,dx=\dfrac{du}{3}$.

$$\int u^4\cdot\frac{du}{3} = \frac13\cdot\frac{u^5}{5}+C = \frac{u^5}{15}+C = \frac{(x^3+1)^5}{15}+C$$

**10.** $\displaystyle\int \cos(2x+1)\,dx$

Let $u=2x+1$, so $du=2\,dx \Rightarrow dx=\dfrac{du}{2}$.

$$\int \cos u\cdot\frac{du}{2} = \frac12\sin u+C = \frac12\sin(2x+1)+C$$

**11.** $\displaystyle\int \frac{2x}{(x^2+1)^2}\,dx$

Let $u=x^2+1$, so $du=2x\,dx$.

$$\int u^{-2}\,du = \frac{u^{-1}}{-1}+C = -\frac1u+C = -\frac{1}{x^2+1}+C$$

**12.** $\displaystyle\int \sec^2x\tan x\,dx$

Let $u=\tan x$, so $du=\sec^2x\,dx$.

$$\int u\,du = \frac{u^2}{2}+C = \frac{\tan^2x}{2}+C$$

**13.** $\displaystyle\int (2x+3)(x^2+3x+1)^2\,dx$

Let $u=x^2+3x+1$, so $du=(2x+3)\,dx$ — matches exactly.

$$\int u^2\,du = \frac{u^3}{3}+C = \frac{(x^2+3x+1)^3}{3}+C$$

**14.** $\displaystyle\int 3x^2\sin(x^3)\,dx$

Let $u=x^3$, so $du=3x^2\,dx$.

$$\int \sin u\,du = -\cos u+C = -\cos(x^3)+C$$

---

### 🔴 Challenge

**15.** $\displaystyle\int x\sqrt{x+1}\,dx$

Let $u=x+1$, so $du=dx$. This also means $x=u-1$ — we need this to replace the lone $x$ still sitting in the integral.

$$\int (u-1)\sqrt{u}\,du = \int (u-1)u^{1/2}\,du = \int \big(u^{3/2}-u^{1/2}\big)\,du$$

$$= \frac25u^{5/2} - \frac23u^{3/2} + C$$

Substitute back $u=x+1$:

$$= \frac25(x+1)^{5/2} - \frac23(x+1)^{3/2} + C$$

**16.** $\displaystyle\int_0^1 2x(x^2+1)^3\,dx$

Let $u=x^2+1$, so $du=2x\,dx$. Change the bounds: when $x=0$, $u=1$; when $x=1$, $u=2$.

$$\int_1^2 u^3\,du = \left[\frac{u^4}{4}\right]_1^2 = \frac{16}{4}-\frac14 = 4-0.25 = 3.75 = \frac{15}{4}$$

**Answer: $\dfrac{15}{4}$.**

**17.** $\displaystyle\int_0^2 \frac{x}{\sqrt{x^2+9}}\,dx$

Let $u=x^2+9$, so $du=2x\,dx \Rightarrow x\,dx=\dfrac{du}{2}$. Change the bounds: when $x=0$, $u=9$; when $x=2$, $u=13$.

$$\int_9^{13} \frac{1}{\sqrt{u}}\cdot\frac{du}{2} = \frac12\int_9^{13} u^{-1/2}\,du = \frac12\Big[2\sqrt{u}\Big]_9^{13} = \Big[\sqrt{u}\Big]_9^{13} = \sqrt{13}-\sqrt9 = \sqrt{13}-3$$

**Answer: $\sqrt{13}-3 \approx 0.606$.**

**18.** $\displaystyle\int \sin^3x\cos x\,dx$

Let $u=\sin x$, so $du=\cos x\,dx$.

$$\int u^3\,du = \frac{u^4}{4}+C = \frac{\sin^4x}{4}+C$$

**19.** $\displaystyle\int x^3\sqrt{x^4+5}\,dx$

Let $u=x^4+5$, so $du=4x^3\,dx \Rightarrow x^3\,dx=\dfrac{du}{4}$.

$$\int \sqrt{u}\cdot\frac{du}{4} = \frac14\cdot\frac23u^{3/2}+C = \frac16u^{3/2}+C = \frac16(x^4+5)^{3/2}+C$$

---

### 🌍 Applied

**20.** $\dfrac{dP}{dt} = \dfrac{100t}{\sqrt{t^2+9}}$

Let $u=t^2+9$, so $du=2t\,dt \Rightarrow t\,dt=\dfrac{du}{2}$.

$$P(t) = \int \frac{100t}{\sqrt{t^2+9}}\,dt = 100\int \frac{1}{\sqrt{u}}\cdot\frac{du}{2} = 50\int u^{-1/2}\,du = 50(2u^{1/2})+C = 100\sqrt{u}+C$$

**Answer: $P(t) = 100\sqrt{t^2+9}+C$.**

**21.** $MR(x)=6x^2(x^3+10)^2$

Let $u=x^3+10$, so $du=3x^2\,dx \Rightarrow x^2\,dx=\dfrac{du}{3}$.

$$R(x) = \int 6x^2(x^3+10)^2\,dx = 6\int u^2\cdot\frac{du}{3} = 2\int u^2\,du = 2\cdot\frac{u^3}{3}+C = \frac23u^3+C$$

**Answer: $R(x) = \dfrac23(x^3+10)^3+C$.**

**22.** $\displaystyle\int_0^2 \frac{8t}{(t^2+1)^2}\,dt$

Let $u=t^2+1$, so $du=2t\,dt \Rightarrow t\,dt=\dfrac{du}{2}$. Change the bounds: when $t=0$, $u=1$; when $t=2$, $u=5$.

$$8\int_1^5 \frac{1}{u^2}\cdot\frac{du}{2} = 4\int_1^5 u^{-2}\,du = 4\Big[-u^{-1}\Big]_1^5 = 4\left(-\frac15-(-1)\right) = 4\left(\frac45\right) = \frac{16}{5}$$

**Answer: total water collected $=\dfrac{16}{5}=3.2$ gallons.**

**23.** $\displaystyle\int_0^{\sqrt{\pi}} t\sin(t^2)\,dt$

Let $u=t^2$, so $du=2t\,dt \Rightarrow t\,dt=\dfrac{du}{2}$. Change the bounds: when $t=0$, $u=0$; when $t=\sqrt\pi$, $u=\pi$.

$$\int_0^{\pi} \sin u\cdot\frac{du}{2} = \frac12\Big[-\cos u\Big]_0^{\pi} = \frac12\big[(-\cos\pi)-(-\cos0)\big] = \frac12\big[1-(-1)\big] = \frac12(2)=1$$

**Answer: exact distance traveled $=1$ meter.**
