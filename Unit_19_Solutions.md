# Unit 19: Monotonic Functions and the First Derivative Test — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2-4x+1$

$f'(x)=2x-4$. Critical point: $x=2$.

Test $x<2$ (e.g., $x=0$): $f'(0)=-4<0$ → decreasing. Test $x>2$ (e.g., $x=3$): $f'(3)=2>0$ → increasing.

**Decreasing on $(-\infty,2)$, increasing on $(2,\infty)$. Local minimum at $x=2$** (sign goes $-$ to $+$).

**2.** $f(x)=-x^2+6x-5$

$f'(x)=-2x+6$. Critical point: $x=3$.

Test $x<3$: $f'(0)=6>0$ → increasing. Test $x>3$: $f'(4)=-2<0$ → decreasing.

**Increasing on $(-\infty,3)$, decreasing on $(3,\infty)$. Local maximum at $x=3$.**

**3.** $f(x)=x^3-3x$

$f'(x)=3x^2-3=3(x-1)(x+1)$. Critical points: $x=1$, $x=-1$.

Test $x<-1$ (e.g., $-2$): $3(-3)(-1)=9>0$ → increasing. Test $-1<x<1$ (e.g., $0$): $3(-1)(1)=-3<0$ → decreasing. Test $x>1$ (e.g., $2$): $3(1)(3)=9>0$ → increasing.

**Increasing on $(-\infty,-1)$, decreasing on $(-1,1)$, increasing on $(1,\infty)$. Local max at $x=-1$; local min at $x=1$.**

**4.** $f(x)=x^3-12x$

$f'(x)=3x^2-12=3(x-2)(x+2)$. Critical points: $x=2$, $x=-2$.

Test $x<-2$ ($-3$): $3(-5)(-1)=15>0$ → increasing. Test $-2<x<2$ ($0$): $3(-2)(2)=-12<0$ → decreasing. Test $x>2$ ($3$): $3(1)(5)=15>0$ → increasing.

**Increasing on $(-\infty,-2)$, decreasing on $(-2,2)$, increasing on $(2,\infty)$. Local max at $x=-2$; local min at $x=2$.**

**5.** $f(x)=x^2+2x-3$

$f'(x)=2x+2$. Critical point: $x=-1$.

Test $x<-1$: $f'(-2)=-2<0$ → decreasing. Test $x>-1$: $f'(0)=2>0$ → increasing.

**Decreasing on $(-\infty,-1)$, increasing on $(-1,\infty)$. Local minimum at $x=-1$.**

**6.** $f(x)=2x^3-6x$

$f'(x)=6x^2-6=6(x-1)(x+1)$. Critical points: $x=1$, $x=-1$.

Test $x<-1$ ($-2$): $6(-3)(-1)=18>0$ → increasing. Test $-1<x<1$ ($0$): $6(-1)(1)=-6<0$ → decreasing. Test $x>1$ ($2$): $6(1)(3)=18>0$ → increasing.

**Increasing on $(-\infty,-1)$, decreasing on $(-1,1)$, increasing on $(1,\infty)$. Local max at $x=-1$; local min at $x=1$.**

---

### 🟡 Standard

**7.** $f(x)=x^3-3x^2-9x+5$

$f'(x)=3x^2-6x-9=3(x-3)(x+1)$. Critical points: $x=3$, $x=-1$.

Test $x<-1$ ($-2$): $3(-5)(-1)=15>0$ → increasing. Test $-1<x<3$ ($0$): $3(-3)(1)=-9<0$ → decreasing. Test $x>3$ ($4$): $3(1)(5)=15>0$ → increasing.

**Increasing on $(-\infty,-1)$, decreasing on $(-1,3)$, increasing on $(3,\infty)$. Local max at $x=-1$; local min at $x=3$.**

**8.** $f(x)=x^4-4x^3$

$f'(x)=4x^3-12x^2=4x^2(x-3)$. Critical points: $x=0$, $x=3$.

