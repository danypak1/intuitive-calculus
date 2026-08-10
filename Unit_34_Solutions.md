# Unit 34: Indeterminate Forms and L'Hôpital's Rule — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\lim_{x\to2}\frac{x^2-4}{x-2}$

Plug in: $\dfrac{4-4}{0}=\dfrac00$ — indeterminate. Apply L'Hôpital:

$$\lim_{x\to2}\frac{2x}{1} = 2(2)=4$$

**Answer: $4$.**

**2.** $\displaystyle\lim_{x\to0}\frac{\sin x}{x}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{\cos x}{1} = \cos0=1$$

**Answer: $1$.**

**3.** $\displaystyle\lim_{x\to0}\frac{e^x-1}{x}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{e^x}{1} = e^0=1$$

**Answer: $1$.**

**4.** $\displaystyle\lim_{x\to3}\frac{x^2-9}{x-3}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to3}\frac{2x}{1} = 6$$

**Answer: $6$.**

**5.** $\displaystyle\lim_{x\to0}\frac{1-\cos x}{x}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{\sin x}{1} = \sin0=0$$

**Answer: $0$.**

**6.** $\displaystyle\lim_{x\to1}\frac{x^3-1}{x-1}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to1}\frac{3x^2}{1} = 3$$

**Answer: $3$.**

---

### 🟡 Standard

**7.** $\displaystyle\lim_{x\to\infty}\frac{3x^2+2x}{5x^2-1}$

$\dfrac{\infty}{\infty}$. Apply L'Hôpital:

$$\lim_{x\to\infty}\frac{6x+2}{10x}$$

Still $\dfrac{\infty}{\infty}$. Apply again:

$$\lim_{x\to\infty}\frac{6}{10} = \frac35$$

**Answer: $\dfrac35$.**

**8.** $\displaystyle\lim_{x\to0}\frac{x^2+3}{x+1}$

Plug in directly: $\dfrac{0+3}{0+1}=\dfrac31=3$. **This is NOT an indeterminate form** — it's just an ordinary number. L'Hôpital's Rule does not apply here.

**Answer: $3$** (found by direct substitution, no L'Hôpital needed).

**9.** $\displaystyle\lim_{x\to0}\frac{\tan x}{x}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{\sec^2x}{1} = \sec^2(0) = 1$$

**Answer: $1$.**

**10.** $\displaystyle\lim_{x\to\infty}\frac{\ln x}{x}$

$\dfrac{\infty}{\infty}$. Apply L'Hôpital:

$$\lim_{x\to\infty}\frac{1/x}{1} = \lim_{x\to\infty}\frac1x = 0$$

**Answer: $0$.**

**11.** $\displaystyle\lim_{x\to0}\frac{e^{2x}-1}{3x}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{2e^{2x}}{3} = \frac{2e^0}{3} = \frac23$$

**Answer: $\dfrac23$.**

**12.** $\displaystyle\lim_{x\to\pi}\frac{\sin x}{x-\pi}$

$\dfrac00$ (since $\sin\pi=0$). Apply L'Hôpital:

$$\lim_{x\to\pi}\frac{\cos x}{1} = \cos\pi = -1$$

**Answer: $-1$.**

---

### 🔴 Challenge

**13.** $\displaystyle\lim_{x\to1}\frac{x^3-1}{4x^3-x-3}$

Check: numerator $=1-1=0$; denominator $=4-1-3=0$. $\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to1}\frac{3x^2}{12x^2-1} = \frac{3(1)}{12(1)-1} = \frac{3}{11}$$

**Answer: $\dfrac{3}{11}$.**

**14.** $\displaystyle\lim_{t\to0}\frac{\sin(t^2)}{t^2}$

Check: numerator $=\sin(0)=0$; denominator $=0$. $\dfrac00$. Apply L'Hôpital (differentiating with respect to $t$):

$$\lim_{t\to0}\frac{\cos(t^2)\cdot2t}{2t}$$

Cancel the $2t$ (valid as $t\to0$ but $t\ne0$):

$$\lim_{t\to0}\cos(t^2) = \cos(0) = 1$$

**Answer: $1$.**

**15.** $\displaystyle\lim_{x\to1}\frac{x-1}{\ln x - \sin(\pi x) + x - 1}$

