# Unit 14: Implicit Differentiation — Full Solutions

### 🟢 Warm-up

**1.** $x^2+y^2=25$

Differentiate both sides with respect to $x$:

$$2x + 2y\cdot y' = 0$$

Solve for $y'$:

$$2y\cdot y' = -2x \quad\Rightarrow\quad y' = -\frac{x}{y}$$

**2.** $x^2+4y^2=16$

$$2x + 8y\cdot y' = 0$$

$$y' = -\frac{2x}{8y} = -\frac{x}{4y}$$

**3.** $y^2=4x$

$$2y\cdot y' = 4$$

$$y' = \frac{4}{2y} = \frac{2}{y}$$

**4.** $x^2-y^2=9$

$$2x - 2y\cdot y' = 0$$

$$2y\cdot y' = 2x \quad\Rightarrow\quad y' = \frac{x}{y}$$

**5.** $xy=6$

Use the product rule on the left side:

$$y + x\cdot y' = 0$$

$$y' = -\frac{y}{x}$$

**6.** $x+y^2=10$

$$1 + 2y\cdot y' = 0$$

$$y' = -\frac{1}{2y}$$

**7.** $3x^2+2y^2=12$

$$6x + 4y\cdot y' = 0$$

$$y' = -\frac{6x}{4y} = -\frac{3x}{2y}$$

---

### 🟡 Standard

**8.** $x^2y+xy^2=8$

Differentiate each term using the product rule.

$\dfrac{d}{dx}[x^2y] = 2xy + x^2y'$

$\dfrac{d}{dx}[xy^2] = y^2 + x\cdot 2y\cdot y' = y^2+2xy\cdot y'$

The right side's derivative is $0$ (it's a constant):

$$2xy + x^2y' + y^2 + 2xy\cdot y' = 0$$

Collect the $y'$ terms:

$$y'(x^2+2xy) = -(2xy+y^2)$$

$$y' = \frac{-(2xy+y^2)}{x^2+2xy}$$

**9.** $2xy+y^2+x^2=x+y$

Differentiate term by term.

