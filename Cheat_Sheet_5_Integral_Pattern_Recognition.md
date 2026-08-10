# Cheat Sheet: Recognize the Integral at a Glance

*A fast lookup table for exam review. Pair this with "Which Integration Technique Do I Use?" if you want the full step-by-step reasoning behind any row.*

| If the integral looks like... | Use... | Quick example |
|---|---|---|
| $x^n$ (plain power of $x$) | Power Rule | $\displaystyle\int x^3\,dx$ |
| $\sin x$, $\cos x$, $e^x$, $\dfrac1x$ (basic function, plain $x$ inside) | Basic formula, direct | $\displaystyle\int e^{x}\,dx$ |
| $f(g(x))\cdot g'(x)$ — inner function's derivative sitting right there | $u$-substitution | $\displaystyle\int 2x(x^2+1)^3\,dx$ |
| Numerator = derivative of denominator | Quick $\ln$ shortcut (a special case of substitution) | $\displaystyle\int \frac{2x-6}{x^2-6x+8}\,dx$ |
| Polynomial $\times$ $\sin x$, $\cos x$, or $e^x$ | Integration by Parts | $\displaystyle\int x\sin x\,dx$ |
| Polynomial $\times$ $\ln x$, or $\ln x$ alone | Integration by Parts | $\displaystyle\int x^5\ln x\,dx$ |
| $e^x\sin x$ or $e^x\cos x$ | Integration by Parts, **twice**, then solve algebraically | $\displaystyle\int e^x\cos x\,dx$ |
| $\sin^m x\cos^n x$, same angle, at least one power odd | Trig Integral — peel off one factor, use $\sin^2+\cos^2=1$ | $\displaystyle\int \sin^3x\cos^2x\,dx$ |
| $\sin^m x\cos^n x$, same angle, both powers even | Trig Integral — power-reducing identities | $\displaystyle\int \sin^2x\cos^2x\,dx$ |
| $\sqrt{1\pm\cos(2x)}$ | Double-angle identity eliminates the root directly | $\displaystyle\int \sqrt{1+\cos2x}\,dx$ |
| $\sqrt{a^2-x^2}$, $\sqrt{a^2+x^2}$, or $\sqrt{x^2-a^2}$, nothing else going on | Basic $\arcsin$/$\arctan$ formula (or complete the square first) | $\displaystyle\int \frac{dx}{\sqrt{4-x^2}}$ |
| Same roots as above, but with extra polynomial factors or powers | Trig Substitution | $\displaystyle\int x^2\sqrt{9-x^2}\,dx$ |
| $\dfrac{P(x)}{Q(x)}$, factorable denominator, proper fraction | Partial Fractions | $\displaystyle\int \frac{2x+3}{(x-1)(x+2)}\,dx$ |
| $\dfrac{P(x)}{Q(x)}$, numerator degree $\ge$ denominator degree | Long division first, then handle the remainder | $\displaystyle\int \frac{x^3+3x^2+2x-7}{x+2}\,dx$ |
| An $\infty$ bound, or a vertical asymptote inside the interval | Improper Integral — replace the trouble spot with a limit | $\displaystyle\int_1^\infty \frac{dx}{x^2}$ |

---

## The single most useful habit

**Before matching a row above, always ask: can I simplify this algebraically first?** Expanding a product, dividing a fraction term-by-term, or applying a trig identity often turns a "hard-looking" integral into a one-line power-rule problem. Many of the trickiest-looking integrals in this course collapse dramatically once you simplify before hunting for a technique.
