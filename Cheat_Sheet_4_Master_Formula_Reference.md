# Master Formula Reference Sheet

*A compact, no-explanation reference to every formula in the course. Use the individual unit "Toolbox" sections if you need the plain-language explanation behind any of these — this sheet is just for fast lookup.*

---

## Limits and Continuity

$$\lim_{x\to a} f(x) = L$$

**Limit laws:** sums, products, quotients, and constant multiples of limits behave exactly like the corresponding operations on the individual limits (as long as the pieces exist).

**Continuity at $x=a$:** all three must hold:
$$f(a) \text{ is defined} \qquad \lim_{x\to a}f(x) \text{ exists} \qquad \lim_{x\to a}f(x) = f(a)$$

**Limits at infinity (rational functions):** compare degrees of numerator and denominator — top smaller $\rightarrow$ limit is $0$; top equal $\rightarrow$ limit is the ratio of leading coefficients; top bigger $\rightarrow$ limit is $\pm\infty$.

---

## Derivative Definition

$$f'(a) = \lim_{h\to 0}\frac{f(a+h)-f(a)}{h} \qquad f'(x) = \lim_{h\to 0}\frac{f(x+h)-f(x)}{h}$$

---

## Basic Derivative Rules

$$\frac{d}{dx}[x^n] = nx^{n-1} \qquad \frac{d}{dx}[c] = 0 \qquad \frac{d}{dx}[cf(x)] = cf'(x)$$

$$\frac{d}{dx}[f\pm g] = f'\pm g'$$

**Product Rule:** $\dfrac{d}{dx}[fg] = f'g+fg'$

**Quotient Rule:** $\dfrac{d}{dx}\left[\dfrac fg\right] = \dfrac{f'g-fg'}{g^2}$

**Chain Rule:** $\dfrac{d}{dx}\big[f(g(x))\big] = f'(g(x))\cdot g'(x)$

---

## Trig Derivatives

$$\frac{d}{dx}[\sin x]=\cos x \qquad \frac{d}{dx}[\cos x]=-\sin x \qquad \frac{d}{dx}[\tan x]=\sec^2x$$

$$\frac{d}{dx}[\cot x]=-\csc^2x \qquad \frac{d}{dx}[\sec x]=\sec x\tan x \qquad \frac{d}{dx}[\csc x]=-\csc x\cot x$$

## Exponential and Log Derivatives

$$\frac{d}{dx}[e^x]=e^x \qquad \frac{d}{dx}[\ln x]=\frac1x$$

## Inverse Trig Derivatives

$$\frac{d}{dx}[\arcsin x]=\frac{1}{\sqrt{1-x^2}} \qquad \frac{d}{dx}[\arccos x]=\frac{-1}{\sqrt{1-x^2}} \qquad \frac{d}{dx}[\arctan x]=\frac{1}{1+x^2}$$

**Inverse function derivative:** $(f^{-1})'(a) = \dfrac{1}{f'(f^{-1}(a))}$

---

## Motion

$$v(t)=s'(t) \qquad a(t)=v'(t)=s''(t) \qquad \text{speed}=|v(t)|$$

Speeding up: $v$ and $a$ same sign. Slowing down: $v$ and $a$ opposite signs.

---

## Linearization

$$L(x) = f(a)+f'(a)(x-a) \qquad dy = f'(x)\,dx$$

---

## Key Theorems

**Mean Value Theorem:** if $f$ continuous on $[a,b]$, differentiable on $(a,b)$:
$$f'(c) = \frac{f(b)-f(a)}{b-a} \text{ for some } c \text{ in } (a,b)$$

**First Derivative Test:** $f'$ changes $+\to-$: local max. $f'$ changes $-\to+$: local min.

**Second Derivative Test:** $f''(c)>0$: local min. $f''(c)<0$: local max. $f''(c)=0$: inconclusive.

**Concavity:** $f''>0$: concave up. $f''<0$: concave down. Inflection point: concavity changes.

