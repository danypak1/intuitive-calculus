# Unit 15: Related Rates — Full Solutions

### 🟢 Warm-up

**1.** Circle, $A=\pi r^2$, $\dfrac{dr}{dt}=3$, find $\dfrac{dA}{dt}$ at $r=5$.

Differentiate with respect to $t$:

$$\frac{dA}{dt} = 2\pi r\cdot\frac{dr}{dt}$$

Plug in $r=5$, $\dfrac{dr}{dt}=3$:

$$\frac{dA}{dt} = 2\pi(5)(3) = 30\pi \text{ cm}^2/\text{s}$$

**2.** Square, $A=s^2$, $\dfrac{ds}{dt}=2$, find $\dfrac{dA}{dt}$ at $s=4$.

$$\frac{dA}{dt} = 2s\cdot\frac{ds}{dt} = 2(4)(2) = 16 \text{ cm}^2/\text{s}$$

**3.** Sphere, $V=\dfrac43\pi r^3$, $\dfrac{dr}{dt}=4$, find $\dfrac{dV}{dt}$ at $r=3$.

$$\frac{dV}{dt} = 4\pi r^2\cdot\frac{dr}{dt}$$

$$\frac{dV}{dt} = 4\pi(3)^2(4) = 4\pi(9)(4) = 144\pi \text{ cm}^3/\text{s}$$

**4.** Cube, $V=s^3$, $\dfrac{ds}{dt}=1$, find $\dfrac{dV}{dt}$ at $s=5$.

$$\frac{dV}{dt} = 3s^2\cdot\frac{ds}{dt} = 3(25)(1) = 75 \text{ cm}^3/\text{s}$$

**5.** Circle, $A=\pi r^2$, $\dfrac{dr}{dt}=-2$ (shrinking), find $\dfrac{dA}{dt}$ at $r=6$.

$$\frac{dA}{dt} = 2\pi r\cdot\frac{dr}{dt} = 2\pi(6)(-2) = -24\pi \text{ cm}^2/\text{s}$$

**The negative sign confirms the area is shrinking**, at a rate of $24\pi$ cm²/s.

**6.** Equilateral triangle, $A=\dfrac{\sqrt3}{4}s^2$, $\dfrac{ds}{dt}=3$, find $\dfrac{dA}{dt}$ at $s=6$.

$$\frac{dA}{dt} = \frac{\sqrt3}{4}\cdot 2s\cdot\frac{ds}{dt} = \frac{\sqrt3}{2}s\cdot\frac{ds}{dt}$$

$$\frac{dA}{dt} = \frac{\sqrt3}{2}(6)(3) = 9\sqrt3 \text{ cm}^2/\text{s}$$

---

### 🟡 Standard

**7.** Ladder: let $x$ = distance of bottom from wall, $y$ = height of top on wall. $x^2+y^2=10^2=100$.

Given $\dfrac{dx}{dt}=2$ ft/s. Find $\dfrac{dy}{dt}$ when $x=6$.

First find $y$ when $x=6$: $y^2 = 100-36=64 \Rightarrow y=8$.

Differentiate the connecting equation with respect to $t$:

$$2x\frac{dx}{dt} + 2y\frac{dy}{dt} = 0$$

Solve for $\dfrac{dy}{dt}$:

$$\frac{dy}{dt} = -\frac{x}{y}\cdot\frac{dx}{dt} = -\frac{6}{8}(2) = -\frac{3}{2} \text{ ft/s}$$

**Answer: the top is sliding down at $\dfrac32$ ft/s** (the negative sign means $y$ is decreasing).

**8.** Balloon: let $h$ = height, $z$ = distance from observer. Fixed horizontal distance $100$ ft, so $z^2 = 100^2+h^2 = 10000+h^2$.

Given $\dfrac{dh}{dt}=5$ ft/s. Find $\dfrac{dz}{dt}$ when $h=75$.

First find $z$: $z^2 = 10000+75^2 = 10000+5625=15625 \Rightarrow z=125$ (since $125^2=15625$).

Differentiate:

$$2z\frac{dz}{dt} = 2h\frac{dh}{dt}$$

$$\frac{dz}{dt} = \frac{h}{z}\cdot\frac{dh}{dt} = \frac{75}{125}(5) = \frac{375}{125} = 3 \text{ ft/s}$$

**9.** Cylinder, fixed radius $r=3$ ft. $V=\pi r^2h = 9\pi h$ (since $r$ never changes).

Given $\dfrac{dV}{dt}=2$ ft³/min. Differentiate:

$$\frac{dV}{dt} = 9\pi\frac{dh}{dt}$$

$$\frac{dh}{dt} = \frac{2}{9\pi} \text{ ft/min}$$

**10.** Two cars: let $x$ = eastbound car's distance, $y$ = northbound car's distance, $z$ = distance between them. $z^2=x^2+y^2$.

Given $\dfrac{dx}{dt}=40$ mph, $\dfrac{dy}{dt}=30$ mph. Find $\dfrac{dz}{dt}$ when $x=3$, $y=4$.

