# Unit 7: Tangent Lines and the Derivative at a Point

## 1. The idea, in plain words

Back in Unit 1, you already did the hard work: sliding a secant line closer and closer until it became a tangent line, using a limit. This unit gives that number a name and a symbol, and hands you a second way to compute it.

**The name and the symbol:** the slope of the tangent line to $f$ at the point $x=a$ is called **"the derivative of $f$ at $a$,"** written $f'(a)$ (say it "f prime of a"). It's just one single number — the slope at that one specific point. It also equals the **instantaneous rate of change** of $f$ at $x=a$, exactly like we discussed in Unit 1.

**Two equivalent ways to compute it:** you already know the first one from Unit 1 — sneak up on $a$ using a tiny step $h$. There's a second, completely equivalent way that instead lets $x$ itself sneak up on $a$ directly. Think of it like two different paths up the same mountain — they get you to the exact same number, and you can pick whichever one is more convenient for a given problem (the second one is often nicer when the function has nice factoring, since $x-a$ becomes something you can cancel directly).

**A new question this unit adds:** does $f'(a)$ always exist? Not always! If the graph has a sharp corner, a cusp, or a break at $x=a$, there's no single well-defined tangent line there, and $f'(a)$ fails to exist. We call this "not differentiable at $a$." You'll learn to recognize this by checking whether the left-approach and right-approach versions of the limit agree — exactly the same idea as one-sided limits from Unit 4, just applied to the difference quotient instead of to $f(x)$ directly.

## 2. Toolbox

**Definition (Version 1 — the $h$ form, from Unit 1):**
$$f'(a) = \lim_{h\to 0} \frac{f(a+h)-f(a)}{h}$$

**Definition (Version 2 — the $x$ form, new this unit):**
$$f'(a) = \lim_{x\to a} \frac{f(x)-f(a)}{x-a}$$

These give the exact same number — they're just two different ways of writing "sneak up on $a$." (If you set $x = a+h$, then $h = x-a$, and as $h\to 0$, $x\to a$ — same limit, different letters.)

**Tangent line at $x=a$:**
$$y - f(a) = f'(a)(x-a)$$

**Normal line at $x=a$** (perpendicular to the tangent, slope $-\dfrac{1}{f'(a)}$):
$$y - f(a) = -\frac{1}{f'(a)}(x-a)$$

**Differentiability:** $f'(a)$ exists only if the left-hand and right-hand versions of the difference-quotient limit **agree**. If they disagree (like a sharp corner), $f$ is **not differentiable** at $a$, even if $f$ is perfectly continuous there.

## 3. Common mistakes

- **Forgetting $f'(a)$ is just one number, tied to one specific point $a$.** It's not yet "a formula for any $x$" — that generalization comes in the next unit.
- **Forgetting to simplify before plugging in, when using the $x$-form.** Plugging $x=a$ straight into $\dfrac{f(x)-f(a)}{x-a}$ gives $\frac{0}{0}$ — you must factor and cancel the $(x-a)$ first, exactly like the $\frac{0}{0}$ fix-it kit from Unit 2.
- **Assuming continuity means differentiability.** A function can be continuous (no breaks) but still have a sharp corner, where the derivative doesn't exist. Always check both sides of the difference quotient separately if you suspect a corner.
- **Sign errors with the normal line.** The normal slope is $-\dfrac{1}{f'(a)}$, not $-f'(a)$.
- **Algebra slips expanding $(a+h)^2$, $(a+h)^3$, or factoring $x^2-a^2$-type expressions.** Slow down and write out every term.

## 4. Problem Set

### 🟢 Warm-up

1. Let $f(x) = x^2+5x$. Use the definition of the derivative to find $f'(1)$.
2. Let $f(x) = 3x^2-2$. Find $f'(0)$.
3. Let $f(x) = -x^2+4x$. Find $f'(2)$.
4. Let $f(x) = 5x-x^2$. Find $f'(-1)$.
5. Let $f(x) = 2x^2+3$. Find $f'(3)$.
6. Let $f(x) = x^2-1$. Find $f'(-2)$.

### 🟡 Standard

7. Using the **$x$-form** of the definition, $f'(a)=\displaystyle\lim_{x\to a}\frac{f(x)-f(a)}{x-a}$, find $f'(1)$ for $f(x) = -2x^2$.
8. Using the $x$-form of the definition, find $f'(3)$ for $f(x) = x^2-4x$.
9. Let $f(x) = x^2+1$. Using the $x$-form of the definition, find $f'(1)$, then write the equation of both the tangent line **and** the normal line at $(1,2)$.
10. Let $f(x) = 3x^2-x$. Find $f'(2)$, then write the equation of the tangent line at that point.
11. Let $f(x) = -x^2+2x+1$. Find $f'(0)$, then write the equation of the tangent line at that point.
12. Let $f(x) = 2x^2-5x$. Find $f'(1)$, then write the equations of both the tangent line and the normal line at that point.

### 🔴 Challenge

13. Let $f(x) = \dfrac{1}{x+1}$. Use the definition to find $f'(1)$.
14. Let $f(x) = \sqrt{x+5}$. Use the definition to find $f'(4)$. (You'll need the conjugate trick from Unit 1/2.)
15. Let $f(x) = x^3-x$. Use the $x$-form of the definition to find $f'(-1)$. (You'll need to factor a cubic expression.)
16. Show that $f(x)=|x-2|$ is **not differentiable** at $x=2$, by computing the left-hand and right-hand versions of the difference-quotient limit separately and showing they disagree.
17. Let $f(x) = \begin{cases} x^2, & x<1 \\ 2x-1, & x\ge 1\end{cases}$. Determine whether $f$ is differentiable at $x=1$ by computing the left-hand and right-hand difference-quotient limits. (This function should look familiar from an earlier unit — you already confirmed it's continuous there.)

### 🌍 Applied

18. A ball's height in meters after $t$ seconds is $h(t) = -5t^2+30t$. Use the definition of the derivative to find $h'(1)$, and explain what this number means physically.
19. A company's total cost (in dollars) to produce $x$ units is $C(x) = 0.5x^2+10x$. Find $C'(4)$ using the definition, and explain what this number means in terms of cost.
20. A town's population $t$ years from now is modeled by $P(t) = t^2+50t$. Find $P'(3)$ using the definition, and explain what it tells you about the population's growth at that moment.
21. An object's position in meters after $t$ seconds is $s(t) = 4t^2-2t$. Find $s'(2)$ using the definition, and explain what this number represents physically.
