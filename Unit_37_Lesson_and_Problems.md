# Unit 37: Integration by Parts

## 1. The idea, in plain words

Substitution (Unit 28) handles integrals built from the chain rule. **Integration by parts is the tool for integrals built from the product rule** — specifically, for integrals where two very different *kinds* of functions are multiplied together, like a polynomial times a trig function, or a polynomial times $\ln x$.

**Where the formula comes from:** recall the product rule, $\dfrac{d}{dx}[uv] = u'v+uv'$. Rearranging and integrating both sides eventually gives you:
$$\int u\,dv = uv - \int v\,du$$

**Picture the whole idea like a trade.** You're not directly integrating the original product — you're trading it for a *different* integral, $\int v\,du$, hoping that new integral is easier to handle than the one you started with. The entire skill of this unit is picking a good trade: choosing which factor becomes "$u$" (the piece you differentiate) and which becomes "$dv$" (the piece you integrate).

**A simple guideline for choosing $u$ — remember "LIATE":** given a choice, prefer to let $u$ be whichever type of function appears **earliest** in this list: **L**ogarithmic, **I**nverse trig, **A**lgebraic (polynomials), **T**rig, **E**xponential. The idea is that $u$ should be the piece that gets *simpler* when you differentiate it (like $\ln x$ turning into $\frac1x$, or $x^2$ turning into $2x$), while $dv$ should be the piece that's easy to integrate no matter what (like $e^x$ or $\cos x$, which don't get more complicated).

**One more trick you'll need almost immediately: what if there's only one function, not two?** Something like $\int \ln x\,dx$ or $\int \arctan x\,dx$ doesn't look like a product at all — there's no obvious second factor to split off. The move: invent one. Rewrite it as $\int 1\cdot\ln x\,dx$, then let $u=\ln x$ and $dv=1\,dx$ (so $v=x$). Multiplying by an invisible "$1$" turns a lone function into a product you can attack normally — this exact move shows up constantly for standalone logs and inverse trig functions.

**Sometimes you'll need to repeat the whole process** if the new integral $\int v\,du$ is still a product needing its own round of integration by parts (this happens with things like $x^2e^x$).

**A genuinely surprising special case: "cyclic" integrals.** For something like $\int e^x\cos x\,dx$, applying integration by parts twice actually brings back the *original* integral on the other side of the equation — at which point you solve for it algebraically, the same way you'd solve $I = 5 - I$ for $I$.

## 2. Toolbox

**Integration by Parts formula:**
$$\int u\,dv = uv - \int v\,du$$

**The procedure:**

1. Identify $u$ and $dv$ from the integrand (use LIATE as a guide for choosing $u$).
2. Compute $du$ (the derivative of $u$) and $v$ (the antiderivative of $dv$).
3. Plug into the formula: $uv - \int v\,du$.
4. Evaluate the new integral $\int v\,du$ — sometimes directly, sometimes with another substitution, and sometimes with a second round of integration by parts.
5. Add $+C$ at the very end (only once, on the final result).

**For a "cyclic" integral** (where the original integral reappears after two rounds): treat the whole equation algebraically — move all copies of the original integral to one side, factor, and divide to solve for it.

## 3. Common mistakes

- **Choosing $u$ and $dv$ poorly**, so that the new integral $\int v\,du$ is *harder* than the one you started with. If this happens, try swapping your choice of $u$ and $dv$.
- **Forgetting the minus sign in the formula.** It's $uv - \int v\,du$, not $uv+\int v\,du$.
- **Losing track of signs during a repeated or cyclic application.** These problems often stack up several negative signs — go slowly and double-check each step.
- **Stopping a cyclic integral partway through, expecting it to resolve normally.** If the original integral reappears, that's the signal to solve for it algebraically, not a sign that something went wrong.
- **Forgetting a constant factor when finding $v$** — for instance, if $dv=\cos(3x)\,dx$, then $v=\frac13\sin(3x)$, not just $\sin(3x)$.
- **Adding $+C$ too early**, or adding it more than once during a multi-step problem — it only belongs on the very final answer.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\int x\cos x\,dx$
2. $\displaystyle\int xe^{2x}\,dx$
3. $\displaystyle\int x\sin(2x)\,dx$
4. $\displaystyle\int \ln x\,dx$
5. $\displaystyle\int (x+1)e^x\,dx$
6. $\displaystyle\int xe^{-x}\,dx$

### 🟡 Standard

7. $\displaystyle\int x\sin x\,dx$
8. $\displaystyle\int x^5\ln x\,dx$
9. $\displaystyle\int x^2e^x\,dx$ (this one needs two rounds!)
10. $\displaystyle\int \ln(x^2)\,dx$
11. $\displaystyle\int x\cos(3x)\,dx$
12. $\displaystyle\int \arctan(x)\,dx$
13. $\displaystyle\int x^3\ln x\,dx$

### 🔴 Challenge

14. $\displaystyle\int xe^x\,dx$
15. $\displaystyle\int e^x\cos x\,dx$ (a cyclic integral!)
16. $\displaystyle\int e^{2x}\sin x\,dx$ (another cyclic integral)
17. $\displaystyle\int x^2\sin x\,dx$ (two rounds needed)
18. $\displaystyle\int x(\ln x)^2\,dx$ (two rounds needed)

### 🌍 Applied

19. A variable force is modeled by $F(x)=x\sin x$ (newtons). Find the total work done, $\displaystyle\int_0^\pi x\sin x\,dx$.
20. A continuous income stream has a present-value rate of $te^{-t}$. Find the total present value, $\displaystyle\int_0^{10} te^{-t}\,dt$.
21. Find $\displaystyle\int_1^e x\ln x\,dx$.
22. Find $\displaystyle\int_0^{\pi/2} x\cos x\,dx$.
