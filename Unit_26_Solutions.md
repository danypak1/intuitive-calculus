# Unit 26: The Definite Integral — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int_1^4 f(x)\,dx=10$, find $\displaystyle\int_4^1 f(x)\,dx$.

Reversing the limits flips the sign:

$$\int_4^1 f(x)\,dx = -\int_1^4 f(x)\,dx = -10$$

**2.** $\displaystyle\int_0^3 f(x)\,dx=7$, find $\displaystyle\int_0^3 5f(x)\,dx$.

$$\int_0^3 5f(x)\,dx = 5\int_0^3 f(x)\,dx = 5(7)=35$$

**3.** $\displaystyle\int_2^2 f(x)\,dx$

By definition, integrating over an interval of zero width gives $0$, regardless of what $f$ is:

$$\int_2^2 f(x)\,dx = 0$$

**4.** $\displaystyle\int_0^2 f(x)\,dx=4$, $\displaystyle\int_2^5 f(x)\,dx=9$, find $\displaystyle\int_0^5 f(x)\,dx$.

By the additivity property:

$$\int_0^5 f(x)\,dx = \int_0^2 f(x)\,dx + \int_2^5 f(x)\,dx = 4+9=13$$

**5.** $\displaystyle\int_1^3 f(x)\,dx=6$, $\displaystyle\int_1^3 g(x)\,dx=2$, find $\displaystyle\int_1^3 [f(x)-g(x)]\,dx$.

$$\int_1^3 [f(x)-g(x)]\,dx = \int_1^3 f(x)\,dx - \int_1^3 g(x)\,dx = 6-2=4$$

**6.** $\displaystyle\int_0^4 f(x)\,dx=8$, $\displaystyle\int_0^4 g(x)\,dx=3$, find $\displaystyle\int_0^4 [2f(x)+3g(x)]\,dx$.

$$\int_0^4 [2f(x)+3g(x)]\,dx = 2\int_0^4 f(x)\,dx + 3\int_0^4 g(x)\,dx = 2(8)+3(3) = 16+9=25$$

---

### 🟡 Standard

**7.** $\displaystyle\int_0^5 f(x)\,dx=12$, $\displaystyle\int_3^5 f(x)\,dx=4$, find $\displaystyle\int_0^3 f(x)\,dx$.

By additivity: $\displaystyle\int_0^5 f(x)\,dx = \int_0^3 f(x)\,dx + \int_3^5 f(x)\,dx$.

$$12 = \int_0^3 f(x)\,dx + 4 \quad\Rightarrow\quad \int_0^3 f(x)\,dx = 8$$

**8.** $\displaystyle\int_1^6 f(x)\,dx=20$, $\displaystyle\int_1^4 f(x)\,dx=9$, find $\displaystyle\int_4^6 f(x)\,dx$.

By additivity: $\displaystyle\int_1^6 f(x)\,dx = \int_1^4 f(x)\,dx + \int_4^6 f(x)\,dx$.

$$20 = 9 + \int_4^6 f(x)\,dx \quad\Rightarrow\quad \int_4^6 f(x)\,dx = 11$$

**9.** $\displaystyle\int_2^7 f(x)\,dx=15$, find $\displaystyle\int_7^2 f(x)\,dx$ and $\displaystyle\int_7^2 [-3f(x)]\,dx$.

$$\int_7^2 f(x)\,dx = -\int_2^7 f(x)\,dx = -15$$

$$\int_7^2 [-3f(x)]\,dx = -3\int_7^2 f(x)\,dx = -3(-15) = 45$$

**10.** $g(x)=f(x)+2$.

$$\int_1^5 g(x)\,dx = \int_1^5 \big[f(x)+2\big]\,dx = \int_1^5 f(x)\,dx + \int_1^5 2\,dx = \int_1^5 f(x)\,dx + 2(5-1) = \int_1^5 f(x)\,dx + 8$$

**Answer: $\displaystyle\int_1^5 g(x)\,dx$ is exactly $8$ more than $\displaystyle\int_1^5 f(x)\,dx$.** This makes sense geometrically: shifting the entire graph up by $2$ units adds a rectangular strip of height $2$ and width $4$ (the length of the interval) underneath the new curve, and $2\times4=8$.

**11.** $f$ continuous, $f(x)\ge0$ on $[-3,3]$, $\displaystyle\int_{-3}^3 f(x)\,dx=0$.

**Conclusion: $f(x)=0$ for every $x$ in $[-3,3]$.**

