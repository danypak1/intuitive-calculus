# Unit 32: Exponential Functions — Full Solutions

### 🟢 Warm-up

**1.** $\dfrac{d}{dx}[e^x] = e^x$

**2.** $\dfrac{d}{dx}[e^{2x}]$

Chain rule: $u=2x$, $u'=2$.

$$\frac{d}{dx}[e^{2x}] = 2e^{2x}$$

**3.** $\dfrac{d}{dx}[3e^x] = 3e^x$

**4.** Solve $e^x=5$.

$$x = \ln5$$

**5.** $\displaystyle\int e^x\,dx = e^x+C$

**6.** $\dfrac{d}{dx}[e^x+x^2] = e^x+2x$

---

### 🟡 Standard

**7.** $\dfrac{d}{dx}[e^{x^2}]$

Chain rule: $u=x^2$, $u'=2x$.

$$\frac{d}{dx}[e^{x^2}] = 2xe^{x^2}$$

**8.** $\dfrac{d}{dx}[e^{3x+1}]$

Chain rule: $u=3x+1$, $u'=3$.

$$\frac{d}{dx}[e^{3x+1}] = 3e^{3x+1}$$

**9.** $\dfrac{d}{dx}[xe^x]$

Product rule: $f=x$ ($f'=1$), $g=e^x$ ($g'=e^x$).

$$\frac{d}{dx}[xe^x] = 1\cdot e^x + x\cdot e^x = e^x(1+x)$$

**10.** $\dfrac{d}{dx}\left[\dfrac{e^x}{x}\right]$

Quotient rule: $f=e^x$ ($f'=e^x$), $g=x$ ($g'=1$).

$$\frac{d}{dx}\left[\frac{e^x}{x}\right] = \frac{e^x\cdot x - e^x\cdot 1}{x^2} = \frac{e^x(x-1)}{x^2}$$

**11.** Solve $e^{2x-1}=7$.

$$2x-1 = \ln7$$

$$2x = \ln7+1$$

$$x = \frac{\ln7+1}{2}$$

**12.** $\displaystyle\int 3e^{2x}\,dx$

Let $u=2x$, $du=2\,dx \Rightarrow dx=\dfrac{du}{2}$.

$$3\int e^u\cdot\frac{du}{2} = \frac32e^u+C = \frac32e^{2x}+C$$

**13.** $\displaystyle\int_0^1 e^x\,dx$

$$\Big[e^x\Big]_0^1 = e^1-e^0 = e-1$$

**Answer: $e-1$.**

---

### 🔴 Challenge

**14.** Solve $e^{3x-6}=9$.

$$3x-6 = \ln9$$

$$3x = \ln9+6$$

$$x = \frac{\ln9+6}{3}$$

(Since $9=3^2$, this can also be written as $x=\dfrac{2\ln3+6}{3} = \dfrac{2\ln3}{3}+2$.)

**15.** $y=(9x^2-6x+2)e^{3x}$. Find $\dfrac{dy}{dx}$.

Product rule: $f=9x^2-6x+2$ ($f'=18x-6$), $g=e^{3x}$ ($g'=3e^{3x}$).

$$\frac{dy}{dx} = (18x-6)e^{3x} + (9x^2-6x+2)(3e^{3x})$$

Factor out $e^{3x}$:

$$= e^{3x}\Big[(18x-6) + 3(9x^2-6x+2)\Big] = e^{3x}\big[18x-6+27x^2-18x+6\big]$$

Notice the $18x$ and $-18x$ cancel, and $-6+6=0$:

$$= e^{3x}(27x^2) = 27x^2e^{3x}$$

**$\dfrac{dy}{dx} = 27x^2e^{3x}$.**

**16.** $\dfrac{d}{dx}[e^{\sin x}]$

Chain rule: $u=\sin x$, $u'=\cos x$.

$$\frac{d}{dx}[e^{\sin x}] = e^{\sin x}\cdot\cos x$$

**17.** $\displaystyle\int 2xe^{x^2}\,dx$

Let $u=x^2$, $du=2x\,dx$.

$$\int e^u\,du = e^u+C = e^{x^2}+C$$

**18.** Solve $2e^{x}-3=7$.

Isolate the exponential term first:

$$2e^x = 10$$

$$e^x = 5$$

$$x = \ln5$$

---

### 🌍 Applied

**19.** $A(t)=1000e^{0.06t}=2000$ (doubled).

$$e^{0.06t} = 2$$

$$0.06t = \ln2$$

$$t = \frac{\ln2}{0.06} \approx \frac{0.6931}{0.06} \approx 11.55 \text{ years}$$

**20.** $P(t)=200e^{0.03t}$

$$\frac{dP}{dt} = 200(0.03)e^{0.03t} = 6e^{0.03t}$$

At $t=10$:

$$\frac{dP}{dt}\bigg|_{t=10} = 6e^{0.3} \approx 6(1.3499) \approx 8.10$$

**Answer: $\dfrac{dP}{dt}=6e^{0.03t}$, and at $t=10$, the growth rate is $\approx8.10$ people per year.**

**21.** $C(t)=50e^{-0.5t}$

$$\frac{dC}{dt} = 50(-0.5)e^{-0.5t} = -25e^{-0.5t}$$

At $t=2$:

$$\frac{dC}{dt}\bigg|_{t=2} = -25e^{-1} \approx -25(0.3679) \approx -9.20$$

**Answer: $\dfrac{dC}{dt}=-25e^{-0.5t}$, and at $t=2$, the concentration is decreasing at a rate of approximately $9.20$ mg per unit time.**

**22.** $D(t)=80e^{-0.1t}$, from $t=0$ to $t=10$.

Let $u=-0.1t$, $du=-0.1\,dt \Rightarrow dt = -10\,du$.

$$\int 80e^{-0.1t}\,dt = 80\int e^u(-10)\,du = -800\int e^u\,du = -800e^u+C = -800e^{-0.1t}+C$$

Evaluate from $0$ to $10$:

$$\Big[-800e^{-0.1t}\Big]_0^{10} = \big(-800e^{-1}\big) - \big(-800e^0\big) = -800e^{-1}+800 = 800\big(1-e^{-1}\big)$$

$$\approx 800(1-0.3679) \approx 800(0.6321) \approx 505.7$$

**Answer: total accumulated area $= 800(1-e^{-1}) \approx 505.7$.**