Test $x<0$ ($-1$): $4(1)(-4)=-16<0$ → decreasing. Test $0<x<3$ ($1$): $4(1)(-2)=-8<0$ → decreasing (same sign as before — no change at $x=0$). Test $x>3$ ($4$): $4(16)(1)=64>0$ → increasing.

**Decreasing on $(-\infty,0)\cup(0,3)$ (i.e., decreasing throughout $(-\infty,3)$), increasing on $(3,\infty)$. At $x=0$: no sign change, so it's neither a local max nor min. Local min at $x=3$.**

**9.** $f(x)=3x^4-4x^3-12x^2+1$

$f'(x)=12x^3-12x^2-24x=12x(x-2)(x+1)$. Critical points: $x=0$, $x=2$, $x=-1$.

Test $x<-1$ ($-2$): $x(x-2)(x+1) = (-2)(-4)(-1)=-8<0$ → decreasing.

Test $-1<x<0$ ($-0.5$): $(-0.5)(-2.5)(0.5)=0.625>0$ → increasing.

Test $0<x<2$ ($1$): $(1)(-1)(2)=-2<0$ → decreasing.

Test $x>2$ ($3$): $(3)(1)(4)=12>0$ → increasing.

**Decreasing on $(-\infty,-1)$, increasing on $(-1,0)$, decreasing on $(0,2)$, increasing on $(2,\infty)$. Local min at $x=-1$; local max at $x=0$; local min at $x=2$.**

**10.** $f(x)=\dfrac{x}{x^2+1}$

Using the quotient rule: $f'(x) = \dfrac{1\cdot(x^2+1) - x\cdot2x}{(x^2+1)^2} = \dfrac{1-x^2}{(x^2+1)^2}$.

The denominator is always positive, so the sign of $f'$ matches the sign of $1-x^2=(1-x)(1+x)$. Critical points: $x=1$, $x=-1$.

Test $x<-1$ ($-2$): $1-4=-3<0$ → decreasing. Test $-1<x<1$ ($0$): $1-0=1>0$ → increasing. Test $x>1$ ($2$): $1-4=-3<0$ → decreasing.

**Decreasing on $(-\infty,-1)$, increasing on $(-1,1)$, decreasing on $(1,\infty)$. Local min at $x=-1$; local max at $x=1$.**

**11.** $f(x)=(x-1)^2(x+2)$

Using the product rule with $u=(x-1)^2$ ($u'=2(x-1)$) and $v=(x+2)$ ($v'=1$):

$$f'(x) = 2(x-1)(x+2) + (x-1)^2(1) = (x-1)\big[2(x+2)+(x-1)\big] = (x-1)(3x+3) = 3(x-1)(x+1)$$

Critical points: $x=1$, $x=-1$.

Test $x<-1$ ($-2$): $3(-3)(-1)=9>0$ → increasing. Test $-1<x<1$ ($0$): $3(-1)(1)=-3<0$ → decreasing. Test $x>1$ ($2$): $3(1)(3)=9>0$ → increasing.

**Increasing on $(-\infty,-1)$, decreasing on $(-1,1)$, increasing on $(1,\infty)$. Local max at $x=-1$; local min at $x=1$.**

**12.** $f(x)=x^5-5x$

$f'(x)=5x^4-5=5(x^4-1)=5(x^2-1)(x^2+1)$. Since $x^2+1$ is always positive, the sign is determined by $(x^2-1)=(x-1)(x+1)$. Critical points: $x=1$, $x=-1$.

Test $x<-1$ ($-2$): $(-3)(-1)=3>0$ → increasing. Test $-1<x<1$ ($0$): $(-1)(1)=-1<0$ → decreasing. Test $x>1$ ($2$): $(1)(3)=3>0$ → increasing.

**Increasing on $(-\infty,-1)$, decreasing on $(-1,1)$, increasing on $(1,\infty)$. Local max at $x=-1$; local min at $x=1$.**

---

### 🔴 Challenge

