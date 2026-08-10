# Unit 21: Applied Optimization

## 1. The idea, in plain words

This is the payoff unit — where finding the "best" answer to a real-world question (the biggest area, the smallest cost, the largest volume) becomes a calculus problem you can actually solve. **Every optimization problem is secretly the same story: find the peak or valley of some quantity, using everything you already know about critical points and extrema.**

**The catch:** word problems don't hand you a tidy function $f(x)$ ready to differentiate. You have to *build* one yourself out of the story — and almost always, the story gives you **two related variables** (like length and width) tied together by some **fixed constraint** (like a fixed amount of fencing). Your job is to use that constraint to eliminate one variable, leaving a single-variable function you can actually optimize with the tools you already have.

**Picture it like a recipe with a fixed budget:** if you have a fixed amount of fencing, making the pen longer forces it to be narrower, and vice versa — the two dimensions are locked together. Once you express one in terms of the other, you've turned a two-variable puzzle into a one-variable calculus problem: build the objective function, differentiate, find where the derivative is zero, and confirm whether that's a max or a min.

**The complete step-by-step strategy:**

1. **Read carefully and draw a picture** if the problem describes a physical shape.
2. **Identify the objective** — the quantity you're trying to maximize or minimize. This becomes your function.
3. **Identify the constraint** — the fixed relationship between the variables (a fixed perimeter, budget, volume, etc.).
4. **Use the constraint to rewrite the objective function in terms of a single variable.**
5. **Figure out the domain** — what values actually make physical sense? (Lengths must be positive, etc.)
6. **Differentiate, set equal to zero, and solve for the critical point(s).**
7. **Confirm it's actually a max or min** — using the first derivative test, the second derivative test, or the closed interval method.
8. **Answer the actual question asked** — sometimes that's a dimension, sometimes it's the optimized value itself, sometimes both. Don't stop at just finding the critical $x$-value.

## 2. Toolbox

**No new formulas this unit** — this is entirely about applying everything from Units 17–20 (critical points, the first/second derivative tests, the closed interval method) to freshly built functions. The "toolbox" here is really the **8-step strategy above** — treat it as your formula.

**Common constraint-and-objective pairs to recognize:**
$$\text{Perimeter of a rectangle: } P=2x+2y \qquad \text{Area: } A=xy$$
$$\text{Volume of a box: } V=xyz \qquad \text{Surface area (varies by shape — build it from the picture)}$$
$$\text{Distance between two points: } d=\sqrt{(x_2-x_1)^2+(y_2-y_1)^2}$$
$$\text{Circle area: } A=\pi r^2 \qquad \text{Circle circumference: } C=2\pi r$$
$$\text{(a semicircle is just half of each: area } \tfrac12\pi r^2\text{, arc length } \pi r\text{)}$$

**A useful shortcut for distance problems:** minimizing $d$ is the same as minimizing $d^2$ (since square-rooting is an increasing operation) — and $d^2$ has no square root to differentiate, so it's usually much easier to work with.

## 3. Common mistakes

- **Trying to optimize a function of two variables directly.** You must always use the constraint to reduce down to one variable before differentiating — basic calculus optimization only works one variable at a time.
- **Forgetting to check the domain.** A length or width can never be negative, and often can't be zero either — always figure out the realistic range of values before trusting a critical point.
- **Finding a critical point and stopping there — without confirming it's actually a max (or min), not the other one.** Solving $f'(x)=0$ only gives you a *candidate*; you still need the first or second derivative test (or the closed interval method) to know which kind of extreme point it is.
- **Answering with the wrong quantity.** If the problem asks for the dimensions, report both dimensions — not just the value of $x$. If it asks for the maximum area itself, compute and report that number too.
- **Setting up the constraint equation incorrectly.** Take extra care translating the word problem into an equation — a wrong constraint dooms the whole problem, even if every calculus step afterward is done perfectly.

## 4. Problem Set

### 🟢 Warm-up

1. Find two positive numbers whose sum is $20$ and whose product is as large as possible.
2. A rectangle has a perimeter of $40$ m. Find the dimensions that maximize its area.
3. Find two positive numbers whose sum is $24$ such that the sum of their squares is as small as possible.
4. A farmer has $80$ m of fencing to enclose a rectangular pen (fencing on all four sides). Find the dimensions that maximize the enclosed area.
5. A rectangle has a perimeter of $60$. Find the dimensions that maximize its area.
6. Find two positive numbers whose product is $36$ such that their sum is as small as possible.

### 🟡 Standard

7. A farmer has $200$ m of fencing to enclose a rectangular field. One side of the field borders a straight river, so no fencing is needed there. Find the dimensions that maximize the enclosed area.
8. An open-top box is made from a square piece of cardboard with side length $12$ inches, by cutting a square of side $x$ from each corner and folding up the sides. Find the value of $x$ that maximizes the box's volume.
9. A rectangular garden must have an area of $200$ square feet and will be fenced on all four sides. Find the dimensions that minimize the amount of fencing needed.
10. Find the minimum value of $f(x)=x+\dfrac1x$ for $x>0$.
11. A box with a square base and no top must have a volume of $32$ cubic feet. Find the dimensions that minimize the surface area (amount of material used).
12. Two positive numbers have a product of $100$. Find the two numbers that minimize the value of (the first number) plus (twice the second number).
13. A rectangular field borders a straight highway on one side (no fencing needed there), and $300$ ft of fencing is available for the other three sides. Find the dimensions that maximize the enclosed area.

### 🔴 Challenge

14. A rectangular plot of farmland will be bounded on one side by a river and on the other three sides by a single-strand electric fence. With $400$ m of wire available, find the dimensions that give the largest possible enclosed area.
15. A closed cylindrical can must hold a volume of $500$ cm³. Find the radius and height that minimize the total surface area (top, bottom, and side) of the can.
16. Find the point on the line $y=2x+3$ that is closest to the origin.
17. A box with a square base and no top must have a volume of $108$ cubic inches. Find the dimensions that minimize the amount of material used.
18. A "Norman window" is shaped like a rectangle topped with a semicircle (the semicircle's diameter equals the rectangle's width). The total perimeter of the window (including the flat bottom, the two straight sides, and the curved top, but not the straight line where the rectangle and semicircle meet) is $20$ ft. Find the dimensions that maximize the area of the window.

### 🌍 Applied

19. A company sells a product at price $p$ dollars, and the quantity sold is $q=1200-40p$ units. Find the price $p$ that maximizes total revenue $R=pq$.
20. A company's total annual cost for ordering and storing inventory is modeled by $C(x)=2x+\dfrac{800}{x}$ dollars, where $x$ is the order size. Find the order size that minimizes total cost.
21. A store manager has $240$ ft of fencing to enclose a rectangular storage yard. One side of the yard is against the store's wall, so no fencing is needed there. Find the dimensions that maximize the enclosed area.
22. A company's profit (in dollars) from producing $x$ units is modeled by $P(x)=-0.02x^2+40x-300$. Find the production level that maximizes profit, and find the maximum profit.
