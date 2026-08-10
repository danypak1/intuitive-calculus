# Unit 31: Natural Logarithms — Full Solutions

### 🟢 Warm-up

**1.** $\ln(8)$

$8=2^3$, so:

$$\ln(8) = \ln(2^3) = 3\ln 2$$

**2.** $\dfrac{d}{dx}[\ln(5x)]$

Chain rule: $u=5x$, $u'=5$.

$$\frac{d}{dx}[\ln(5x)] = \frac{5}{5x} = \frac1x$$

(Alternatively: $\ln(5x)=\ln5+\ln x$, so its derivative is $0+\dfrac1x=\dfrac1x$ — same answer.)

**3.** $\dfrac{d}{dx}[\ln(x^2+1)]$

Chain rule: $u=x^2+1$, $u'=2x$.

$$\frac{d}{dx}[\ln(x^2+1)] = \frac{2x}{x^2+1}$$

**4.** Solve $\ln(x)=3$.

$$x = e^3$$

**5.** $\displaystyle\int \frac3x\,dx$

$$\int \frac3x\,dx = 3\ln|x|+C$$

**6.** $\ln(x^3y^2)$

$$\ln(x^3y^2) = \ln(x^3)+\ln(y^2) = 3\ln x+2\ln y$$

---

### 🟡 Standard

**7.** Solve $\ln(x-8)=5$.

Exponentiate both sides:

$$x-8 = e^5$$

$$x = e^5+8$$

**8.** $\dfrac{d}{dx}[x\ln x]$

Product rule: $f=x$ ($f'=1$), $g=\ln x$ ($g'=\frac1x$).

$$\frac{d}{dx}[x\ln x] = 1\cdot\ln x + x\cdot\frac1x = \ln x+1$$

**9.** $\dfrac{d}{dx}\left[\dfrac{\ln x}{x}\right]$

Quotient rule: $f=\ln x$ ($f'=\frac1x$), $g=x$ ($g'=1$).

$$\frac{d}{dx}\left[\frac{\ln x}{x}\right] = \frac{\frac1x\cdot x - \ln x\cdot1}{x^2} = \frac{1-\ln x}{x^2}$$

**10.** $\ln\big(x^2\sqrt{x+3}\big)$

Simplify first:

$$\ln\big(x^2\sqrt{x+3}\big) = \ln(x^2) + \ln\big((x+3)^{1/2}\big) = 2\ln x + \frac12\ln(x+3)$$

Differentiate:

$$\frac{d}{dx} = \frac2x + \frac12\cdot\frac{1}{x+3} = \frac2x + \frac{1}{2(x+3)}$$

**11.** $\displaystyle\int \frac{2x}{x^2+1}\,dx$

Let $u=x^2+1$, $du=2x\,dx$.

$$\int \frac1u\,du = \ln|u|+C = \ln(x^2+1)+C$$

(No absolute value needed here since $x^2+1$ is always positive.)

**12.** Solve $\ln(2x+1)=0$.

$$2x+1 = e^0 = 1$$

$$2x=0 \quad\Rightarrow\quad x=0$$

**13.** $\dfrac{d}{dx}[\ln(\sin x)]$

Chain rule: $u=\sin x$, $u'=\cos x$.

$$\frac{d}{dx}[\ln(\sin x)] = \frac{\cos x}{\sin x} = \cot x$$

---

### 🔴 Challenge

**14.** $y = \dfrac{x^5}{4}\ln x - \dfrac{x^4}{4}$

Differentiate the first term using the product rule: $f=\dfrac{x^5}{4}$ ($f'=\dfrac{5x^4}{4}$), $g=\ln x$ ($g'=\dfrac1x$).

$$\frac{d}{dx}\left[\frac{x^5}{4}\ln x\right] = \frac{5x^4}{4}\ln x + \frac{x^5}{4}\cdot\frac1x = \frac{5x^4}{4}\ln x + \frac{x^4}{4}$$

Differentiate the second term: $\dfrac{d}{dx}\left[-\dfrac{x^4}{4}\right] = -x^3$.

Combine:

$$\frac{dy}{dx} = \frac{5x^4}{4}\ln x + \frac{x^4}{4} - x^3$$

**15.** $y = \ln\left(\dfrac{1}{x^2\sqrt{x+1}}\right)$

Simplify first:

$$y = \ln(1) - \ln\big(x^2\sqrt{x+1}\big) = 0 - \left[2\ln x + \frac12\ln(x+1)\right] = -2\ln x - \frac12\ln(x+1)$$

Differentiate:

$$\frac{dy}{dx} = -\frac2x - \frac12\cdot\frac{1}{x+1} = -\frac2x - \frac{1}{2(x+1)}$$

**16.** $y = \ln\big(3x^3e^{x^2}\big)$

Simplify first:

$$y = \ln3 + \ln(x^3) + \ln\big(e^{x^2}\big) = \ln3 + 3\ln x + x^2$$

(using $\ln(e^{x^2})=x^2$ directly, since $\ln$ and $e^{(\cdot)}$ undo each other).

Differentiate ($\ln3$ is just a constant, so its derivative is $0$):

$$\frac{dy}{dx} = \frac3x + 2x$$

**17.** Solve $2\ln(x)+\ln(4)=\ln(36)$.

Combine the left side using log properties: $2\ln x = \ln(x^2)$, so:

$$\ln(x^2) + \ln(4) = \ln(36)$$

$$\ln(4x^2) = \ln(36)$$

Since the logs are equal, their insides must be equal:

$$4x^2 = 36 \quad\Rightarrow\quad x^2=9 \quad\Rightarrow\quad x=3$$

(We take only the positive root, since $x$ must be positive for $\ln x$ to be defined in the original equation.)

**18.** $\displaystyle\int \frac{x^2+1}{x}\,dx$

Split the fraction first:

$$\frac{x^2+1}{x} = \frac{x^2}{x}+\frac1x = x+\frac1x$$

Now integrate term by term:

$$\int \left(x+\frac1x\right)dx = \frac{x^2}{2}+\ln|x|+C$$

---

### 🌍 Applied

**19.** $P(t)=500e^{0.05t}=1000$

$$e^{0.05t} = \frac{1000}{500}=2$$

$$0.05t = \ln2$$

$$t = \frac{\ln2}{0.05} = 20\ln2 \approx 13.86 \text{ years}$$

**20.** $A(t)=100e^{-0.2t}=25$

$$e^{-0.2t} = \frac{25}{100} = 0.25$$

$$-0.2t = \ln(0.25) = -\ln4$$

$$t = \frac{\ln4}{0.2} = 5\ln4 = 10\ln2 \approx 6.93 \text{ years}$$

**21.** $MC(x)=\dfrac{10}{x}$, from $x=1$ to $x=5$.

$$\int_1^5 \frac{10}{x}\,dx = 10\Big[\ln x\Big]_1^5 = 10\big(\ln5-\ln1\big) = 10\ln5 \quad(\text{since } \ln1=0)$$

$$\approx 10(1.6094) \approx 16.09$$

**Answer: total cost increase $\approx \$16.09$ (exactly $10\ln5$).**

**22.** $\dfrac{dV}{dt}=\dfrac{6}{t}$, from $t=1$ to $t=e$.

$$\int_1^e \frac6t\,dt = 6\Big[\ln t\Big]_1^e = 6\big(\ln e - \ln1\big) = 6(1-0) = 6$$

**Answer: total volume change $=6$ gallons.**
