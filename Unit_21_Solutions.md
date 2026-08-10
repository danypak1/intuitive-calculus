# Unit 21: Applied Optimization — Full Solutions

### 🟢 Warm-up

**1.** Two positive numbers, sum $=20$, maximize the product.

Let the numbers be $x$ and $20-x$. Objective: $P(x)=x(20-x)=20x-x^2$.

$$P'(x)=20-2x$$

Set $=0$: $x=10$. Check: $P''(x)=-2<0$, confirming a maximum.

**Answer: the numbers are $10$ and $10$; the maximum product is $100$.**

**2.** Rectangle, perimeter $=40$ m, maximize area.

Let the sides be $x$ and $y$, with $2x+2y=40 \Rightarrow y=20-x$. Objective: $A(x)=x(20-x)=20x-x^2$.

$$A'(x)=20-2x$$

Set $=0$: $x=10$, so $y=10$. $A''(x)=-2<0$ confirms a maximum.

**Answer: the rectangle is a $10\text{ m}\times10\text{ m}$ square; maximum area $=100$ m².**

**3.** Two positive numbers, sum $=24$, minimize the sum of their squares.

Let the numbers be $x$ and $24-x$. Objective: $S(x)=x^2+(24-x)^2$.

$$S'(x)=2x+2(24-x)(-1)=2x-2(24-x)=4x-48$$

Set $=0$: $x=12$, so $24-x=12$. $S''(x)=4>0$ confirms a minimum.

**Answer: the numbers are $12$ and $12$; the minimum sum of squares is $144+144=288$.**

**4.** Farmer, $80$ m fencing, rectangular pen (all 4 sides).

Let $2x+2y=80 \Rightarrow y=40-x$. Objective: $A(x)=x(40-x)=40x-x^2$.

$$A'(x)=40-2x$$

Set $=0$: $x=20$, so $y=20$. $A''(x)=-2<0$ confirms a maximum.

**Answer: a $20\text{ m}\times20\text{ m}$ square; maximum area $=400$ m².**

**5.** Rectangle, perimeter $=60$, maximize area.

Let $2x+2y=60 \Rightarrow y=30-x$. Objective: $A(x)=x(30-x)=30x-x^2$.

$$A'(x)=30-2x$$

Set $=0$: $x=15$, so $y=15$. $A''(x)=-2<0$ confirms a maximum.

**Answer: a $15\times15$ square; maximum area $=225$.**

**6.** Two positive numbers, product $=36$, minimize the sum.

Let the numbers be $x$ and $\dfrac{36}{x}$. Objective: $S(x)=x+\dfrac{36}{x}$.

$$S'(x)=1-\frac{36}{x^2}$$

Set $=0$: $x^2=36 \Rightarrow x=6$ (taking the positive root). Then $\dfrac{36}{6}=6$. $S''(x)=\dfrac{72}{x^3}>0$ at $x=6$, confirming a minimum.

**Answer: the numbers are $6$ and $6$; the minimum sum is $12$.**

---

### 🟡 Standard

**7.** $200$ m fencing, 3 sides (river on the 4th).

Let $x$ be each of the two perpendicular sides, and $y$ be the side parallel to the river. Constraint: $2x+y=200 \Rightarrow y=200-2x$. Objective: $A(x)=xy=x(200-2x)=200x-2x^2$.

$$A'(x)=200-4x$$

Set $=0$: $x=50$, so $y=200-100=100$. Domain: $0<x<100$. $A''(x)=-4<0$ confirms a maximum.

**Answer: the sides perpendicular to the river should be $50$ m, and the side parallel to the river should be $100$ m; maximum area $=5000$ m².**

**8.** Square cardboard, side $12$ in, cut $x$ from corners.

The resulting open box has base side $(12-2x)$ and height $x$. Objective: $V(x)=x(12-2x)^2$, for $0<x<6$.

Expand: $V(x) = x(144-48x+4x^2) = 144x-48x^2+4x^3$.

$$V'(x) = 144-96x+12x^2 = 12(x^2-8x+12) = 12(x-2)(x-6)$$