**Newton's Method:** $x_{n+1} = x_n - \dfrac{f(x_n)}{f'(x_n)}$

---

## Basic Antiderivatives

$$\int x^n\,dx = \frac{x^{n+1}}{n+1}+C \ (n\ne-1) \qquad \int \frac1x\,dx=\ln|x|+C \qquad \int e^x\,dx=e^x+C$$

$$\int \sin x\,dx=-\cos x+C \qquad \int \cos x\,dx=\sin x+C \qquad \int \sec^2x\,dx=\tan x+C$$

$$\int \frac{dx}{\sqrt{a^2-x^2}}=\arcsin\left(\frac xa\right)+C \qquad \int \frac{dx}{a^2+x^2}=\frac1a\arctan\left(\frac xa\right)+C$$

---

## The Definite Integral

$$\int_a^a f(x)\,dx=0 \qquad \int_a^b f\,dx=-\int_b^a f\,dx \qquad \int_a^b f+\int_b^c f = \int_a^c f$$

**Max-Min Inequality:** if $m\le f(x)\le M$ on $[a,b]$: $\quad m(b-a)\le\int_a^b f(x)\,dx\le M(b-a)$

**Odd/Even symmetry** (on $[-a,a]$): odd function $\rightarrow$ integral is $0$. Even function $\rightarrow \int_{-a}^a f = 2\int_0^a f$.

---

## Fundamental Theorem of Calculus

**Part 1:** $\dfrac{d}{dx}\left[\displaystyle\int_a^x f(t)\,dt\right] = f(x)$

**Part 2:** $\displaystyle\int_a^b f(x)\,dx = F(b)-F(a)$, where $F'=f$

---

## Integration Techniques

**$u$-substitution:** $\displaystyle\int f(g(x))g'(x)\,dx = \int f(u)\,du$

**Integration by Parts:** $\displaystyle\int u\,dv = uv-\int v\,du$

**Trig identities for integration:**
$$\sin^2x=\frac{1-\cos2x}{2} \qquad \cos^2x=\frac{1+\cos2x}{2}$$

**Trig substitution patterns:**

| Expression | Substitute |
|---|---|
| $\sqrt{a^2-x^2}$ | $x=a\sin\theta$ |
| $\sqrt{a^2+x^2}$ | $x=a\tan\theta$ |
| $\sqrt{x^2-a^2}$ | $x=a\sec\theta$ |

$$\int \sec\theta\,d\theta = \ln|\sec\theta+\tan\theta|+C$$

**Partial fractions:** $\dfrac{P(x)}{(x-a)(x-b)} = \dfrac{A}{x-a}+\dfrac{B}{x-b}$; for a repeated factor $(x-a)^2$, include both $\dfrac{A}{x-a}$ and $\dfrac{B}{(x-a)^2}$.

---

## Improper Integrals

$$\int_a^\infty f(x)\,dx = \lim_{b\to\infty}\int_a^b f(x)\,dx$$

For a discontinuity at $x=a$: $\displaystyle\int_a^b f(x)\,dx = \lim_{t\to a^+}\int_t^b f(x)\,dx$

**p-integral reference:** $\displaystyle\int_1^\infty \frac{dx}{x^p}$ converges iff $p>1$. $\displaystyle\int_0^1 \frac{dx}{x^p}$ converges iff $p<1$.

---

## L'Hôpital's Rule

If $\displaystyle\lim_{x\to a}\frac{f(x)}{g(x)}$ is $\dfrac00$ or $\dfrac{\infty}{\infty}$:
$$\lim_{x\to a}\frac{f(x)}{g(x)} = \lim_{x\to a}\frac{f'(x)}{g'(x)}$$

---

## Exponential Change

$$\frac{dy}{dt}=ky \implies y=y_0e^{kt}$$

Newton's Law of Cooling: $T(t) = T_s+(T_0-T_s)e^{-kt}$
