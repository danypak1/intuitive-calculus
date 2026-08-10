# Unit 14: Implicit Differentiation

## 1. The idea, in plain words

Every function you've differentiated so far has had $y$ written all by itself on one side, like $y=x^2+3$. But some equations tangle $x$ and $y$ together in a way that's messy or even impossible to untangle — like $x^2y+xy^2=8$. You'd have a hard time solving that for "$y=$ (some formula in $x$)."

**Here's the trick: you don't have to.** You can differentiate *both sides of the equation, exactly as written*, term by term — you just have to remember one crucial extra rule: **whenever you differentiate something involving $y$, you must tack on a $\dfrac{dy}{dx}$ (also written $y'$), because $y$ is secretly a function of $x$, even though it's not written as "$y=\dots$."**

**Picture it like this:** imagine $y$ is a hidden, invisible function of $x$ — think of it as "$y(x)$" even though nobody bothered to write the "$(x)$" part. Every time you differentiate a $y$-term, the chain rule kicks in automatically, because you're really differentiating $y(x)$, not just plain $y$. The "inner function" is $y$ itself, and its derivative is $y'$ — so it tags along as a multiplier, just like in any other chain rule problem.

**The overall game plan:**

1. Differentiate both sides of the equation, term by term, with respect to $x$.
2. Every time you differentiate a $y$-term, remember to multiply by $y'$ (chain rule). Every time $x$ and $y$ are multiplied together, remember the product rule too.
3. After differentiating, you'll have an equation with some $y'$ terms mixed in with plain $x$ and $y$ terms. Gather *all* the $y'$ terms onto one side, and everything else onto the other side.
4. Factor out $y'$, then divide to solve for it by itself.

## 2. Toolbox

**The key extra rule:** whenever you differentiate a term with $y$ in it, multiply by $y'=\dfrac{dy}{dx}$, since $y$ stands for a function of $x$:
$$\frac{d}{dx}\big[y^n\big] = n\,y^{n-1}\cdot y'$$

**Product rule still applies** whenever $x$ and $y$ are multiplied together (like $xy$ or $x^2y$):
$$\frac{d}{dx}[xy] = y + x\cdot y' \qquad \frac{d}{dx}\big[x^2y\big] = 2xy + x^2y'$$

**Trig and other chain-rule versions work the same way, with $y'$ tagging along:**
$$\frac{d}{dx}[\sin y] = \cos y \cdot y' \qquad \frac{d}{dx}[xy^2] = y^2 + x\cdot 2y\cdot y'$$

**Solving for $y'$ once everything's differentiated:**

1. Move every term containing $y'$ to one side of the equation; move everything else to the other side.
2. Factor $y'$ out of every term on that side.
3. Divide both sides by whatever's left multiplying $y'$.

## 3. Common mistakes

- **Forgetting to multiply by $y'$ when differentiating a $y$-term.** This is by far the single most common mistake in this entire unit — treating $y$ like a plain constant (with derivative $0$) instead of a hidden function of $x$.
- **Forgetting the product rule whenever $x$ and $y$ appear multiplied together.** Terms like $xy$, $x^2y$, or $xy^2$ always need the product rule — don't just differentiate one factor and ignore the other.
- **Losing track of terms when moving things across the equation.** Take it slow — write out every single term before rearranging, and double-check signs as you move things across the equals sign.
- **Forgetting to factor $y'$ out completely before dividing.** Every term that has $y'$ in it needs to be gathered together and factored as a group.
- **Trying to solve the original equation for $y$ first.** That's often exactly what implicit differentiation is designed to help you avoid — many of these equations can't be solved for $y$ explicitly at all (or only with painful algebra), so there's no need to even attempt it.

## 4. Problem Set

### 🟢 Warm-up

1. $x^2+y^2=25$
2. $x^2+4y^2=16$
3. $y^2=4x$
4. $x^2-y^2=9$
5. $xy=6$
6. $x+y^2=10$
7. $3x^2+2y^2=12$

### 🟡 Standard

8. $x^2y+xy^2=8$
9. $2xy+y^2+x^2=x+y$
10. $xy^2+x^2y=6$
11. $x^2y^3=x+y$
12. $y^3+x^2y=2x$
13. $xy+y^2=4$
14. $x^3+y^3=6xy$

### 🔴 Challenge

15. $y\sin\left(\dfrac{1}{x}\right)=1-xy$
16. $y^3=\dfrac{x-1}{x+1}$
17. $x^2(x+y)^2=x^2+y^2$
18. $\sin(xy)=x+y$
19. $x^2y+y^2=3xy^2$
20. Find the equation of the tangent line to $x^2+y^2=25$ at the point $(3,4)$, using implicit differentiation to find the slope.

### 🌍 Applied

21. A budget constraint relating spending on two goods is $4x+9y^2=100$. Use implicit differentiation to find $\dfrac{dy}{dx}$.
22. A price-quantity relationship for a product is given by $p^2+q^2=200$. Use implicit differentiation to find $\dfrac{dp}{dq}$.
23. A machine part's boundary curve is modeled by $x^2+xy+y^2=19$. Find $\dfrac{dy}{dx}$, then evaluate it at the point $(2,3)$ (you can check this point satisfies the equation), and interpret the result as the slope of the tangent line to the boundary at that point.
24. An indifference curve in economics is modeled by $xy+x^2=12$. Find $\dfrac{dy}{dx}$, then evaluate it at the point where $x=2$ (first find the matching $y$-value), and interpret the result as the marginal rate of substitution at that point.