Critical points: $x=2$, $x=6$. Only $x=2$ lies inside the open domain $(0,6)$.

Testing: for $x<2$ (e.g., $x=1$): $12(-1)(-5)=60>0$ (increasing). For $2<x<6$ (e.g., $x=3$): $12(1)(-3)=-36<0$ (decreasing). Sign changes $+$ to $-$, confirming a **maximum** at $x=2$.

$$V(2) = 2(12-4)^2 = 2(8)^2 = 2(64) = 128$$

**Answer: cut squares of side $x=2$ inches; the resulting box has base $8\times8$ inches and height $2$ inches, giving a maximum volume of $128$ in³.**

**9.** Rectangular garden, area $=200$ ft², minimize the perimeter.

Let $xy=200 \Rightarrow y=\dfrac{200}{x}$. Objective: $P(x)=2x+2y=2x+\dfrac{400}{x}$.

$$P'(x) = 2-\frac{400}{x^2}$$

Set $=0$: $x^2=200 \Rightarrow x=\sqrt{200}=10\sqrt2$. Then $y=\dfrac{200}{10\sqrt2}=\dfrac{20}{\sqrt2}=10\sqrt2$.

**Answer: the garden should be a $10\sqrt2 \times 10\sqrt2$ ft square (both dimensions equal, $\approx14.14$ ft); minimum perimeter $=40\sqrt2 \approx 56.57$ ft.**

**10.** Minimize $f(x)=x+\dfrac1x$ for $x>0$.

$$f'(x) = 1-\frac{1}{x^2}$$

Set $=0$: $x^2=1 \Rightarrow x=1$ (positive root). $f''(x)=\dfrac{2}{x^3}>0$ at $x=1$, confirming a minimum.

$$f(1) = 1+1 = 2$$

**Answer: the minimum value is $2$, occurring at $x=1$.**

**11.** Box, square base, no top, volume $=32$ ft³, minimize surface area.

Let the base side be $x$ and height $h$. Constraint: $x^2h=32 \Rightarrow h=\dfrac{32}{x^2}$.

Objective (base $+$ 4 sides, no top): $S(x)=x^2+4xh = x^2+4x\left(\dfrac{32}{x^2}\right) = x^2+\dfrac{128}{x}$.

$$S'(x) = 2x-\frac{128}{x^2}$$

Set $=0$: $2x^3=128 \Rightarrow x^3=64 \Rightarrow x=4$. Then $h=\dfrac{32}{16}=2$.

$S''(x)=2+\dfrac{256}{x^3}>0$ for all $x>0$, confirming a minimum.

$$S(4) = 16+\frac{128}{4} = 16+32=48$$

**Answer: base $4\times4$ ft, height $2$ ft; minimum surface area $=48$ ft².**

**12.** Two positive numbers, product $=100$, minimize (first number) $+2\times$(second number).

Let $xy=100 \Rightarrow y=\dfrac{100}{x}$. Objective: $S(x) = x+2y = x+\dfrac{200}{x}$.

$$S'(x) = 1-\frac{200}{x^2}$$

Set $=0$: $x^2=200 \Rightarrow x=\sqrt{200}=10\sqrt2$. Then $y=\dfrac{100}{10\sqrt2}=\dfrac{10}{\sqrt2}=5\sqrt2$.

$S''(x)=\dfrac{400}{x^3}>0$, confirming a minimum.

**Answer: the numbers are $x=10\sqrt2$ and $y=5\sqrt2$; the minimum value of $x+2y$ is $10\sqrt2+2(5\sqrt2)=20\sqrt2\approx28.28$.**

**13.** Highway on one side, $300$ ft fencing for the other 3 sides.

Let $x$ be each of the two perpendicular sides, $y$ the side parallel to the highway. $2x+y=300 \Rightarrow y=300-2x$. Objective: $A(x)=x(300-2x)=300x-2x^2$.

$$A'(x) = 300-4x$$

Set $=0$: $x=75$, so $y=300-150=150$. $A''(x)=-4<0$ confirms a maximum.

**Answer: the perpendicular sides should be $75$ ft each, and the side parallel to the highway should be $150$ ft; maximum area $=11{,}250$ ft².**