Check: numerator $=0$; denominator $=\ln1-\sin\pi+1-1 = 0-0+0=0$. $\dfrac00$. Apply L'Hôpital:

Numerator's derivative: $1$.

Denominator's derivative: $\dfrac1x - \pi\cos(\pi x) + 1$.

At $x=1$: $\dfrac11 - \pi\cos(\pi) + 1 = 1-\pi(-1)+1 = 1+\pi+1 = 2+\pi$.

$$\lim_{x\to1}\frac{1}{\frac1x-\pi\cos(\pi x)+1} = \frac{1}{2+\pi}$$

**Answer: $\dfrac{1}{2+\pi}$.**

**16.** $\displaystyle\lim_{x\to0}\frac{\tan^2x(1-\cos x)}{x^4}$

Rather than brute-forcing repeated L'Hôpital on this tangled product, it's much cleaner to **split the limit into two recognizable pieces**:

$$\frac{\tan^2x(1-\cos x)}{x^4} = \left(\frac{\tan x}{x}\right)^2 \cdot \frac{1-\cos x}{x^2}$$

**First piece:** from Problem 9, $\displaystyle\lim_{x\to0}\frac{\tan x}{x}=1$, so $\displaystyle\lim_{x\to0}\left(\frac{\tan x}{x}\right)^2 = 1^2=1$.

**Second piece:** $\displaystyle\lim_{x\to0}\frac{1-\cos x}{x^2}$. Check: $\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{\sin x}{2x}$$

Still $\dfrac00$. Apply again:

$$\lim_{x\to0}\frac{\cos x}{2} = \frac12$$

**Combine both pieces:**

$$1 \times \frac12 = \frac12$$

**Answer: $\dfrac12$.**

**17.** $\displaystyle\lim_{x\to0}\frac{x-\sin x}{x^3}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{1-\cos x}{3x^2}$$

Still $\dfrac00$. Apply again:

$$\lim_{x\to0}\frac{\sin x}{6x}$$

Still $\dfrac00$. Apply a third time:

$$\lim_{x\to0}\frac{\cos x}{6} = \frac16$$

**Answer: $\dfrac16$.**

---

### 🌍 Applied

**18.** Show $\displaystyle\lim_{t\to a}\frac{t^2-a^2}{t-a}=2a$.

Check: at $t=a$, numerator $=a^2-a^2=0$; denominator $=a-a=0$. $\dfrac00$. Apply L'Hôpital (differentiating with respect to $t$, treating $a$ as a constant):

$$\lim_{t\to a}\frac{2t}{1} = 2a$$

**Confirmed.** This exactly matches the difference-quotient definition of the derivative from Unit 7: for $f(t)=t^2$, this limit is precisely $f'(a)$, and since $f'(t)=2t$, we get $f'(a)=2a$ — the same answer, arrived at two different ways.

**19.** $C(x)=x^2+3x$, evaluate $\displaystyle\lim_{x\to0}\dfrac{C(x)-C(0)}{x}$.

$C(0)=0$. This limit is $\dfrac00$ at $x=0$. Apply L'Hôpital (differentiating the numerator as a function of $x$, since $C(0)$ is just a constant):

$$\lim_{x\to0}\frac{C'(x)}{1} = C'(0)$$

$C'(x)=2x+3$, so $C'(0)=3$.

**Answer: $3$**, which matches $C'(0)=3$ exactly — confirming that this limit *is* the definition of the derivative at $x=0$.

**20.** Show $\displaystyle\lim_{t\to0}\dfrac{1-e^{-kt}}{t}=k$.

Check: at $t=0$, numerator $=1-e^0=1-1=0$; denominator $=0$. $\dfrac00$. Apply L'Hôpital:

$$\lim_{t\to0}\frac{ke^{-kt}}{1} = ke^{0} = k$$

**Confirmed: the limit equals $k$.**

**21.** $\displaystyle\lim_{x\to0}\frac{\sin(3x)}{\sin(5x)}$

$\dfrac00$. Apply L'Hôpital:

$$\lim_{x\to0}\frac{3\cos(3x)}{5\cos(5x)} = \frac{3\cos(0)}{5\cos(0)} = \frac35$$

**Answer: $\dfrac35$.**
