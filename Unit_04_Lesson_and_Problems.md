# Unit 4: One-Sided Limits

## 1. The idea, in plain words

So far we've asked "what does $f(x)$ approach as $x$ gets close to $a$?" — sneaking up on $a$ from *both* directions at once. But sometimes a function behaves differently depending on which side you sneak up from. **One-sided limits** let us check each direction separately.

**Picture it:** imagine walking along a graph toward a certain $x$-value, $a$.

- If you're walking in from the **left** (from smaller $x$-values, heading up toward $a$), the height you're approaching is called the **left-hand limit**, written $\displaystyle\lim_{x\to a^-} f(x)$.
- If you're walking in from the **right** (from larger $x$-values, heading down toward $a$), the height you're approaching is called the **right-hand limit**, written $\displaystyle\lim_{x\to a^+} f(x)$.

Most of the time — for nice smooth curves — it doesn't matter which side you approach from; you land at the same height either way. But **piecewise functions** (functions built out of different formulas glued together at a breakpoint) can behave very differently on the two sides. Imagine a staircase: walking up to a step from the left, you're at one height; stepping in from the right, you might be at a completely different height. In that case, there's no single "the limit" — the two sides disagree.

**The big rule:** the ordinary (two-sided) limit only exists if *both* one-sided limits exist *and* agree with each other. If they don't match, we say the limit "does not exist" (DNE) at that point.

**Important reminder:** a limit only cares about what $f(x)$ is doing *near* $a$ — it does not care what $f(a)$ itself equals, or even whether $f$ is defined at $a$ at all. Don't let the actual value at the point distract you from what the function is approaching.

## 2. Toolbox

**Left-hand limit:** consider only $x$-values slightly *less than* $a$.
$$\lim_{x\to a^-} f(x)$$

**Right-hand limit:** consider only $x$-values slightly *greater than* $a$.
$$\lim_{x\to a^+} f(x)$$

**Existence rule:**
$$\lim_{x\to a} f(x) = L \quad \Longleftrightarrow \quad \lim_{x\to a^-}f(x) = L \ \text{ and }\ \lim_{x\to a^+}f(x) = L$$

If the two one-sided limits are different numbers, the two-sided limit **does not exist**.

**For piecewise functions:** use whichever formula applies just *below* $a$ to compute the left-hand limit, and whichever formula applies just *above* $a$ to compute the right-hand limit. Then plug $a$ into each formula (direct substitution, or factor-and-cancel first if needed, same as Unit 2).

**For absolute value expressions**, remember:
$$|x-a| = \begin{cases} x-a, & x \ge a \\ -(x-a), & x < a \end{cases}$$
This is exactly why absolute value functions are a classic source of one-sided limit problems — the formula genuinely changes depending on which side you're on.

## 3. Common mistakes

- **Grabbing the wrong piece.** Always double check: which formula is valid for $x$-values *just below* $a$? Which one for *just above*? It's easy to grab the wrong one under time pressure.
- **Stopping after checking only one side.** To claim the two-sided limit exists, you must check *both* sides and confirm they match — don't skip the second side.
- **Confusing the limit with the function's actual value at $a$.** A piecewise function often defines a specific (sometimes weird) value right at the breakpoint — that value is irrelevant to the limit computation.
- **Forgetting the sign flip inside an absolute value.** For $x<a$, $|x-a|$ becomes $-(x-a)$, not $(x-a)$. Missing this sign flip is the most common error on these problems.
- **Arithmetic slips when plugging the breakpoint into each formula.** Take an extra moment — these are usually simple substitutions, so a careless error is the main risk, not the concept itself.

## 4. Problem Set

### 🟢 Warm-up

1. $f(x) = \begin{cases} x+1, & x<2 \\ 3x-1, & x\ge 2\end{cases}$ — Find $\displaystyle\lim_{x\to 2^-}f(x)$ and $\displaystyle\lim_{x\to 2^+}f(x)$. Does $\displaystyle\lim_{x\to 2}f(x)$ exist?

2. $f(x) = \begin{cases} x^2, & x<1 \\ 2x-1, & x\ge 1\end{cases}$ — Find both one-sided limits at $x=1$. Does the two-sided limit exist?

3. $f(x) = \begin{cases} 3, & x<0 \\ x+3, & x\ge 0\end{cases}$ — Find both one-sided limits at $x=0$. Does the two-sided limit exist?

4. $f(x) = |x|$ — Find $\displaystyle\lim_{x\to 0^-}f(x)$ and $\displaystyle\lim_{x\to 0^+}f(x)$. Does $\displaystyle\lim_{x\to 0}f(x)$ exist?