$\dfrac{d}{dx}[2xy] = 2(y+x\cdot y') = 2y+2xy'$

$\dfrac{d}{dx}[y^2] = 2y\cdot y'$

$\dfrac{d}{dx}[x^2] = 2x$

Right side: $\dfrac{d}{dx}[x+y] = 1+y'$

$$2y+2xy' + 2yy' + 2x = 1+y'$$

Collect $y'$ terms on the left, everything else on the right:

$$2xy'+2yy'-y' = 1-2y-2x$$

$$y'(2x+2y-1) = 1-2y-2x$$

$$y' = \frac{1-2y-2x}{2x+2y-1}$$

**10.** $xy^2+x^2y=6$

$\dfrac{d}{dx}[xy^2] = y^2+2xy\cdot y'$

$\dfrac{d}{dx}[x^2y] = 2xy+x^2y'$

$$y^2+2xy\cdot y' + 2xy+x^2y' = 0$$

$$y'(2xy+x^2) = -(y^2+2xy)$$

$$y' = \frac{-(y^2+2xy)}{2xy+x^2}$$

**11.** $x^2y^3=x+y$

$\dfrac{d}{dx}[x^2y^3] = 2xy^3 + x^2\cdot 3y^2\cdot y' = 2xy^3+3x^2y^2y'$

$$2xy^3+3x^2y^2y' = 1+y'$$

Collect $y'$ terms:

$$3x^2y^2y'-y' = 1-2xy^3$$

$$y'(3x^2y^2-1) = 1-2xy^3$$

$$y' = \frac{1-2xy^3}{3x^2y^2-1}$$

**12.** $y^3+x^2y=2x$

$\dfrac{d}{dx}[y^3] = 3y^2y'$

$\dfrac{d}{dx}[x^2y] = 2xy+x^2y'$

$$3y^2y'+2xy+x^2y' = 2$$

$$y'(3y^2+x^2) = 2-2xy$$

$$y' = \frac{2-2xy}{3y^2+x^2}$$

**13.** $xy+y^2=4$

$\dfrac{d}{dx}[xy] = y+xy'$

$\dfrac{d}{dx}[y^2] = 2yy'$

$$y+xy'+2yy' = 0$$

$$y'(x+2y) = -y$$

$$y' = -\frac{y}{x+2y}$$

**14.** $x^3+y^3=6xy$

$\dfrac{d}{dx}[x^3] = 3x^2$

$\dfrac{d}{dx}[y^3] = 3y^2y'$

$\dfrac{d}{dx}[6xy] = 6(y+xy') = 6y+6xy'$

$$3x^2+3y^2y' = 6y+6xy'$$

Collect $y'$ terms:

$$3y^2y'-6xy' = 6y-3x^2$$

$$y'(3y^2-6x) = 6y-3x^2$$

Divide top and bottom by $3$:

$$y' = \frac{2y-x^2}{y^2-2x}$$

---

### 🔴 Challenge

**15.** $y\sin\left(\dfrac{1}{x}\right)=1-xy$

**Left side** (product rule, with the second factor needing the chain rule):

Let $u=y$ ($u'=y'$) and $v=\sin\left(\frac{1}{x}\right)$. To find $v'$, use the chain rule with inner function $\frac{1}{x}=x^{-1}$ (derivative $-x^{-2}=-\frac{1}{x^2}$):

$$v' = \cos\left(\frac{1}{x}\right)\cdot\left(-\frac{1}{x^2}\right) = -\frac{\cos(1/x)}{x^2}$$

$$\frac{d}{dx}\left[y\sin\left(\frac1x\right)\right] = y'\sin\left(\frac1x\right) + y\cdot\left(-\frac{\cos(1/x)}{x^2}\right) = y'\sin\left(\frac1x\right) - \frac{y\cos(1/x)}{x^2}$$

**Right side:**

$$\frac{d}{dx}[1-xy] = 0-(y+xy') = -y-xy'$$

Set both sides equal:

$$y'\sin\left(\frac1x\right) - \frac{y\cos(1/x)}{x^2} = -y-xy'$$

Collect the $y'$ terms on the left:

$$y'\sin\left(\frac1x\right)+xy' = -y+\frac{y\cos(1/x)}{x^2}$$

$$y'\left[\sin\left(\frac1x\right)+x\right] = y\left[\frac{\cos(1/x)}{x^2}-1\right]$$

$$y' = \frac{y\left[\dfrac{\cos(1/x)}{x^2}-1\right]}{\sin\left(\dfrac1x\right)+x}$$

**16.** $y^3=\dfrac{x-1}{x+1}$

Left side: $\dfrac{d}{dx}[y^3] = 3y^2y'$.

Right side: use the quotient rule with $f=x-1$ ($f'=1$), $g=x+1$ ($g'=1$):

$$\frac{d}{dx}\left[\frac{x-1}{x+1}\right] = \frac{1\cdot(x+1) - (x-1)\cdot 1}{(x+1)^2} = \frac{(x+1)-(x-1)}{(x+1)^2} = \frac{2}{(x+1)^2}$$

Set both sides equal:

$$3y^2y' = \frac{2}{(x+1)^2}$$

$$y' = \frac{2}{3y^2(x+1)^2}$$

**17.** $x^2(x+y)^2=x^2+y^2$

**Left side:** product rule with $f=x^2$ ($f'=2x$) and $g=(x+y)^2$. For $g'$, use the chain rule with inner function $x+y$ (whose derivative is $1+y'$, since $y$ depends on $x$):

$$g' = 2(x+y)(1+y')$$

$$\frac{d}{dx}\big[x^2(x+y)^2\big] = 2x(x+y)^2 + x^2\cdot 2(x+y)(1+y')$$

Expand the second piece: $2x^2(x+y)(1+y') = 2x^2(x+y) + 2x^2(x+y)y'$.

So the left side becomes:

$$2x(x+y)^2 + 2x^2(x+y) + 2x^2(x+y)\,y'$$

**Right side:**

$$\frac{d}{dx}[x^2+y^2] = 2x+2y\cdot y'$$

Setting both sides equal:

$$2x(x+y)^2 + 2x^2(x+y) + 2x^2(x+y)\,y' = 2x+2y\cdot y'$$

Collect the $y'$ terms:

$$2x^2(x+y)\,y' - 2y\,y' = 2x - 2x(x+y)^2 - 2x^2(x+y)$$

$$y'\big[2x^2(x+y)-2y\big] = 2x-2x(x+y)^2-2x^2(x+y)$$

Divide top and bottom by $2$:

$$y' = \frac{x-x(x+y)^2-x^2(x+y)}{x^2(x+y)-y}$$

**18.** $\sin(xy)=x+y$

Left side: chain rule with inner function $u=xy$ (whose derivative uses the product rule: $u'=y+xy'$):

$$\frac{d}{dx}[\sin(xy)] = \cos(xy)\cdot(y+xy')$$

Right side:

$$\frac{d}{dx}[x+y] = 1+y'$$

Set equal:

$$\cos(xy)\cdot(y+xy') = 1+y'$$

Expand the left side:

$$y\cos(xy) + xy'\cos(xy) = 1+y'$$

Collect $y'$ terms:

$$xy'\cos(xy)-y' = 1-y\cos(xy)$$

$$y'\big[x\cos(xy)-1\big] = 1-y\cos(xy)$$

$$y' = \frac{1-y\cos(xy)}{x\cos(xy)-1}$$

**19.** $x^2y+y^2=3xy^2$

$\dfrac{d}{dx}[x^2y] = 2xy+x^2y'$

$\dfrac{d}{dx}[y^2] = 2yy'$

$\dfrac{d}{dx}[3xy^2] = 3(y^2+x\cdot 2y\cdot y') = 3y^2+6xyy'$

$$2xy+x^2y'+2yy' = 3y^2+6xyy'$$

Collect the $y'$ terms:

$$x^2y'+2yy'-6xyy' = 3y^2-2xy$$

$$y'\big(x^2+2y-6xy\big) = 3y^2-2xy$$

$$y' = \frac{3y^2-2xy}{x^2+2y-6xy}$$

**20.** Tangent line to $x^2+y^2=25$ at $(3,4)$.

From Problem 1, we already know: $y' = -\dfrac{x}{y}$.

At $(3,4)$:

$$y' = -\frac{3}{4}$$

Using point-slope form with point $(3,4)$ and slope $-\dfrac34$:

$$y-4 = -\frac34(x-3)$$

$$y = -\frac34x+\frac94+4 = -\frac34x+\frac94+\frac{16}{4} = -\frac34x+\frac{25}{4}$$

**Tangent line: $y=-\dfrac34x+\dfrac{25}{4}$.**

---

### 🌍 Applied

**21.** $4x+9y^2=100$

$$4+18y\cdot y' = 0$$

$$y' = -\frac{4}{18y} = -\frac{2}{9y}$$

**Answer: $\dfrac{dy}{dx} = -\dfrac{2}{9y}$.**

**22.** $p^2+q^2=200$, find $\dfrac{dp}{dq}$.

Differentiate with respect to $q$, treating $p$ as a function of $q$:

$$2p\cdot\frac{dp}{dq} + 2q = 0$$

$$\frac{dp}{dq} = -\frac{2q}{2p} = -\frac{q}{p}$$

**Answer: $\dfrac{dp}{dq} = -\dfrac{q}{p}$.**

**23.** $x^2+xy+y^2=19$

Differentiate:

$$2x + (y+xy') + 2yy' = 0$$

$$2x+y+xy'+2yy' = 0$$

Collect $y'$ terms:

$$y'(x+2y) = -(2x+y)$$

$$y' = -\frac{2x+y}{x+2y}$$

Check the point $(2,3)$: $2^2+2(3)+3^2 = 4+6+9=19$ ✓.

Evaluate at $(2,3)$:

$$y' = -\frac{2(2)+3}{2+2(3)} = -\frac{4+3}{2+6} = -\frac{7}{8}$$

**Answer: $\dfrac{dy}{dx} = -\dfrac{2x+y}{x+2y}$, and at $(2,3)$, $\dfrac{dy}{dx}=-\dfrac{7}{8}$.** This means the boundary curve of the machine part has a slope of $-\dfrac78$ at that point.

**24.** $xy+x^2=12$

Differentiate:

$$y+xy'+2x = 0$$

$$xy' = -y-2x$$

$$y' = -\frac{y+2x}{x}$$

Find $y$ when $x=2$: plug into the original equation, $2y+4=12 \Rightarrow 2y=8 \Rightarrow y=4$. So the point is $(2,4)$.

Evaluate at $(2,4)$:

$$y' = -\frac{4+2(2)}{2} = -\frac{4+4}{2} = -\frac{8}{2} = -4$$

**Answer: $\dfrac{dy}{dx} = -\dfrac{y+2x}{x}$, and at $(2,4)$, $\dfrac{dy}{dx}=-4$.** This means the marginal rate of substitution at that point on the indifference curve is $-4$.
