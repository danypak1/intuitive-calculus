# Unit 18: The Mean Value Theorem — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2-4x$ on $[0,4]$

$f$ is a polynomial, so it's continuous and differentiable everywhere — MVT applies.

$f(0)=0$. $f(4)=16-16=0$. Average rate of change: $\dfrac{0-0}{4-0}=0$.

$f'(x)=2x-4$. Set $2x-4=0 \Rightarrow x=2$.

**$c=2$**, which lies in $(0,4)$. ✓

**2.** $f(x)=x^2+2x$ on $[-1,3]$

$f(-1)=1-2=-1$. $f(3)=9+6=15$. Average rate: $\dfrac{15-(-1)}{3-(-1)} = \dfrac{16}{4}=4$.

$f'(x)=2x+2$. Set $2x+2=4 \Rightarrow x=1$.

**$c=1$**, which lies in $(-1,3)$. ✓

**3.** $f(x)=x^3$ on $[0,2]$

$f(0)=0$. $f(2)=8$. Average rate: $\dfrac{8-0}{2-0}=4$.

$f'(x)=3x^2$. Set $3x^2=4 \Rightarrow x^2=\dfrac43 \Rightarrow x=\dfrac{2}{\sqrt3}=\dfrac{2\sqrt3}{3}$.

**$c=\dfrac{2\sqrt3}{3}\approx1.155$**, which lies in $(0,2)$. ✓

**4.** $f(x)=x^2-1$ on $[1,3]$

$f(1)=0$. $f(3)=8$. Average rate: $\dfrac{8-0}{3-1}=4$.

$f'(x)=2x$. Set $2x=4 \Rightarrow x=2$.

**$c=2$**, which lies in $(1,3)$. ✓

**5.** $f(x)=x^2-4x+3$ on $[1,3]$

$f(1)=1-4+3=0$. $f(3)=9-12+3=0$. Since $f(1)=f(3)$, this is a Rolle's Theorem scenario.

$f'(x)=2x-4$. Set $2x-4=0 \Rightarrow x=2$.

**$c=2$**, which lies in $(1,3)$. ✓

**6.** $f(x)=2x^2-3x$ on $[0,2]$

$f(0)=0$. $f(2)=8-6=2$. Average rate: $\dfrac{2-0}{2-0}=1$.

$f'(x)=4x-3$. Set $4x-3=1 \Rightarrow 4x=4 \Rightarrow x=1$.

**$c=1$**, which lies in $(0,2)$. ✓

---

### 🟡 Standard

**7.** $f(x)=x^3-3x$ on $[-1,2]$

$f(-1)=-1+3=2$. $f(2)=8-6=2$. Since $f(-1)=f(2)$, this is a Rolle's scenario.

$f'(x)=3x^2-3$. Set $3x^2-3=0 \Rightarrow x^2=1 \Rightarrow x=\pm1$.

Check the interval $(-1,2)$: $x=1$ lies inside; $x=-1$ is the **endpoint itself**, not inside the open interval, so it's discarded.

**$c=1$** (only).

**8.** $f(x)=\dfrac1x$ on $[1,3]$

Since $0$ is not in $[1,3]$, $f$ is continuous and differentiable throughout — MVT applies.

$f(1)=1$. $f(3)=\dfrac13$. Average rate: $\dfrac{\frac13-1}{3-1} = \dfrac{-\frac23}{2} = -\dfrac13$.

$f'(x)=-\dfrac{1}{x^2}$. Set $-\dfrac{1}{x^2}=-\dfrac13 \Rightarrow x^2=3 \Rightarrow x=\sqrt3$ (taking the positive root, since we're working in $[1,3]$).

**$c=\sqrt3\approx1.732$**, which lies in $(1,3)$. ✓

**9.** $f(x)=x^3-x$ on $[-1,1]$

$f(-1)=-1+1=0$. $f(1)=1-1=0$. Rolle's scenario.

$f'(x)=3x^2-1$. Set $3x^2-1=0 \Rightarrow x^2=\dfrac13 \Rightarrow x=\pm\dfrac{1}{\sqrt3}=\pm\dfrac{\sqrt3}{3}$.

Both values lie inside $(-1,1)$.

**$c=\dfrac{\sqrt3}{3}$ and $c=-\dfrac{\sqrt3}{3}$** (both valid).

**10.** $f(x)=\sqrt{x}$ on $[0,4]$

