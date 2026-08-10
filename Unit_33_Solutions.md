# Unit 33: Exponential Change and Separable Differential Equations — Full Solutions

### 🟢 Warm-up

**1.** $\dfrac{dy}{dx}=x$

$$dy = x\,dx \quad\Rightarrow\quad \int dy = \int x\,dx \quad\Rightarrow\quad y = \frac{x^2}{2}+C$$

**2.** $\dfrac{dy}{dx}=2y$

Separate: $\dfrac{dy}{y}=2\,dx$.

$$\int \frac{dy}{y} = \int 2\,dx \quad\Rightarrow\quad \ln|y| = 2x+C \quad\Rightarrow\quad y = Ae^{2x}$$

(where $A=e^C$ is just a renamed arbitrary constant).

**3.** $\dfrac{dy}{dx}=\dfrac{x}{y}$

Separate: $y\,dy = x\,dx$.

$$\int y\,dy = \int x\,dx \quad\Rightarrow\quad \frac{y^2}{2} = \frac{x^2}{2}+C \quad\Rightarrow\quad y^2 - x^2 = K$$

(renaming $2C$ as $K$).

**4.** $\dfrac{dy}{dx}=3x^2$, $y(0)=5$.

$$y = \int 3x^2\,dx = x^3+C$$

Apply $y(0)=5$: $0+C=5 \Rightarrow C=5$.

**$y = x^3+5$.**

**5.** $\dfrac{dy}{dx}=\dfrac{y}{x}$ ($x>0$)

Separate: $\dfrac{dy}{y}=\dfrac{dx}{x}$.

$$\ln|y| = \ln|x|+C \quad\Rightarrow\quad y = e^{\ln|x|+C} = A\cdot x$$

(since $x>0$, $|x|=x$).

**6.** $\dfrac{dy}{dx}=-2y$, $y(0)=10$.

Separate: $\dfrac{dy}{y}=-2\,dx$.

$$\ln|y| = -2x+C \quad\Rightarrow\quad y = Ae^{-2x}$$

Apply $y(0)=10$: $A=10$.

**$y = 10e^{-2x}$.**

---

### 🟡 Standard

**7.** $\dfrac{dy}{dx}=xe^{-y}$

Separate: $e^y\,dy = x\,dx$.

$$\int e^y\,dy = \int x\,dx \quad\Rightarrow\quad e^y = \frac{x^2}{2}+C$$

Solve for $y$:

$$y = \ln\left(\frac{x^2}{2}+C\right)$$

**8.** $\dfrac{dy}{dx}=\dfrac{\cos x}{y}$

Separate: $y\,dy=\cos x\,dx$.

$$\int y\,dy = \int \cos x\,dx \quad\Rightarrow\quad \frac{y^2}{2} = \sin x+C \quad\Rightarrow\quad y^2 = 2\sin x+K$$

$$y = \pm\sqrt{2\sin x+K}$$

**9.** $\dfrac{dy}{dx}=y\cos x$

Separate: $\dfrac{dy}{y}=\cos x\,dx$.

$$\ln|y| = \sin x+C \quad\Rightarrow\quad y = Ae^{\sin x}$$

**10.** $\dfrac{dy}{dx}=x^2y$, $y(0)=2$.

Separate: $\dfrac{dy}{y}=x^2\,dx$.

$$\ln|y| = \frac{x^3}{3}+C \quad\Rightarrow\quad y = Ae^{x^3/3}$$

Apply $y(0)=2$: $A=2$.

**$y = 2e^{x^3/3}$.**

**11.** $\dfrac{dy}{dx}=2xy^2$

Separate: $\dfrac{dy}{y^2}=2x\,dx$.

$$\int y^{-2}\,dy = \int 2x\,dx \quad\Rightarrow\quad -y^{-1} = x^2+C$$

Solve for $y$:

$$y = \frac{-1}{x^2+C}$$

**12.** $\dfrac{dy}{dx}=e^{x+y}$

Rewrite: $e^{x+y}=e^x\cdot e^y$. Separate: $\dfrac{dy}{e^y}=e^x\,dx \Rightarrow e^{-y}\,dy = e^x\,dx$.

$$\int e^{-y}\,dy = \int e^x\,dx \quad\Rightarrow\quad -e^{-y} = e^x+C$$

Solve for $y$: $e^{-y}=-e^x-C$. Renaming the constant so the right side reads more cleanly ($K=-C$):

$$e^{-y} = K-e^x \quad\Rightarrow\quad -y = \ln(K-e^x) \quad\Rightarrow\quad y = -\ln(K-e^x)$$

---

### 🔴 Challenge

**13.** $\dfrac{dy}{dx}=\sin x\cdot e^{-y}$

Separate: $e^y\,dy = \sin x\,dx$.

$$\int e^y\,dy = \int \sin x\,dx \quad\Rightarrow\quad e^y = -\cos x+C$$

Solve for $y$ (renaming the constant for a cleaner form):

$$y = \ln(C-\cos x)$$

**14.** Deriving the Law of Exponential Change from $\dfrac{dy}{dt}=ky$.

