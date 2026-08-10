# Unit 23: Antiderivatives — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int x^3\,dx$

Bump the exponent up by $1$ (to $4$), then divide by that new exponent:

$$\int x^3\,dx = \frac{x^4}{4}+C$$

**2.** $\displaystyle\int 5\,dx$

A constant antidifferentiates to that constant times $x$:

$$\int 5\,dx = 5x+C$$

**3.** $\displaystyle\int x^4\,dx$

$$\int x^4\,dx = \frac{x^5}{5}+C$$

**4.** $\displaystyle\int 3x^2\,dx$

The constant $3$ just tags along:

$$\int 3x^2\,dx = 3\cdot\frac{x^3}{3}+C = x^3+C$$

**5.** $\displaystyle\int (x^2+2x)\,dx$

Antidifferentiate each term separately:

$$\int (x^2+2x)\,dx = \frac{x^3}{3}+x^2+C$$

**6.** $\displaystyle\int (4x^3-3x^2+1)\,dx$

$$\int (4x^3-3x^2+1)\,dx = x^4-x^3+x+C$$

**7.** $\displaystyle\int \sqrt{x}\,dx$

Rewrite as a power first: $\sqrt{x}=x^{1/2}$.

$$\int x^{1/2}\,dx = \frac{x^{3/2}}{3/2}+C = \frac23x^{3/2}+C$$

---

### 🟡 Standard

**8.** $\displaystyle\int \sin x\,dx$

$$\int \sin x\,dx = -\cos x+C$$

**9.** $\displaystyle\int (3\cos x - 2\sin x)\,dx$

$$\int (3\cos x - 2\sin x)\,dx = 3\sin x - 2(-\cos x)+C = 3\sin x+2\cos x+C$$

**10.** $\displaystyle\int \sec^2x\,dx$

$$\int \sec^2x\,dx = \tan x+C$$

**11.** $\displaystyle\int \frac{2}{x^3}\,dx$

Rewrite: $\dfrac{2}{x^3}=2x^{-3}$.

$$\int 2x^{-3}\,dx = 2\cdot\frac{x^{-2}}{-2}+C = -x^{-2}+C = -\frac{1}{x^2}+C$$

**12.** $\displaystyle\int \left(x^2-\frac{1}{x^2}\right)dx$

Rewrite: $x^2-x^{-2}$.

$$\int x^2\,dx = \frac{x^3}{3}$$

$$\int -x^{-2}\,dx = -\frac{x^{-1}}{-1}+C = x^{-1}+C = \frac1x+C$$

Combining:

$$\int \left(x^2-\frac{1}{x^2}\right)dx = \frac{x^3}{3}+\frac1x+C$$

**13.** $\displaystyle\int (\sec x\tan x + \csc x\cot x)\,dx$

$$\int (\sec x\tan x + \csc x\cot x)\,dx = \sec x + (-\csc x)+C = \sec x-\csc x+C$$

**14.** $\displaystyle\int (4x^3-6\sqrt{x})\,dx$

Rewrite $\sqrt{x}=x^{1/2}$.

$$\int 4x^3\,dx = x^4$$

$$\int -6x^{1/2}\,dx = -6\cdot\frac{x^{3/2}}{3/2}+C = -4x^{3/2}+C$$

Combining:

$$\int (4x^3-6\sqrt{x})\,dx = x^4-4x^{3/2}+C$$

---

### 🔴 Challenge

**15.** $f'(x)=3x^2-4x+1$, $f(0)=5$.

First, find the general antiderivative:

$$f(x) = x^3-2x^2+x+C$$

Use $f(0)=5$: $f(0) = 0-0+0+C = C$. So $C=5$.

**$f(x) = x^3-2x^2+x+5$.**

**16.** $f'(x)=6x^2-2$, $f(1)=3$.

General antiderivative:

$$f(x) = 2x^3-2x+C$$

Use $f(1)=3$: $f(1) = 2-2+C = C$. So $C=3$.

**$f(x) = 2x^3-2x+3$.**

**17.** $a(t)=6t-4$, $v(0)=3$, $s(0)=2$.

First antidifferentiate $a(t)$ to get the general velocity function:

$$v(t) = 3t^2-4t+C_1$$

Use $v(0)=3$: $v(0)=0-0+C_1=C_1$. So $C_1=3$.

$$v(t) = 3t^2-4t+3$$

Now antidifferentiate $v(t)$ to get the general position function:

$$s(t) = t^3-2t^2+3t+C_2$$

Use $s(0)=2$: $s(0)=0-0+0+C_2=C_2$. So $C_2=2$.

**$v(t) = 3t^2-4t+3$ and $s(t) = t^3-2t^2+3t+2$.**

**18.** $f'(x)=2\sin x+3\cos x$, $f(0)=4$.

General antiderivative:

$$f(x) = -2\cos x+3\sin x+C$$

Use $f(0)=4$: $f(0) = -2\cos(0)+3\sin(0)+C = -2(1)+3(0)+C = -2+C$. So $-2+C=4 \Rightarrow C=6$.

**$f(x) = -2\cos x+3\sin x+6$.**

**19.** $\displaystyle\int (x+1)(x-2)\,dx$

Expand first, since the power rule can't be applied directly to a product:

$$(x+1)(x-2) = x^2-2x+x-2 = x^2-x-2$$

Now antidifferentiate term by term:

$$\int (x^2-x-2)\,dx = \frac{x^3}{3}-\frac{x^2}{2}-2x+C$$

---

### 🌍 Applied

**20.** $a(t)=-32$, $v(0)=48$, $s(0)=0$.

Antidifferentiate acceleration to get velocity:

$$v(t) = -32t+C_1$$

Use $v(0)=48$: $C_1=48$.

$$v(t) = -32t+48$$

Antidifferentiate velocity to get position:

$$s(t) = -16t^2+48t+C_2$$

Use $s(0)=0$: $C_2=0$.

$$s(t) = -16t^2+48t$$

Find the maximum height: this occurs when $v(t)=0$.

$$-32t+48=0 \quad\Rightarrow\quad t=\frac{48}{32}=1.5 \text{ seconds}$$

$$s(1.5) = -16(2.25)+48(1.5) = -36+72=36$$

**Answer: $v(t)=-32t+48$, $s(t)=-16t^2+48t$, and the maximum height is $36$ feet, reached at $t=1.5$ seconds.**

**21.** $MC(x)=3x^2-12x+15$, $C(0)=200$.

General antiderivative:

$$C(x) = x^3-6x^2+15x+K$$

(using $K$ here to avoid confusion with the cost function's own name $C$)

Use $C(0)=200$: $K=200$.

**$C(x) = x^3-6x^2+15x+200$.**

**22.** $MR(x)=50-2x$, $R(0)=0$.

General antiderivative:

$$R(x) = 50x-x^2+C$$

Use $R(0)=0$: $C=0$.

**$R(x) = 50x-x^2$.**

**23.** $a(t)=-10$, $v(0)=60$.

General antiderivative:

$$v(t) = -10t+C$$

Use $v(0)=60$: $C=60$.

$$v(t) = -10t+60$$

The car stops when $v(t)=0$:

$$-10t+60=0 \quad\Rightarrow\quad t=6$$

**Answer: $v(t)=-10t+60$, and the car comes to a complete stop after $6$ seconds.**