$f$ is continuous on $[0,4]$ and differentiable on the open interval $(0,4)$ (the derivative is undefined only at the endpoint $x=0$, which doesn't affect the open-interval requirement) — MVT applies.

$f(0)=0$. $f(4)=2$. Average rate: $\dfrac{2-0}{4-0}=\dfrac12$.

$f'(x)=\dfrac{1}{2\sqrt{x}}$. Set $\dfrac{1}{2\sqrt{x}}=\dfrac12 \Rightarrow 2\sqrt{x}=2 \Rightarrow \sqrt{x}=1 \Rightarrow x=1$.

**$c=1$**, which lies in $(0,4)$. ✓

**11.** $f(x)=\sin x$ on $[0,\pi]$

$f(0)=0$. $f(\pi)=0$. Rolle's scenario.

$f'(x)=\cos x$. Set $\cos x=0$. Within $(0,\pi)$, the only solution is $x=\dfrac{\pi}{2}$.

**$c=\dfrac{\pi}{2}$.**

**12.** $f(x)=x^2-6x+5$ on $[0,6]$

$f(0)=5$. $f(6)=36-36+5=5$. Rolle's scenario.

$f'(x)=2x-6$. Set $2x-6=0 \Rightarrow x=3$.

**$c=3$**, which lies in $(0,6)$. ✓

---

### 🔴 Challenge

**13.** $f(x)=\dfrac1x$ on $[-1,1]$

**MVT does not apply.** The function $f(x)=\dfrac1x$ is **not continuous** at $x=0$ (it's not even defined there — division by zero), and $x=0$ lies right inside the interval $[-1,1]$. Since continuity on the entire closed interval is a required hypothesis, and it fails at this interior point, we cannot use MVT here at all — there's no guarantee that a value $c$ with the required property exists.

**14.** $f(x)=|x|$ on $[-2,2]$

**MVT does not apply.** The function $f(x)=|x|$ is continuous everywhere (no breaks), but it is **not differentiable** at $x=0$ — it has a sharp corner there, as we established back in Unit 7. Since $x=0$ lies inside the open interval $(-2,2)$, and differentiability on the entire open interval is a required hypothesis, this hypothesis fails, so MVT's guarantee does not apply.

**15.** $f(x)=x^3-3x^2+2$ on $[0,3]$

$f(0)=2$. $f(3)=27-27+2=2$. Rolle's scenario.

$f'(x)=3x^2-6x=3x(x-2)$. Set $3x(x-2)=0 \Rightarrow x=0$ or $x=2$.

Check the open interval $(0,3)$: $x=0$ is the **endpoint itself**, so it's discarded. $x=2$ lies inside $(0,3)$.

**$c=2$** (only).

**16.** Suppose $f'(x)\le 2$ everywhere, with $f(0)=0$ and $f(3)=10$.

By the Mean Value Theorem (assuming $f$ is differentiable everywhere, which makes it automatically continuous too), there must exist some $c$ in $(0,3)$ such that:

$$f'(c) = \frac{f(3)-f(0)}{3-0} = \frac{10-0}{3} = \frac{10}{3} \approx 3.33$$

But we assumed $f'(x)\le 2$ for **every** value of $x$, including $x=c$. This means we'd need $f'(c)\le 2$ **and** $f'(c)=\dfrac{10}{3}$ at the same time — but $\dfrac{10}{3} > 2$, which is a direct contradiction.

**Conclusion: no such function can exist.** A function whose derivative never exceeds $2$ anywhere simply cannot climb from $f(0)=0$ up to $f(3)=10$ — that would require an average rate of change of $\dfrac{10}{3}$, which is faster than the derivative is ever allowed to be.

**17.** $f$ continuous on $[1,5]$, differentiable on $(1,5)$, $f(1)=3$, $f(5)=15$.

Average rate of change: $\dfrac{15-3}{5-1} = \dfrac{12}{4}=3$.

By MVT, there exists some $c$ in $(1,5)$ such that $f'(c)=3$.

**In words:** if $f'(x)$ stayed strictly *below* $3$ for the entire interval, the function couldn't possibly climb fast enough on average to go from $3$ up to $15$ — its overall average rate would necessarily be less than $3$, contradicting the actual computed average of exactly $3$. Likewise, if $f'(x)$ stayed strictly *above* $3$ the whole time, the function would climb too fast on average, again contradicting the true average. So the derivative is forced to actually equal $3$ at some point in between — it can't just hover above or below that value forever.

---

### 🌍 Applied

**18.** A car travels $150$ miles in $3$ hours.

Average velocity $=\dfrac{150}{3}=50$ mph.

Let $s(t)$ be the car's position, a continuous and differentiable function of time (a reasonable physical assumption — a car's position doesn't teleport or jump). By the Mean Value Theorem, there must exist some time $c$ during the $3$-hour trip where

$$s'(c) = 50 \text{ mph}$$

**Since $s'(t)$ represents the car's instantaneous velocity (what the speedometer reads), this guarantees the speedometer read exactly $50$ mph at some instant during the drive** — no matter how the car sped up, slowed down, or varied its speed throughout the trip.

**19.** Profit $P(0)=200$, $P(12)=1400$.

Average rate of change: $\dfrac{1400-200}{12-0} = \dfrac{1200}{12}=100$ dollars/month.

By MVT, there exists some $c$ in $(0,12)$ such that $P'(c)=100$.

**This guarantees there was some specific moment during the year when the company's profit was growing at an instantaneous rate of exactly $\$100$ per month.**

**20.** A $10$ km race completed in $40$ minutes.

Convert $40$ minutes to hours: $40 \div 60 = \dfrac{2}{3}$ hour.

Average speed: $\dfrac{10}{2/3} = 10\times\dfrac32 = 15$ km/h.

By MVT (assuming the runner's position is a continuous, differentiable function of time — a reasonable assumption for a real race), there must exist some instant during the race where the runner's instantaneous speed was exactly $15$ km/h.

**21.** $h(0)=0$, $h(10)=2000$.

Average velocity: $\dfrac{2000-0}{10-0} = 200$ ft/s.

By MVT, there exists some $c$ in $(0,10)$ such that $h'(c)=200$.

**This means at some moment during the $10$-second flight, the rocket's instantaneous velocity was exactly $200$ ft/s** — it couldn't have stayed entirely above or entirely below that value the whole time and still average out to $200$ ft/s overall.
