# Unit 22: Newton's Method

## 1. The idea, in plain words

Sometimes an equation like $x^4-2=0$ has a real solution, but there's no clean algebra trick to solve for it exactly (try it — you can't just factor your way to the answer). **Newton's Method is a clever way to zero in on that solution numerically, getting closer and closer with each step, using nothing but tangent lines.**

**Picture it like this:** you make a rough first guess, $x_0$, for where the root (the place where the graph crosses the x-axis) might be. You're probably not exactly right — but you don't need to be. Draw the **tangent line** to the curve at your guess. Since the tangent line is straight, it's easy to find exactly where *it* crosses the x-axis — and that crossing point becomes your **new, improved guess**, $x_1$. Repeat the process at $x_1$ to get an even better guess $x_2$, and so on. Each round, your guess typically gets closer to the true root, often startlingly fast.

**Where the formula comes from:** the tangent line at $x_n$ is $y - f(x_n) = f'(x_n)(x-x_n)$. To find where this tangent line crosses the x-axis, set $y=0$ and solve for $x$ — that $x$ becomes your next guess, $x_{n+1}$. Working through that algebra gives you the Newton's Method formula directly.

## 2. Toolbox

**Newton's Method formula:**
$$x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}$$

**The procedure:**

1. Choose a starting guess $x_0$, ideally reasonably close to the actual root, and somewhere the derivative isn't zero.
2. Compute $f(x_0)$ and $f'(x_0)$.
3. Plug into the formula to get $x_1$.
4. To go further, repeat the same process using $x_1$ in place of $x_0$ to get $x_2$, and so on — each new guess uses the derivative evaluated at the *most recent* guess, not the original one.

**A quick sanity check on the formula:** if $f(x_n)$ is positive and $f'(x_n)$ is positive, the correction term is subtracted, moving your guess to the left — matching the picture of a tangent line sloping up crossing the axis to the left of where you are.

## 3. Common mistakes

- **Reusing $f'(x_0)$ for every iteration, instead of recomputing the derivative at the current guess each time.** Each new step needs $f'$ evaluated at the *most recent* $x$-value, not the original one.
- **Sign errors in the subtraction.** The formula is $x_n$ **minus** $\dfrac{f(x_n)}{f'(x_n)}$ — it's easy to accidentally add instead.
- **Stopping too early.** If a problem asks for $x_2$, you need to complete two full iterations — computing $x_1$ alone isn't enough.
- **Mixing up $f(x)$ and $f'(x)$ in the formula**, or dividing by the wrong one.
- **Rounding too aggressively partway through.** Carry several decimal places through your intermediate calculations, and only round your very final answer — early rounding can noticeably throw off later iterations.

## 4. Problem Set

For each problem, use Newton's Method to compute the requested iteration(s), starting from the given $x_0$.

### 🟢 Warm-up

1. $f(x)=x^2-2$, $x_0=1$. Find $x_1$.
2. $f(x)=x^2-5$, $x_0=2$. Find $x_1$.
3. $f(x)=x^3-2$, $x_0=1$. Find $x_1$.
4. $f(x)=x^2-10$, $x_0=3$. Find $x_1$.
5. $f(x)=x^3-8$, $x_0=3$. Find $x_1$.
6. $f(x)=x^2-7$, $x_0=3$. Find $x_1$.

### 🟡 Standard

7. $f(x)=x^2-3$, $x_0=2$. Find $x_1$ and $x_2$.
8. $f(x)=x^3-5$, $x_0=2$. Find $x_1$ and $x_2$.
9. $f(x)=x^2+x-6$, $x_0=1$. Find $x_1$ and $x_2$.
10. $f(x)=\cos x - x$, $x_0=1$ (radians). Find $x_1$.
11. $f(x)=x^3-x-1$, $x_0=1$. Find $x_1$ and $x_2$.
12. $f(x)=x^2-6$, $x_0=2$. Find $x_1$ and $x_2$.

### 🔴 Challenge

13. $f(x)=x^4-2$, $x_0=1$. Find $x_1$.
14. $f(x)=x^4-2$, $x_0=1$. Find $x_1$ **and** $x_2$.
15. $f(x)=x^5-3$, $x_0=1$. Find $x_1$ and $x_2$.
16. Explain what goes wrong with Newton's Method if you happen to choose a starting guess $x_0$ where $f'(x_0)=0$. Use the formula itself to justify your answer.
17. $f(x)=\sin x$, $x_0=3$ (radians). Find $x_1$ and $x_2$, and compare $x_2$ to the actual value of $\pi$.

### 🌍 Applied

18. Use Newton's Method to approximate $\sqrt7$ (i.e., find the positive root of $f(x)=x^2-7$), starting from $x_0=2.5$. Find $x_1$.
19. A company's break-even condition (cost minus revenue) is modeled by $f(x)=x^2-50x+200=0$. Use Newton's Method starting from $x_0=5$ to find $x_1$, an approximation of the lower break-even production level.
20. Find the root of $f(x)=x^3-2x-5$, starting from $x_0=2$. Find $x_1$ and $x_2$.
21. Use Newton's Method to approximate $\sqrt[3]{10}$ (i.e., find the positive root of $f(x)=x^3-10$), starting from $x_0=2$. Find $x_1$.
