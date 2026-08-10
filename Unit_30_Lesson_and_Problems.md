# Unit 30: Inverse Functions and Their Derivatives

## 1. The idea, in plain words

A function takes an input and produces an output. An **inverse function undoes that** — it takes the output and hands you back the original input. If $f$ turns $3$ into $7$, then $f^{-1}$ turns $7$ back into $3$.

**A crucial warning right up front: $f^{-1}(x)$ does NOT mean $\dfrac{1}{f(x)}$.** This is probably the single most common misconception with inverse functions — the "$-1$" here is *not* an exponent. It's just notation meaning "the inverse function," a completely different function from $f$ itself.

**Picture it like undoing a set of instructions.** If $f$ says "double the number, then add 3," the inverse has to undo those steps in reverse order: "subtract 3, then divide by 2." **Finding an inverse algebraically works the exact same way:** write $y=f(x)$, then swap the roles of $x$ and $y$ (since input and output are trading places), and solve for $y$ again. Whatever you get is $f^{-1}(x)$.

**Not every function has an inverse.** A function only has an inverse if it's **one-to-one** — meaning every output comes from exactly one input (no two different $x$-values ever produce the same $y$-value). A function that's always increasing, or always decreasing, across its whole domain automatically qualifies (it can't ever repeat an output).

**The real payoff of this unit — the Inverse Function Derivative formula.** Sometimes finding an explicit formula for $f^{-1}(x)$ is difficult or flat-out impossible (imagine trying to solve a complicated cubic or a fifth-degree polynomial for $x$ in terms of $y$). The wonderful news: **you can still find the derivative of the inverse at a specific point, without ever writing down the inverse function itself** — just using facts about the *original* function $f$.

## 2. Toolbox

**Finding an inverse algebraically:**

1. Write $y=f(x)$.
2. Swap $x$ and $y$.
3. Solve the new equation for $y$.
4. That result is $f^{-1}(x)$.

**Verifying two functions are inverses of each other:**
$$f\big(f^{-1}(x)\big) = x \qquad \text{and} \qquad f^{-1}\big(f(x)\big) = x$$

**One-to-one requirement:** $f$ has an inverse only if it's one-to-one. A function that is strictly increasing ($f'(x)>0$ everywhere) or strictly decreasing ($f'(x)<0$ everywhere) on its domain is automatically one-to-one.

**The Inverse Function Derivative formula** — the star of this unit:
$$\big(f^{-1}\big)'(a) = \frac{1}{f'\big(f^{-1}(a)\big)}$$

**In plain words:** to find the derivative of the inverse at the point $a$, first figure out **which input of $f$ produces the output $a$** (that input is $f^{-1}(a)$), then take the reciprocal of $f'$ evaluated at *that* input.

**A convenient way to organize this when you're given $f(p)=a$ directly:** since $f^{-1}(a)=p$,
$$\big(f^{-1}\big)'(a) = \frac{1}{f'(p)}$$

## 3. Common mistakes

- **Confusing $f^{-1}(x)$ with $\dfrac{1}{f(x)}$.** These are completely different things — always keep this distinction sharp.
- **Forgetting to swap $x$ and $y$ before solving**, when finding an inverse explicitly — solving for $y$ without swapping just gives you back the original function.
- **Applying the derivative formula with the wrong input.** The formula needs $f'$ evaluated at $f^{-1}(a)$ — that is, at whatever input of $f$ produces the output $a$ — not at $a$ itself.
- **Forgetting to first identify $f^{-1}(a)$** before plugging into the formula. If you're given that $f(p)=a$, then $f^{-1}(a)=p$ — use that $p$-value inside $f'(\cdot)$.
- **Assuming every function has an inverse.** Always check (or be told) that $f$ is one-to-one before treating $f^{-1}$ as a legitimate function.

## 4. Problem Set

### 🟢 Warm-up

1. Find $f^{-1}(x)$ for $f(x)=2x+3$.
2. Find $f^{-1}(x)$ for $f(x)=5x-2$.
3. Find $f^{-1}(x)$ for $f(x)=4x$.
4. Find $f^{-1}(x)$ for $f(x)=\dfrac{x}{2}+1$.
5. Verify that $f(x)=3x-6$ and $g(x)=\dfrac{x+6}{3}$ are inverses of each other by checking that $f(g(x))=x$.
6. Find $f^{-1}(x)$ for $f(x)=-2x+7$.

### 🟡 Standard

7. Find $f^{-1}(x)$ for $f(x)=x^3$.
8. Find $f^{-1}(x)$ for $f(x)=\sqrt{x-2}$, $x\ge2$, and state the domain of the inverse.
9. Find $f^{-1}(x)$ for $f(x)=x^2+3$, $x\ge0$.
10. Given $f(x)=2x+1$: (a) find $f^{-1}(x)$ explicitly and differentiate it directly; (b) use the Inverse Function Derivative formula instead. Confirm both methods agree.
11. Given $f(x)=x^3$, use the Inverse Function Derivative formula to find $(f^{-1})'(8)$ — without finding a general formula for $f^{-1}(x)$.
12. Given $f(x)=x^2+1$ for $x\ge0$, with $f(2)=5$, use the Inverse Function Derivative formula to find $(f^{-1})'(5)$.

### 🔴 Challenge

13. Given $f(x)=6x-1$, find the inverse $f^{-1}$ of $f(x)$.
14. Let $f(x)=x^3+x^2+6x+1$, $x\ge0$. Find the value of $\dfrac{d(f^{-1})}{dx}$ at the point $a=1=f(0)$.
15. Given $f(x)=x^5+2x+1$, explain why finding $f^{-1}(x)$ explicitly would be extremely difficult. Then, using the fact that $f(1)=4$, use the Inverse Function Derivative formula to find $(f^{-1})'(4)$.
16. Given $f(x)=x^3+x$: first verify that $f$ is one-to-one, then find $(f^{-1})'(2)$, given that $f(1)=2$.
17. Given $f(x)=2x^5+x^3+1$, and knowing $f(1)=4$, find $(f^{-1})'(4)$.

### 🌍 Applied

18. A temperature conversion function $f(C)=1.8C+32$ converts Celsius to Fahrenheit. Find $f^{-1}(F)$ (converting Fahrenheit back to Celsius), and use it to convert $98.6°F$ to Celsius.
19. A company's cost to produce $x$ units is $C(x)=50x+200$ dollars. Find the inverse function (giving the number of units producible for a given budget), and use it to find how many units can be produced with a budget of $\$1200$.
20. A demand function relating price to quantity is $p(q)=100-2q$. Find the inverse function $q(p)$, and briefly interpret what it represents.
21. A rocket's height (in meters) as a function of fuel burned (in tons) is modeled by $h(x)=x^3+2x$ for $x\ge0$, with $h(2)=12$. Use the Inverse Function Derivative formula to find $(h^{-1})'(12)$, and interpret what this value represents physically.