Separate: $\dfrac{dy}{y}=k\,dt$.

$$\int \frac{dy}{y} = \int k\,dt \quad\Rightarrow\quad \ln|y| = kt+C$$

Exponentiate both sides:

$$y = e^{kt+C} = e^C\cdot e^{kt}$$

Let $C_1=e^C$ (a renamed positive constant):

$$y = C_1e^{kt}$$

**Relating $C_1$ to $y_0$:** plug in $t=0$:

$$y(0) = C_1e^{k(0)} = C_1\cdot1 = C_1$$

So $C_1$ is exactly $y(0)$, the initial value — which we usually call $y_0$. This confirms:

$$y = y_0e^{kt}$$

**15.** $\dfrac{dy}{dx}=y^2\sin x$, $y(0)=1$.

Separate: $\dfrac{dy}{y^2}=\sin x\,dx$.

$$\int y^{-2}\,dy = \int \sin x\,dx \quad\Rightarrow\quad -y^{-1} = -\cos x+C$$

Multiply both sides by $-1$: $y^{-1} = \cos x - C$. Rename the constant ($-C \to C$ again, standard practice):

$$\frac1y = \cos x - C \quad\Rightarrow\quad y = \frac{1}{\cos x - C}$$

Apply $y(0)=1$: $1 = \dfrac{1}{\cos(0)-C} = \dfrac{1}{1-C}$, so $1-C=1 \Rightarrow C=0$.

$$y = \frac{1}{\cos x} = \sec x$$

**$y=\sec x$.**

**16.** $\dfrac{dy}{dx}=\dfrac{x+1}{y-2}$, $y(0)=4$.

Separate: $(y-2)\,dy = (x+1)\,dx$.

$$\int (y-2)\,dy = \int (x+1)\,dx \quad\Rightarrow\quad \frac{y^2}{2}-2y = \frac{x^2}{2}+x+C$$

Apply $y(0)=4$: $\dfrac{16}{2}-2(4) = 0+0+C \Rightarrow 8-8=C \Rightarrow C=0$.

$$\frac{y^2}{2}-2y = \frac{x^2}{2}+x$$

Multiply by $2$: $y^2-4y = x^2+2x$. Solve for $y$ using the quadratic formula (treating this as $y^2-4y-(x^2+2x)=0$):

$$y = \frac{4\pm\sqrt{16+4(x^2+2x)}}{2} = 2\pm\sqrt{4+x^2+2x} = 2\pm\sqrt{x^2+2x+4}$$

Check which sign matches $y(0)=4$: $2\pm\sqrt{0+0+4} = 2\pm2$. We need $4$, so we take the $+$ sign.

**$y = 2+\sqrt{x^2+2x+4}$.**

**17.** $\dfrac{dy}{dx}=-xy$, $y(0)=3$.

Separate: $\dfrac{dy}{y}=-x\,dx$.

$$\ln|y| = -\frac{x^2}{2}+C \quad\Rightarrow\quad y = Ae^{-x^2/2}$$

Apply $y(0)=3$: $A=3$.

**$y = 3e^{-x^2/2}$.**

---

### 🌍 Applied

**18.** $\dfrac{dP}{dt}=0.04P$, $P(0)=1000$.

By the Law of Exponential Change:

$$P(t) = 1000e^{0.04t}$$

At $t=20$:

$$P(20) = 1000e^{0.8} \approx 1000(2.2255) \approx 2225.5$$

**Answer: $P(t)=1000e^{0.04t}$, and after $20$ years, the population is $\approx2226$.**

**19.** $\dfrac{dT}{dt}=-0.1(T-70)$, $T(0)=200$.

Using the Newton's Law of Cooling shortcut, with $T_s=70$ and $T_0-T_s=200-70=130$:

$$T(t) = 70+130e^{-0.1t}$$

At $t=10$:

$$T(10) = 70+130e^{-1} \approx 70+130(0.3679) \approx 70+47.83 \approx 117.83$$

**Answer: $T(t)=70+130e^{-0.1t}$, and after $10$ minutes, the temperature is $\approx117.8°$.**

**20.** $\dfrac{dA}{dt}=-0.05A$, $A(0)=200$.

$$A(t) = 200e^{-0.05t}$$

Find $t$ when $A=100$:

$$100 = 200e^{-0.05t} \quad\Rightarrow\quad 0.5 = e^{-0.05t} \quad\Rightarrow\quad \ln(0.5) = -0.05t$$

$$t = \frac{\ln(0.5)}{-0.05} = \frac{-0.6931}{-0.05} \approx 13.86$$

**Answer: $A(t)=200e^{-0.05t}$, and it takes $\approx13.86$ time units to decay to $100$ grams.**

**21.** $\dfrac{dC}{dt}=-0.3C$, $C(0)=80$.

$$C(t) = 80e^{-0.3t}$$

At $t=5$:

$$C(5) = 80e^{-1.5} \approx 80(0.22313) \approx 17.85$$

**Answer: $C(t)=80e^{-0.3t}$, and after $5$ hours, the concentration is $\approx17.85$ mg.**
