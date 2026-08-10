# Unit 34: Indeterminate Forms and L'Hôpital's Rule

## 1. The idea, in plain words

Back in Unit 2, you learned the "$\frac{0}{0}$ fix-it kit" — factor and cancel, or rationalize, to dodge a dead-end limit. This unit hands you a much more powerful tool that works even when factoring is impossible: **L'Hôpital's Rule.**

**Here's the surprising fact at the heart of it:** if a limit of the form $\dfrac{f(x)}{g(x)}$ comes out to $\dfrac{0}{0}$ (or $\dfrac{\infty}{\infty}$) when you plug in the target value, you can **replace the numerator and denominator with their own separate derivatives**, and the limit of that *new* fraction will be exactly the same as the original limit. Keep doing this — differentiate top and bottom separately — until the indeterminate form finally clears up into something you can just plug straight into.

**Picture why this makes sense:** near the point in question, both the top and bottom of the fraction are shrinking toward zero (or blowing up toward infinity) together. What actually matters for the *limit* isn't their sizes — it's how *fast* each one is changing right at that instant. That's precisely what a derivative measures. So comparing their derivatives is like comparing their "closing speeds" instead of comparing two numbers that are both stuck at zero.

**A critical warning before you dive in:** L'Hôpital's Rule only applies when the limit is genuinely indeterminate — specifically $\dfrac00$ or $\dfrac{\infty}{\infty}$. **If you plug in the value and get an ordinary number (even something like $\dfrac{3}{1}$), stop — just report that number as the answer.** Applying the rule to a non-indeterminate limit doesn't just waste effort, it can actually produce the wrong answer.

**Another crucial warning: L'Hôpital's Rule is NOT the quotient rule.** You are differentiating the numerator and denominator **completely separately** — you do not combine them into one single derivative using the quotient rule formula. That would be solving a totally different problem.

## 2. Toolbox

**L'Hôpital's Rule:** if $\displaystyle\lim_{x\to a}\frac{f(x)}{g(x)}$ produces the indeterminate form $\dfrac00$ or $\dfrac{\infty}{\infty}$, and $f,g$ are differentiable near $a$, then
$$\lim_{x\to a}\frac{f(x)}{g(x)} = \lim_{x\to a}\frac{f'(x)}{g'(x)}$$
(provided the limit on the right exists, or is $\pm\infty$).

**The procedure:**

1. Plug in the target value. Confirm you genuinely get $\dfrac00$ or $\dfrac{\infty}{\infty}$ — if not, stop and just report the direct answer.
2. Differentiate the numerator and denominator **separately** (not with the quotient rule).
3. Take the limit of this new fraction.
4. If it's still indeterminate, repeat the process — apply L'Hôpital again on the new fraction.
5. If it's no longer indeterminate, plug in and report the answer.

**Recognizing $\dfrac{\infty}{\infty}$ forms:** these work exactly the same way as $\dfrac00$ forms — differentiate top and bottom separately, and check the new limit.

## 3. Common mistakes

- **Applying L'Hôpital's Rule to a limit that isn't actually indeterminate.** Always check first — if plugging in gives you a normal finite number over a nonzero number, that number *is* the answer; don't touch the derivative.
- **Confusing L'Hôpital's Rule with the quotient rule.** You differentiate the top and bottom *independently*, each on its own — you never combine them into a single derivative expression.
- **Stopping after one application when the result is still indeterminate.** Always re-check the new fraction — sometimes you need to apply the rule two or even three times before it resolves.
- **Forgetting basic limits you already know how to compute directly** (like recognizing $\lim_{x\to0}\frac{\sin x}{x}=1$) and reaching for L'Hôpital unnecessarily when a quicker method is available — not wrong, just slower.
- **Losing track of algebra when a limit is a product of two things both going to $0$ (a "$0\times\infty$" style setup in disguise).** Sometimes it's easier to split the limit into two separate, recognizable pieces (using limit laws) rather than brute-forcing repeated derivatives on a tangled product.

## 4. Problem Set

### 🟢 Warm-up

1. $\displaystyle\lim_{x\to2}\frac{x^2-4}{x-2}$
2. $\displaystyle\lim_{x\to0}\frac{\sin x}{x}$
3. $\displaystyle\lim_{x\to0}\frac{e^x-1}{x}$
4. $\displaystyle\lim_{x\to3}\frac{x^2-9}{x-3}$
5. $\displaystyle\lim_{x\to0}\frac{1-\cos x}{x}$
6. $\displaystyle\lim_{x\to1}\frac{x^3-1}{x-1}$

### 🟡 Standard

7. $\displaystyle\lim_{x\to\infty}\frac{3x^2+2x}{5x^2-1}$
8. $\displaystyle\lim_{x\to0}\frac{x^2+3}{x+1}$ (check carefully whether this is actually indeterminate before doing anything!)
9. $\displaystyle\lim_{x\to0}\frac{\tan x}{x}$
10. $\displaystyle\lim_{x\to\infty}\frac{\ln x}{x}$
11. $\displaystyle\lim_{x\to0}\frac{e^{2x}-1}{3x}$
12. $\displaystyle\lim_{x\to\pi}\frac{\sin x}{x-\pi}$

### 🔴 Challenge

13. $\displaystyle\lim_{x\to1}\frac{x^3-1}{4x^3-x-3}$
14. $\displaystyle\lim_{t\to0}\frac{\sin(t^2)}{t^2}$
15. $\displaystyle\lim_{x\to1}\frac{x-1}{\ln x - \sin(\pi x) + x - 1}$
16. $\displaystyle\lim_{x\to0}\frac{\tan^2x(1-\cos x)}{x^4}$
17. $\displaystyle\lim_{x\to0}\frac{x-\sin x}{x^3}$

### 🌍 Applied

18. Show, using L'Hôpital's Rule, that $\displaystyle\lim_{t\to a}\frac{t^2-a^2}{t-a} = 2a$, and explain how this confirms the derivative of $f(t)=t^2$ at $t=a$.
19. For $C(x)=x^2+3x$, evaluate $\displaystyle\lim_{x\to0}\frac{C(x)-C(0)}{x}$, and confirm it matches $C'(0)$.
20. Show, using L'Hôpital's Rule, that $\displaystyle\lim_{t\to0}\frac{1-e^{-kt}}{t} = k$.
21. Find $\displaystyle\lim_{x\to0}\frac{\sin(3x)}{\sin(5x)}$.