**Reasoning:** suppose, for contradiction, that $f$ were positive at some point in the interval. Since $f$ is continuous, it would then have to stay positive on some small stretch of $x$-values surrounding that point (a continuous function can't jump instantly back to zero). That small positive stretch would contribute a strictly positive amount of area to the integral. But we're told the *total* integral is exactly $0$, and since $f(x)\ge0$ everywhere else too (no negative area to cancel it out), there's no way to make the total come out to $0$ if any part of it is strictly positive. So $f$ must be $0$ at every single point in the interval.

**12.** $m=2$, $M=6$ on $[1,4]$ (interval length $=3$).

$$m(b-a) \le \int_1^4 f(x)\,dx \le M(b-a)$$

$$2(3) \le \int_1^4 f(x)\,dx \le 6(3)$$

$$6 \le \int_1^4 f(x)\,dx \le 18$$

---

### 🔴 Challenge

**13.** Show $1 \le \displaystyle\int_0^1 \sqrt{x^2+1}\,dx \le \sqrt2$.

Let $f(x)=\sqrt{x^2+1}$. Since $x^2+1$ is increasing for $x\ge0$ (as $x$ grows, $x^2$ grows), and the square root function preserves increasing order, $f(x)$ is also increasing on $[0,1]$.

So the minimum of $f$ on $[0,1]$ occurs at $x=0$: $f(0)=\sqrt{0+1}=1$.

The maximum occurs at $x=1$: $f(1)=\sqrt{1+1}=\sqrt2$.

By the Max-Min Inequality, with $b-a=1-0=1$:

$$1\times(1) \le \int_0^1\sqrt{x^2+1}\,dx \le \sqrt2\times(1)$$

$$1 \le \int_0^1\sqrt{x^2+1}\,dx \le \sqrt2$$

**This confirms the claim.**

**14.** Bounds for $\displaystyle\int_0^2 (x^2+3)\,dx$.

$f(x)=x^2+3$ is increasing on $[0,2]$ (since $f'(x)=2x\ge0$ there). So the minimum is $f(0)=3$, and the maximum is $f(2)=4+3=7$.

With $b-a=2$:

$$3(2) \le \int_0^2 (x^2+3)\,dx \le 7(2)$$

$$6 \le \int_0^2 (x^2+3)\,dx \le 14$$

**15.** Is $\displaystyle\int_{-2}^{2} (x^3-4x)\,dx = 0$?

Let $f(x)=x^3-4x$. Check whether it's odd:

$$f(-x) = (-x)^3-4(-x) = -x^3+4x = -(x^3-4x) = -f(x)$$

Since $f(-x)=-f(x)$, **$f$ is an odd function**.

The interval $[-2,2]$ is symmetric about $0$. By the odd-function symmetry property:

$$\int_{-2}^{2}(x^3-4x)\,dx = 0$$

**Yes — the integral equals $0$, confirmed without any direct evaluation.**

**16.** Can $\displaystyle\int_{-\pi}^{\pi} x^2\cos x\,dx$ be simplified using symmetry?

Let $f(x)=x^2\cos x$. Check its symmetry:

$$f(-x) = (-x)^2\cos(-x) = x^2\cos x = f(x)$$

(using the fact that $(-x)^2=x^2$ is even, and $\cos(-x)=\cos x$ is even, so their product is even too.)

Since $f(-x)=f(x)$, **$f$ is an even function.**

This integral does **not** vanish to zero — the even-function property only guarantees a simplification, not automatic cancellation (cancellation to zero only happens for *odd* functions). Instead, it simplifies to:

$$\int_{-\pi}^{\pi} x^2\cos x\,dx = 2\int_0^{\pi} x^2\cos x\,dx$$

**This cuts the required computation in half — you'd only need to evaluate the integral over $[0,\pi]$ and double the result — but it doesn't eliminate the integral the way an odd function would.**

**17.** Why does $\displaystyle\int_{-1}^{1} \left(x^{2024}\sin x + \frac{x^7}{1+x^2}\right)dx = 0$?

**Classify the first term, $x^{2024}\sin x$:** $x^{2024}$ has an even exponent, so it's an **even** function. $\sin x$ is a well-known **odd** function. By the combination rule, even $\times$ odd $=$ **odd**. So the first term is odd.

**Classify the second term, $\dfrac{x^7}{1+x^2}$:** $x^7$ has an odd exponent, so it's **odd**. The denominator $1+x^2$ is a constant plus an even power, so it's **even**. By the combination rule, odd $\div$ even $=$ **odd**. So the second term is odd too.

**Combine:** odd $+$ odd $=$ **odd**. So the entire integrand is an odd function.

Since the interval $[-1,1]$ is symmetric about $0$, and the whole integrand is odd, the odd-function symmetry property applies directly:

$$\int_{-1}^{1} \left(x^{2024}\sin x + \frac{x^7}{1+x^2}\right)dx = 0$$

**No antiderivative techniques were needed at all — the symmetry argument alone fully settles the answer.**

**18.** Is $\displaystyle\int_0^6 f(x)\,dx=20$ consistent with $2\le f(x)\le5$ on $[0,6]$?

Using the Max-Min Inequality with $m=2$, $M=5$, and $b-a=6$:

$$2(6) \le \int_0^6 f(x)\,dx \le 5(6)$$

$$12 \le \int_0^6 f(x)\,dx \le 30$$

Since $12 \le 20 \le 30$, **yes, this is fully consistent** — the given value of $20$ falls comfortably within the guaranteed bounds.

---

### 🌍 Applied

**19.** $-50\le p(t)\le 200$ on $[0,30]$ (interval length $=30$).

$$-50(30) \le \int_0^{30} p(t)\,dt \le 200(30)$$

$$-1500 \le \int_0^{30} p(t)\,dt \le 6000$$

**Answer: total monthly profit is between $-\$1500$ and $\$6000$.**

**20.** $d(t)$ is odd on $[-6,6]$.

By the odd-function symmetry property:

$$\int_{-6}^{6} d(t)\,dt = 0$$

**Interpretation:** the net temperature deviation over the entire day sums to exactly zero — the amount by which mornings run below the daily average exactly balances the amount by which evenings run above it, so there's no net bias across the full day.

**21.** $\displaystyle\int_0^{10} r(t)\,dt=150$, $\displaystyle\int_0^{10} s(t)\,dt=90$.

$$\int_0^{10} \big[r(t)+s(t)\big]\,dt = \int_0^{10} r(t)\,dt + \int_0^{10} s(t)\,dt = 150+90=240$$

**Answer: total combined output $=240$ gallons.**

**22.** $40\le v(t)\le65$ on $[0,3]$ (interval length $=3$).

$$40(3) \le \int_0^3 v(t)\,dt \le 65(3)$$

$$120 \le \int_0^3 v(t)\,dt \le 195$$

**Answer: total distance traveled is between $120$ and $195$ miles.**