**13.** $f(x)=x^3-\dfrac32x^2-6x+3$

$f'(x)=3x^2-3x-6=3(x^2-x-2)=3(x-2)(x+1)$. Critical points: $x=2$, $x=-1$.

Test $x<-1$ ($-2$): $3(-4)(-1)=12>0$ → increasing. Test $-1<x<2$ ($0$): $3(-2)(1)=-6<0$ → decreasing. Test $x>2$ ($3$): $3(1)(4)=12>0$ → increasing.

**Increasing on $(-\infty,-1)$, decreasing on $(-1,2)$, increasing on $(2,\infty)$.**

**Local max at $x=-1$:** $f(-1) = -1-\dfrac32-(-6)+3 = -1-1.5+6+3 = 6.5 = \dfrac{13}{2}$.

**Local min at $x=2$:** $f(2) = 8-\dfrac32(4)-12+3 = 8-6-12+3 = -7$.

**14.** $f(x)=x^{2/3}(x-5)$

First, expand: $f(x) = x^{5/3}-5x^{2/3}$.

$$f'(x) = \frac53x^{2/3} - \frac{10}{3}x^{-1/3}$$

Factor out $\dfrac53x^{-1/3}$:

$$f'(x) = \frac53x^{-1/3}(x-2) = \frac{5(x-2)}{3x^{1/3}}$$

