# Unit 10: Product Rule & Quotient Rule

## 1. The idea, in plain words

Here's a trap almost everyone falls into at first: if $y = f(x)\cdot g(x)$, it feels natural to guess that $y' = f'(x)\cdot g'(x)$ — just differentiate each piece and multiply. **This is wrong**, and it's worth seeing why with a quick sanity check: let $f(x)=x^2$ and $g(x)=x^3$, so $f(x)g(x)=x^5$. We already know $\frac{d}{dx}[x^5]=5x^4$. But $f'(x)g'(x) = (2x)(3x^2) = 6x^3$ — completely different! Multiplication and differentiation just don't "distribute" over each other like that.

**Product Rule, in plain words:** when you differentiate a product of two functions, you have to give each function a turn "holding still" while the other one gets differentiated, and then add the two results together. Think of it like a relay race: first, differentiate the first runner while the second one holds their exact position; then swap — differentiate the second runner while the first one holds still. Add both legs of the race together, and that's your answer.

**Quotient Rule, in plain words:** dividing is trickier than multiplying, so the rule looks a little more involved — but it follows a similar "each one gets a turn" idea, with one extra twist: **order matters** (unlike the product rule, where addition doesn't care about order), and you also divide by the denominator squared at the end. A popular memory chant for this is: **"low-dee-high minus high-dee-low, over low-low"** — where "low" means the denominator and "high" means the numerator, and "dee" means "the derivative of."

**An important strategic skill this unit adds:** sometimes it's actually *easier* to simplify first (expand a product, or split apart a quotient with a simple monomial denominator, like you practiced in Unit 9) rather than reaching for these rules at all. Part of getting good at this is learning to recognize which situation you're in.

## 2. Toolbox

**Product Rule:**
$$\frac{d}{dx}\big[f(x)\cdot g(x)\big] = f'(x)\cdot g(x) + f(x)\cdot g'(x)$$

**Quotient Rule:**
$$\frac{d}{dx}\left[\frac{f(x)}{g(x)}\right] = \frac{f'(x)\cdot g(x) - f(x)\cdot g'(x)}{\big[g(x)\big]^2}$$

**Memory chant for the quotient rule:** "low-dee-high minus high-dee-low, over low-low" — i.e., $\dfrac{\text{(denom)}\cdot(\text{deriv. of numer}) - (\text{numer})\cdot(\text{deriv. of denom})}{(\text{denom})^2}$.

**When to simplify instead of using the rule:** if a "product" is really just two simple polynomials that would be easy to expand and combine, or if a "quotient" has a single monomial in the denominator (like $\dfrac{x^2+4}{x}$), it's often faster to simplify completely first and then just use the power rule term by term. Save the product/quotient rule for cases where the pieces genuinely can't be combined that way.

## 3. Common mistakes

- **The #1 mistake: treating $(fg)'$ as $f'g'$.** Multiplication and differentiation do not commute — you must use the full product rule, every time.
- **Forgetting that order matters in the quotient rule.** Unlike addition in the product rule, subtraction cares about order: it's "derivative of the top times the bottom, MINUS the top times derivative of the bottom" — flipping this order gives you the wrong sign.
- **Forgetting to square the denominator at the end of the quotient rule.**
- **Forgetting to rewrite a fraction like $\dfrac{1}{x}$ as $x^{-1}$ before finding its derivative**, when it's tucked inside one of the factors in a product.
- **Reaching for the product or quotient rule when simple algebra would be faster.** Always glance first: could I just expand this, or divide term-by-term, before doing anything else?
- **Sign errors when distributing a negative sign through the numerator of a quotient-rule result.** Take an extra beat to expand carefully before combining like terms.

## 4. Problem Set

### 🟢 Warm-up

1. $y=(x^2)(x+3)$
2. $y=(2x+1)(x-4)$
3. $y=(x^2+1)(x-2)$
4. $y=\dfrac{x+1}{x-1}$
5. $y=\dfrac{3x-2}{x+5}$
6. $y=\dfrac{x^2}{x+1}$
7. $y=(x-3)(x^2+2)$

### 🟡 Standard

8. $y=(x^2+1)\left(x+1+\dfrac{1}{x}\right)$
9. $y=\dfrac{x+5}{3x+2}$
10. $y=\dfrac{x^2-3}{2x+1}$
11. $y=(x+2)(x^2-3x+1)$
12. $y=\left(\dfrac{1}{x}\right)(x^2+4)$
13. $y=\dfrac{2x-1}{x^2+3}$
14. $y=(x^2+x)(3-x)$

### 🔴 Challenge

15. $y = \dfrac{(x^2+x)(x^2-x+1)}{x^4}$
16. $y = \sqrt{x}\,(x^2-1)$
17. $y = \dfrac{x^2-4}{\sqrt{x}}$
18. $y = \left(x+\dfrac{1}{x}\right)(x^2-2)$
19. $y = \dfrac{x^3-1}{x^2+1}$
20. Find the equation of the tangent line to $y=(2x-1)(x+3)$ at $x=1$.

### 🌍 Applied

21. A company sets a price per unit of $p(x) = 50-0.5x$ dollars when selling $x$ units, so total revenue is $R(x)=x\cdot p(x)$. Find the marginal revenue function $R'(x)$ using the product rule, then evaluate $R'(10)$.
22. A company's total cost (in dollars) to produce $x$ units is $C(x)=x^2+20x+100$. The average cost per unit is $\bar{A}(x) = \dfrac{C(x)}{x}$. Find $\bar{A}'(x)$, then evaluate $\bar{A}'(5)$.
23. A city's population is modeled by $P(t)=t^2+5t$ (in thousands) and its developed area is modeled by $A(t)=t+2$ (in square miles), $t$ years from now. The population density is $D(t) = \dfrac{P(t)}{A(t)}$. Find $D'(t)$ using the quotient rule, then evaluate $D'(3)$.
24. A store sells $(x+10)$ units at a price of $(50-2x)$ dollars each, so total revenue is $N(x)=(x+10)(50-2x)$. Find $N'(x)$ using the product rule, then evaluate $N'(5)$.