5. $f(x) = \begin{cases} 5-x, & x\le 3 \\ x-1, & x>3\end{cases}$ — Find both one-sided limits at $x=3$. Does the two-sided limit exist?

6. $f(x) = \begin{cases} 2x, & x<-1 \\ x^2, & x\ge -1\end{cases}$ — Find both one-sided limits at $x=-1$. Does the two-sided limit exist?

### 🟡 Standard

7. $f(x) = \begin{cases} 1-x^2, & x\ne 1 \\ 2, & x=1\end{cases}$ — Find $\displaystyle\lim_{x\to 1^-}f(x)$ and $\displaystyle\lim_{x\to 1^+}f(x)$. Does $\displaystyle\lim_{x\to 1}f(x)$ exist, and if so, what is it?

8. $f(x) = \begin{cases} x^2-4, & x\ne 2 \\ 5, & x=2\end{cases}$ — Find both one-sided limits at $x=2$. Does the two-sided limit exist?

9. $f(x) = \begin{cases} \dfrac{x^2-9}{x-3}, & x\ne 3 \\ 10, & x=3\end{cases}$ — Find $\displaystyle\lim_{x\to 3}f(x)$. How does it compare to $f(3)$?

10. $f(x) = \begin{cases} x+2, & x<0 \\ x^2+2, & x\ge 0\end{cases}$ — Find both one-sided limits at $x=0$. Does the two-sided limit exist?

11. $f(x) = \begin{cases} 3x+2, & x\le -2 \\ -x, & x>-2\end{cases}$ — Find both one-sided limits at $x=-2$. Does the two-sided limit exist?

12. $f(x) = \dfrac{|x-3|}{x-3}$ — Find $\displaystyle\lim_{x\to 3^-}f(x)$ and $\displaystyle\lim_{x\to 3^+}f(x)$. Does the two-sided limit exist?

### 🔴 Challenge

13. $f(x) = \begin{cases} x+3, & x<-1 \\ x^2-1, & -1\le x<2 \\ 2x-1, & x\ge 2\end{cases}$ — Find the one-sided limits at $x=-1$ and at $x=2$, and state whether the two-sided limit exists at each point.

14. $f(x) = \begin{cases} \dfrac{x^2-1}{x-1}, & x<1 \\ 3, & x=1 \\ 2x, & x>1\end{cases}$ — Find both one-sided limits at $x=1$. Does the two-sided limit exist, and how does it compare to $f(1)$?

15. $f(x) = \dfrac{x^2-4}{|x-2|}$ — Find $\displaystyle\lim_{x\to 2^-}f(x)$ and $\displaystyle\lim_{x\to 2^+}f(x)$. Does the two-sided limit exist?

16. Find the value of $k$ that makes $\displaystyle\lim_{x\to 3}f(x)$ exist, where $f(x) = \begin{cases} kx+1, & x<3 \\ x^2-2, & x\ge 3\end{cases}$.

17. Find the value of $c$ that makes $\displaystyle\lim_{x\to 2}f(x)$ exist, where $f(x) = \begin{cases} x^2+c, & x\le 2 \\ 3x-4, & x>2\end{cases}$.

### 🌍 Applied

18. A (hypothetical) simplified tax model says the tax owed, $T(x)$ dollars, on income $x$ (in thousands of dollars) is $T(x) = \begin{cases} 0.10x, & x\le 50 \\ 0.12x-1, & x>50\end{cases}$. Find $\displaystyle\lim_{x\to 50^-}T(x)$ and $\displaystyle\lim_{x\to 50^+}T(x)$. Does the limit exist at the bracket boundary — in other words, is there a sudden jump in tax owed right at $x=50$?

19. A shipping company charges $C(w) = \begin{cases} 5, & w\le 2 \\ 5+2(w-2), & w>2\end{cases}$ dollars for a package weighing $w$ pounds. Find both one-sided limits as $w\to 2$. Is there a jump in price right at the $2$-pound mark?

20. A parking garage charges a flat rate per hour-block: $P(h) = \begin{cases} 5, & 0<h\le 1 \\ 8, & 1<h\le 2 \\ 11, & 2<h\le 3\end{cases}$ dollars, where $h$ is hours parked. Find $\displaystyle\lim_{h\to 1^-}P(h)$ and $\displaystyle\lim_{h\to 1^+}P(h)$. Does the limit exist at $h=1$? What does that tell you about the price the instant you cross into a new hour?

21. A phone data plan costs $D(x) = \begin{cases} 30, & x\le 2 \\ 30+10(x-2), & x>2\end{cases}$ dollars for $x$ gigabytes used. Find both one-sided limits as $x\to 2$. Is there a sudden jump in cost right at the $2$ GB mark?