---

### 🔴 Challenge

**14.** Farmland, $400$ m wire, river on one side.

Let $x$ be each of the two perpendicular sides, $y$ the side parallel to the river. $2x+y=400 \Rightarrow y=400-2x$. Objective: $A(x) = x(400-2x) = 400x-2x^2$.

$$A'(x) = 400-4x$$

Set $=0$: $x=100$, so $y=400-200=200$. Domain: $0<x<200$. $A''(x)=-4<0$ confirms a maximum.

**Answer: the sides perpendicular to the river should be $100$ m each, and the side parallel to the river should be $200$ m; maximum enclosed area $=20{,}000$ m².**

**15.** Closed cylinder, volume $=500$ cm³, minimize surface area.

Constraint: $V=\pi r^2h=500 \Rightarrow h=\dfrac{500}{\pi r^2}$.

Objective (top $+$ bottom $+$ side): $S(r) = 2\pi r^2+2\pi rh = 2\pi r^2 + 2\pi r\left(\dfrac{500}{\pi r^2}\right) = 2\pi r^2+\dfrac{1000}{r}$.

$$S'(r) = 4\pi r - \frac{1000}{r^2}$$

Set $=0$: $4\pi r^3 = 1000 \Rightarrow r^3 = \dfrac{250}{\pi} \Rightarrow r = \sqrt[3]{\dfrac{250}{\pi}} \approx 4.30 \text{ cm}$.

Then $h=\dfrac{500}{\pi r^2}$. Using the relationship $\pi = \dfrac{250}{r^3}$ from above:

$$h = \frac{500}{\left(\frac{250}{r^3}\right)r^2} = \frac{500}{\frac{250}{r}} = \frac{500r}{250} = 2r$$

**Answer: $r=\sqrt[3]{\dfrac{250}{\pi}}\approx4.30$ cm, and $h=2r\approx8.60$ cm** — notice the elegant result that the minimizing height is always exactly twice the radius for a closed cylinder.

**16.** Point on $y=2x+3$ closest to the origin.

Distance squared from a point $(x,2x+3)$ on the line to the origin:

$$D(x) = x^2+(2x+3)^2 = x^2+4x^2+12x+9 = 5x^2+12x+9$$

(Minimizing $D(x)$ is equivalent to minimizing the actual distance, since square-rooting doesn't change where the minimum occurs.)

$$D'(x) = 10x+12$$

Set $=0$: $x=-\dfrac{12}{10}=-\dfrac{6}{5}$. Then $y=2\left(-\dfrac65\right)+3 = -\dfrac{12}{5}+\dfrac{15}{5}=\dfrac35$.

$D''(x)=10>0$ confirms a minimum.

**Answer: the closest point is $\left(-\dfrac65,\dfrac35\right)$.** (The minimum distance itself is $\sqrt{D\left(-\frac65\right)} = \sqrt{1.8} = \dfrac{3\sqrt5}{5}\approx1.34$.)

**17.** Box, square base, no top, volume $=108$ in³, minimize material.

Let base side $x$, height $h$. Constraint: $x^2h=108 \Rightarrow h=\dfrac{108}{x^2}$.

Objective: $S(x) = x^2+4xh = x^2+4x\left(\dfrac{108}{x^2}\right) = x^2+\dfrac{432}{x}$.

$$S'(x) = 2x-\frac{432}{x^2}$$

Set $=0$: $2x^3=432 \Rightarrow x^3=216 \Rightarrow x=6$. Then $h=\dfrac{108}{36}=3$.

$S''(x)=2+\dfrac{864}{x^3}>0$, confirming a minimum.

$$S(6) = 36+\frac{432}{6} = 36+72=108$$

**Answer: base $6\times6$ in, height $3$ in; minimum material used $=108$ in².**

**18.** Norman window, perimeter $=20$ ft, maximize area.

Let $x$ be the rectangle's width (also the semicircle's diameter), and $y$ the rectangle's height.