Critical points: $x=2$ (where the numerator is $0$) and $x=0$ (where the denominator is $0$, making $f'$ undefined).

Test $x<0$ ($-1$): numerator $=5(-3)=-15$; denominator $=3(-1)^{1/3}=3(-1)=-3$. $f'=-15/-3=5>0$ → increasing.

Test $0<x<2$ ($1$): numerator $=5(-1)=-5$; denominator $=3(1)=3$. $f'=-5/3<0$ → decreasing.

Test $x>2$ ($3$): numerator $=5(1)=5$; denominator $=3(3^{1/3})>0$. $f'>0$ → increasing.

**Increasing on $(-\infty,0)$, decreasing on $(0,2)$, increasing on $(2,\infty)$.**

**At $x=0$ (a cusp, since $f'$ is undefined there):** sign changes $+$ to $-$, so **$x=0$ is a local maximum**, with $f(0)=0$.

**At $x=2$:** sign changes $-$ to $+$, so **$x=2$ is a local minimum**, with $f(2) = 2^{2/3}(2-5) = -3\cdot2^{2/3} = -3\sqrt[3]{4} \approx -4.76$.

**15.** $f(x)=\sin x+\cos x$ on $[0,2\pi]$

$f'(x)=\cos x-\sin x$. Setting this to $0$: $\tan x=1$, giving $x=\dfrac{\pi}{4}$ and $x=\dfrac{5\pi}{4}$ within $[0,2\pi]$.

Test $[0,\pi/4)$ (e.g., $x=0$): $f'(0)=1-0=1>0$ → increasing.

Test $(\pi/4,5\pi/4)$ (e.g., $x=\pi$): $f'(\pi)=-1-0=-1<0$ → decreasing.

Test $(5\pi/4,2\pi]$ (e.g., $x=\frac{3\pi}{2}$): $f'\left(\frac{3\pi}{2}\right)=0-(-1)=1>0$ → increasing.

**Increasing on $\left[0,\frac{\pi}{4}\right)$, decreasing on $\left(\frac{\pi}{4},\frac{5\pi}{4}\right)$, increasing on $\left(\frac{5\pi}{4},2\pi\right]$.**

**Local max at $x=\dfrac{\pi}{4}$**, where $f\left(\dfrac{\pi}{4}\right)=\sqrt2$. **Local min at $x=\dfrac{5\pi}{4}$**, where $f\left(\dfrac{5\pi}{4}\right)=-\sqrt2$.

**16.** $f(x)=x^4-8x^2+3$

$f'(x)=4x^3-16x=4x(x^2-4)=4x(x-2)(x+2)$. Critical points: $x=0$, $x=2$, $x=-2$.

Test $x<-2$ ($-3$): $4(-3)(-5)(-1)=-60<0$ → decreasing.

Test $-2<x<0$ ($-1$): $4(-1)(-3)(1)=12>0$ → increasing.

Test $0<x<2$ ($1$): $4(1)(-1)(3)=-12<0$ → decreasing.

Test $x>2$ ($3$): $4(3)(1)(5)=60>0$ → increasing.

**Decreasing on $(-\infty,-2)$, increasing on $(-2,0)$, decreasing on $(0,2)$, increasing on $(2,\infty)$. Local min at $x=-2$; local max at $x=0$; local min at $x=2$.**

**17.** $f(x)=\dfrac{x^2-4}{x}$

Simplify first: $f(x) = x-\dfrac4x = x-4x^{-1}$.

$$f'(x) = 1+4x^{-2} = 1+\frac{4}{x^2}$$

Since $\dfrac{4}{x^2}$ is always positive for $x\ne0$, $f'(x)$ is **always greater than $1$**, meaning it's always positive — there's no $x$ where $f'(x)=0$. The only place $f'$ is undefined is $x=0$, which isn't in the domain of $f$ at all (it's excluded, not a true critical point to classify).

**Answer: $f$ is increasing on $(-\infty,0)$ and increasing on $(0,\infty)$ (each piece separately, since $x=0$ is a vertical asymptote that breaks the domain). There are no local maxima or minima anywhere.**

---

### 🌍 Applied

**18.** $P(x)=-x^3+15x^2-48x+10$, $x\ge0$

$P'(x)=-3x^2+30x-48=-3(x^2-10x+16)=-3(x-2)(x-8)$. Critical points: $x=2$, $x=8$.

Test $0\le x<2$ ($1$): $-3(-1)(-7)=-21<0$ → decreasing.

Test $2<x<8$ ($5$): $-3(3)(-3)=27>0$ → increasing.

Test $x>8$ ($9$): $-3(7)(1)=-21<0$ → decreasing.

**Decreasing on $[0,2)$, increasing on $(2,8)$, decreasing on $(8,\infty)$. Local minimum at $x=2$; local maximum profit at $x=8$ units.**

**19.** $P(t)=-t^3+9t^2+120$, $t$ in $[0,10]$

$P'(t)=-3t^2+18t=-3t(t-6)$. Critical points: $t=0$, $t=6$.

Test $0<t<6$ ($3$): $-3(3)(-3)=27>0$ → increasing.

Test $6<t<10$ ($8$): $-3(8)(2)=-48<0$ → decreasing.

**Increasing on $(0,6)$, decreasing on $(6,10)$. Local (and here, absolute on this interval) maximum population at $t=6$ years.**

**20.** $h(t)=-16t^2+64t+5$

$h'(t)=-32t+64$. Critical point: $t=2$.

Test $t<2$: $h'(0)=64>0$ → increasing. Test $t>2$: $h'(3)=-32<0$ → decreasing.

**Increasing on $(-\infty,2)$ (physically, $[0,2)$), decreasing on $(2,\infty)$. Local maximum height occurs at $t=2$ seconds** — the peak of the ball's flight.

**21.** $T(t)=t^3-6t^2+9t+20$, $t$ in $[0,5]$

$T'(t)=3t^2-12t+9=3(t-1)(t-3)$. Critical points: $t=1$, $t=3$.

Test $0\le t<1$ ($0.5$): $3(-0.5)(-2.5)=3.75>0$ → increasing.

Test $1<t<3$ ($2$): $3(1)(-1)=-3<0$ → decreasing.

Test $3<t\le5$ ($4$): $3(3)(1)=9>0$ → increasing.

**Increasing on $[0,1)$, decreasing on $(1,3)$, increasing on $(3,5]$.**

**Local max at $t=1$:** $T(1) = 1-6+9+20=24°F$.

**Local min at $t=3$:** $T(3) = 27-54+27+20=20°F$.