First find $z$: $z^2=9+16=25 \Rightarrow z=5$.

Differentiate:

$$2z\frac{dz}{dt} = 2x\frac{dx}{dt}+2y\frac{dy}{dt}$$

$$\frac{dz}{dt} = \frac{x\frac{dx}{dt}+y\frac{dy}{dt}}{z} = \frac{(3)(40)+(4)(30)}{5} = \frac{120+120}{5} = \frac{240}{5} = 48 \text{ mph}$$

**11.** Rectangle, $A=LW$. Given $\dfrac{dL}{dt}=3$ cm/s, $\dfrac{dW}{dt}=-2$ cm/s. Find $\dfrac{dA}{dt}$ at $L=10$, $W=6$.

Differentiate using the product rule:

$$\frac{dA}{dt} = \frac{dL}{dt}\cdot W + L\cdot\frac{dW}{dt}$$

$$\frac{dA}{dt} = (3)(6) + (10)(-2) = 18-20 = -2 \text{ cm}^2/\text{s}$$

**The area is currently decreasing**, at a rate of $2$ cm²/s.

**12.** Shadow: let $x$ = person's distance from the lamp post, $s$ = shadow length. By similar triangles (comparing the lamp post's height/distance triangle to the person's height/shadow triangle):

$$\frac{15}{x+s} = \frac{6}{s}$$

Cross-multiply: $15s = 6(x+s) = 6x+6s$, so $9s=6x$, giving $s=\dfrac{2}{3}x$.

Differentiate this simplified relationship directly:

$$\frac{ds}{dt} = \frac{2}{3}\cdot\frac{dx}{dt} = \frac{2}{3}(5) = \frac{10}{3} \text{ ft/s}$$

**The shadow length is growing at $\dfrac{10}{3}$ ft/s** — notice this rate stays constant no matter how far the person has already walked.

**13.** Rectangle, fixed width $W=4$, length $L$ growing at $\dfrac{dL}{dt}=2$ cm/s. Diagonal: $d^2=L^2+W^2=L^2+16$.

Find $\dfrac{dd}{dt}$ when $L=3$: first find $d$: $d^2=9+16=25 \Rightarrow d=5$.

Differentiate:

$$2d\frac{dd}{dt} = 2L\frac{dL}{dt}$$

$$\frac{dd}{dt} = \frac{L}{d}\cdot\frac{dL}{dt} = \frac{3}{5}(2) = \frac{6}{5} = 1.2 \text{ cm/s}$$

---

### 🔴 Challenge

**14.** Conical tank: top radius $R=4$ ft, height $H=10$ ft (fixed tank dimensions). Let $r$ and $h$ be the radius and height of the water's surface at any moment.

By similar triangles, $\dfrac{r}{h}=\dfrac{R}{H}=\dfrac{4}{10}=\dfrac25$, so $r=\dfrac25 h$.

Substitute into the cone volume formula to eliminate $r$:

$$V = \frac13\pi r^2h = \frac13\pi\left(\frac25h\right)^2h = \frac13\pi\cdot\frac{4}{25}h^2\cdot h = \frac{4\pi}{75}h^3$$

Differentiate with respect to $t$:

$$\frac{dV}{dt} = \frac{4\pi}{75}\cdot 3h^2\cdot\frac{dh}{dt} = \frac{4\pi}{25}h^2\cdot\frac{dh}{dt}$$

Given $\dfrac{dV}{dt}=-3$ ft³/min (draining, so negative) and $h=5$:

$$-3 = \frac{4\pi}{25}(25)\cdot\frac{dh}{dt} = 4\pi\cdot\frac{dh}{dt}$$

$$\frac{dh}{dt} = -\frac{3}{4\pi} \text{ ft/min}$$

**The water level is dropping at a rate of $\dfrac{3}{4\pi}$ ft/min.**

**15.** Ships: let $x$ = remaining east-west gap between the ships, $y$ = Ship B's northward distance, $z$ = distance between the ships.

Ship A starts $100$ km west of Ship B and sails east at $15$ km/h, closing the east-west gap, so $x = 100-15t$. Ship B sails north at $20$ km/h, so $y=20t$.

At $t=4$ (4:00 PM): $x=100-15(4)=100-60=40$. $y=20(4)=80$.

$$z^2 = x^2+y^2 = 40^2+80^2 = 1600+6400 = 8000$$

$$z = \sqrt{8000} = 40\sqrt5$$

Rates: $\dfrac{dx}{dt}=-15$ (the east-west gap is shrinking), $\dfrac{dy}{dt}=20$.

Differentiate $z^2=x^2+y^2$:

$$2z\frac{dz}{dt} = 2x\frac{dx}{dt}+2y\frac{dy}{dt}$$