**Perimeter constraint:** bottom ($x$) $+$ two sides ($2y$) $+$ semicircular arc ($\dfrac{\pi x}{2}$, since the arc length of a full circle of radius $\frac{x}{2}$ is $\pi x$, and we only use half):

$$x+2y+\frac{\pi x}{2} = 20$$

Solve for $y$:

$$2y = 20-x-\frac{\pi x}{2} \quad\Rightarrow\quad y = 10-\frac{x}{2}-\frac{\pi x}{4}$$

**Area:** rectangle plus semicircle ($\dfrac12\pi\left(\dfrac{x}{2}\right)^2 = \dfrac{\pi x^2}{8}$):

$$A(x) = xy + \frac{\pi x^2}{8}$$

Substitute $y$:

$$A(x) = x\left(10-\frac{x}{2}-\frac{\pi x}{4}\right) + \frac{\pi x^2}{8} = 10x-\frac{x^2}{2}-\frac{\pi x^2}{4}+\frac{\pi x^2}{8}$$

Combine the $\pi x^2$ terms: $-\dfrac{\pi x^2}{4}+\dfrac{\pi x^2}{8} = -\dfrac{\pi x^2}{8}$.

$$A(x) = 10x - \frac{x^2}{2} - \frac{\pi x^2}{8} = 10x - \frac{(4+\pi)x^2}{8}$$

Differentiate:

$$A'(x) = 10 - \frac{(4+\pi)x}{4}$$

Set $=0$:

$$10 = \frac{(4+\pi)x}{4} \quad\Rightarrow\quad x = \frac{40}{4+\pi} \approx 5.60 \text{ ft}$$

Then:

$$y = 10-\frac{x}{2}-\frac{\pi x}{4}$$

It turns out (after simplifying algebraically) that at this optimal $x$, $y=\dfrac{x}{2}$ exactly:

$$y = \frac{20}{4+\pi} \approx 2.80 \text{ ft}$$

The maximum area simplifies to:

$$A = \frac{200}{4+\pi} \approx 28.01 \text{ ft}^2$$

**Answer: width $x=\dfrac{40}{4+\pi}\approx5.60$ ft, rectangle height $y=\dfrac{20}{4+\pi}\approx2.80$ ft; maximum area $\approx28.01$ ft².**

---

### 🌍 Applied

**19.** $q=1200-40p$, maximize $R=pq$.

$$R(p) = p(1200-40p) = 1200p-40p^2$$

$$R'(p) = 1200-80p$$

Set $=0$: $p=15$. $R''(p)=-80<0$ confirms a maximum. $q=1200-40(15)=1200-600=600$.

**Answer: set the price at $p=\$15$; maximum revenue $=15\times600=\$9000$.**

**20.** $C(x)=2x+\dfrac{800}{x}$, minimize for $x>0$.

$$C'(x) = 2-\frac{800}{x^2}$$

Set $=0$: $x^2=400 \Rightarrow x=20$. $C''(x)=\dfrac{1600}{x^3}>0$ at $x=20$, confirming a minimum.

$$C(20) = 40+40=80$$

**Answer: order size $x=20$ units; minimum total cost $=\$80$.**

**21.** Storage yard, wall on one side, $240$ ft fencing for the other 3 sides.

Let $x$ be each of the two perpendicular sides, $y$ the side parallel to the wall. $2x+y=240 \Rightarrow y=240-2x$. Objective: $A(x)=x(240-2x)=240x-2x^2$.

$$A'(x) = 240-4x$$

Set $=0$: $x=60$, so $y=240-120=120$. $A''(x)=-4<0$ confirms a maximum.

**Answer: the sides perpendicular to the wall should be $60$ ft each, and the side parallel to the wall should be $120$ ft; maximum area $=7200$ ft².**

**22.** $P(x)=-0.02x^2+40x-300$.

$$P'(x) = -0.04x+40$$

Set $=0$: $x=1000$. $P''(x)=-0.04<0$ confirms a maximum.

$$P(1000) = -0.02(1{,}000{,}000)+40{,}000-300 = -20{,}000+40{,}000-300 = 19{,}700$$

**Answer: produce $1000$ units; maximum profit $=\$19{,}700$.**