$$\frac{dz}{dt} = \frac{x\frac{dx}{dt}+y\frac{dy}{dt}}{z} = \frac{(40)(-15)+(80)(20)}{40\sqrt5} = \frac{-600+1600}{40\sqrt5} = \frac{1000}{40\sqrt5} = \frac{25}{\sqrt5}$$

Rationalize: $\dfrac{25}{\sqrt5} = \dfrac{25\sqrt5}{5} = 5\sqrt5$.

**Answer: the distance between the ships is increasing at a rate of $5\sqrt5 \approx 11.18$ km/h.**

**16.** Kite: fixed height $h=300$ ft. Let $x$ = horizontal distance, $L$ = string length. $L^2=x^2+300^2=x^2+90000$.

Given $\dfrac{dx}{dt}=25$ ft/s. Find $\dfrac{dL}{dt}$ when $L=500$.

First find $x$ when $L=500$: $x^2 = 500^2-90000 = 250000-90000=160000 \Rightarrow x=400$.

Differentiate:

$$2L\frac{dL}{dt} = 2x\frac{dx}{dt}$$

$$\frac{dL}{dt} = \frac{x}{L}\cdot\frac{dx}{dt} = \frac{400}{500}(25) = \frac{10000}{500} = 20 \text{ ft/s}$$

**17.** Box: $V=lwh$. At this instant, $l=4$, $w=3$, $h=2$, with $\dfrac{dl}{dt}=2$, $\dfrac{dw}{dt}=-1$, $\dfrac{dh}{dt}=3$.

Differentiate using the extended product rule (three factors — each term holds two factors still while differentiating the third):

$$\frac{dV}{dt} = \frac{dl}{dt}\cdot wh + l\cdot\frac{dw}{dt}\cdot h + lw\cdot\frac{dh}{dt}$$

$$\frac{dV}{dt} = (2)(3)(2) + (4)(-1)(2) + (4)(3)(3)$$

$$= 12 + (-8) + 36 = 40$$

**Answer: the volume is increasing at a rate of $40$ ft³/min.**

**18.** Spotlight: fixed perpendicular distance $50$ m. Let $x$ = runner's distance along the track from the closest point, $\theta$ = angle between the beam and the perpendicular.

$$\tan\theta = \frac{x}{50}$$

Differentiate with respect to $t$:

$$\sec^2\theta\cdot\frac{d\theta}{dt} = \frac{1}{50}\cdot\frac{dx}{dt}$$

$$\frac{d\theta}{dt} = \frac{1}{50\sec^2\theta}\cdot\frac{dx}{dt} = \frac{\cos^2\theta}{50}\cdot\frac{dx}{dt}$$

At $x=50$: $\tan\theta = \dfrac{50}{50}=1 \Rightarrow \theta = 45°$, so $\cos\theta = \dfrac{\sqrt2}{2}$, and $\cos^2\theta = \dfrac12$.

Given $\dfrac{dx}{dt}=6$ m/s:

$$\frac{d\theta}{dt} = \frac{\frac12}{50}(6) = \frac{6}{100} = 0.06 \text{ rad/s}$$

---

### 🌍 Applied

**19.** $R=xp$. Given $x=100$, $p=20$, $\dfrac{dx}{dt}=5$, $\dfrac{dp}{dt}=-0.5$.

$$\frac{dR}{dt} = \frac{dx}{dt}\cdot p + x\cdot\frac{dp}{dt}$$

$$\frac{dR}{dt} = (5)(20) + (100)(-0.5) = 100-50 = 50$$

**Answer: revenue is increasing at $\$50$ per week.**

**20.** $A=\pi r^2$. Given $r=20$, $\dfrac{dr}{dt}=0.5$.

$$\frac{dA}{dt} = 2\pi r\cdot\frac{dr}{dt} = 2\pi(20)(0.5) = 20\pi \text{ m}^2/\text{min}$$

**21.** $D=\dfrac{P}{A}$. Given $P=5000$, $\dfrac{dP}{dt}=200$, $A=25$, $\dfrac{dA}{dt}=3$.

Using the quotient rule with respect to $t$:

$$\frac{dD}{dt} = \frac{\frac{dP}{dt}\cdot A - P\cdot\frac{dA}{dt}}{A^2}$$

$$\frac{dD}{dt} = \frac{(200)(25) - (5000)(3)}{25^2} = \frac{5000-15000}{625} = \frac{-10000}{625} = -16$$

**Answer: population density is currently decreasing at $16$ people per square mile, per year** — even though the population itself is growing, the developed area is growing fast enough to outpace it.

**22.** $V=\dfrac43\pi r^3$. Given $\dfrac{dV}{dt}=100$ ft³/min. Find $\dfrac{dr}{dt}$ at $r=5$.

$$\frac{dV}{dt} = 4\pi r^2\cdot\frac{dr}{dt}$$

$$100 = 4\pi(25)\cdot\frac{dr}{dt} = 100\pi\cdot\frac{dr}{dt}$$

$$\frac{dr}{dt} = \frac{100}{100\pi} = \frac{1}{\pi} \text{ ft/min}$$
