# Unit 22: Newton's Method — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2-2$, $f'(x)=2x$, $x_0=1$.

$f(1)=1-2=-1$. $f'(1)=2$.

$$x_1 = 1 - \frac{-1}{2} = 1+0.5 = 1.5$$

**$x_1=1.5$.**

**2.** $f(x)=x^2-5$, $f'(x)=2x$, $x_0=2$.

$f(2)=4-5=-1$. $f'(2)=4$.

$$x_1 = 2-\frac{-1}{4} = 2+0.25 = 2.25$$

**$x_1=2.25$.**

**3.** $f(x)=x^3-2$, $f'(x)=3x^2$, $x_0=1$.

$f(1)=1-2=-1$. $f'(1)=3$.

$$x_1 = 1-\frac{-1}{3} = 1+\frac13 = \frac43 \approx 1.3333$$

**$x_1=\dfrac43\approx1.3333$.**

**4.** $f(x)=x^2-10$, $f'(x)=2x$, $x_0=3$.

$f(3)=9-10=-1$. $f'(3)=6$.

$$x_1 = 3-\frac{-1}{6} = 3+\frac16 = \frac{19}{6} \approx 3.1667$$

**$x_1=\dfrac{19}{6}\approx3.1667$.**

**5.** $f(x)=x^3-8$, $f'(x)=3x^2$, $x_0=3$.

$f(3)=27-8=19$. $f'(3)=27$.

$$x_1 = 3-\frac{19}{27} = \frac{81-19}{27} = \frac{62}{27} \approx 2.2963$$

**$x_1=\dfrac{62}{27}\approx2.2963$.**

**6.** $f(x)=x^2-7$, $f'(x)=2x$, $x_0=3$.

$f(3)=9-7=2$. $f'(3)=6$.

$$x_1 = 3-\frac{2}{6} = 3-\frac13 = \frac83 \approx 2.6667$$

**$x_1=\dfrac83\approx2.6667$.**

---

### 🟡 Standard

**7.** $f(x)=x^2-3$, $f'(x)=2x$, $x_0=2$.

$f(2)=4-3=1$. $f'(2)=4$.

$$x_1 = 2-\frac14 = 1.75$$

$f(1.75)=3.0625-3=0.0625$. $f'(1.75)=3.5$.

$$x_2 = 1.75-\frac{0.0625}{3.5} = 1.75-0.017857 \approx 1.732143$$

**$x_1=1.75$; $x_2\approx1.732143$** (the true value of $\sqrt3\approx1.732051$ — very close already).

**8.** $f(x)=x^3-5$, $f'(x)=3x^2$, $x_0=2$.

$f(2)=8-5=3$. $f'(2)=12$.

$$x_1 = 2-\frac{3}{12} = 2-0.25=1.75$$

$f(1.75)=1.75^3-5=5.359375-5=0.359375$. $f'(1.75)=3(1.75)^2=3(3.0625)=9.1875$.

$$x_2 = 1.75-\frac{0.359375}{9.1875} \approx 1.75-0.039122 \approx 1.710878$$

**$x_1=1.75$; $x_2\approx1.710878$** (true value $\sqrt[3]{5}\approx1.709976$).

**9.** $f(x)=x^2+x-6$, $f'(x)=2x+1$, $x_0=1$.

$f(1)=1+1-6=-4$. $f'(1)=3$.

$$x_1 = 1-\frac{-4}{3} = 1+\frac43 = \frac73 \approx 2.3333$$

$f\left(\frac73\right) = \frac{49}{9}+\frac73-6 = \frac{49}{9}+\frac{21}{9}-\frac{54}{9}=\frac{16}{9}$. $f'\left(\frac73\right)=2\left(\frac73\right)+1=\frac{14}{3}+1=\frac{17}{3}$.

$$x_2 = \frac73 - \frac{16/9}{17/3} = \frac73 - \frac{16}{9}\cdot\frac{3}{17} = \frac73-\frac{48}{153} = \frac73-\frac{16}{51}$$

Convert $\frac73$ to fifty-firsts: $\frac{7}{3}=\frac{119}{51}$.

$$x_2 = \frac{119}{51}-\frac{16}{51} = \frac{103}{51} \approx 2.0196$$

**$x_1=\dfrac73\approx2.3333$; $x_2\approx2.0196$** (converging nicely toward the true root $x=2$).

**10.** $f(x)=\cos x - x$, $f'(x)=-\sin x - 1$, $x_0=1$.

$f(1)=\cos(1)-1\approx0.5403-1=-0.4597$. $f'(1)=-\sin(1)-1\approx-0.8415-1=-1.8415$.

$$x_1 = 1-\frac{-0.4597}{-1.8415} = 1-0.2497 \approx 0.7503$$

**$x_1\approx0.7503$** (the true fixed point is $\approx0.739085$ — already quite close after one step).

**11.** $f(x)=x^3-x-1$, $f'(x)=3x^2-1$, $x_0=1$.

$f(1)=1-1-1=-1$. $f'(1)=3-1=2$.

$$x_1 = 1-\frac{-1}{2} = 1.5$$

$f(1.5)=3.375-1.5-1=0.875$. $f'(1.5)=3(2.25)-1=5.75$.

$$x_2 = 1.5-\frac{0.875}{5.75} \approx 1.5-0.152174 \approx 1.347826$$

**$x_1=1.5$; $x_2\approx1.347826$** (true root $\approx1.324718$, still converging).

**12.** $f(x)=x^2-6$, $f'(x)=2x$, $x_0=2$.

$f(2)=4-6=-2$. $f'(2)=4$.

$$x_1 = 2-\frac{-2}{4} = 2+0.5=2.5$$

$f(2.5)=6.25-6=0.25$. $f'(2.5)=5$.

$$x_2 = 2.5-\frac{0.25}{5} = 2.5-0.05=2.45$$

**$x_1=2.5$; $x_2=2.45$** (true value $\sqrt6\approx2.449490$ — extremely close already).

---

### 🔴 Challenge

**13.** $f(x)=x^4-2$, $f'(x)=4x^3$, $x_0=1$.

$f(1)=1-2=-1$. $f'(1)=4$.

$$x_1 = 1-\frac{-1}{4} = 1+0.25 = 1.25$$

**$x_1=1.25$.**

**14.** $f(x)=x^4-2$, $f'(x)=4x^3$, $x_0=1$. (Same setup as Problem 13.)

$x_1=1.25$ (from Problem 13).

$f(1.25)=(1.25)^4-2$. Compute step by step: $1.25^2=1.5625$; $1.25^4=(1.5625)^2=2.44140625$. So $f(1.25)=2.44140625-2=0.44140625$.

$f'(1.25)=4(1.25)^3=4(1.953125)=7.8125$.

$$x_2 = 1.25-\frac{0.44140625}{7.8125} \approx 1.25-0.0565 \approx 1.1935$$

**$x_1=1.25$; $x_2\approx1.1935$** (the true value of $\sqrt[4]{2}\approx1.189207$ — converging fast).

**15.** $f(x)=x^5-3$, $f'(x)=5x^4$, $x_0=1$.

$f(1)=1-3=-2$. $f'(1)=5$.

$$x_1 = 1-\frac{-2}{5} = 1+0.4=1.4$$

Compute $f(1.4)$: $1.4^2=1.96$, $1.4^3=2.744$, $1.4^4=3.8416$, $1.4^5=5.37824$. So $f(1.4)=5.37824-3=2.37824$.

$f'(1.4)=5(3.8416)=19.208$.

$$x_2 = 1.4-\frac{2.37824}{19.208} \approx 1.4-0.123807 \approx 1.276193$$

**$x_1=1.4$; $x_2\approx1.276193$** (the true value of $\sqrt[5]{3}\approx1.245731$, still converging).

**16.** What goes wrong if $f'(x_0)=0$?

Looking at the formula:

$$x_1 = x_0 - \frac{f(x_0)}{f'(x_0)}$$

If $f'(x_0)=0$, this requires dividing by $0$, which is **undefined** — the formula breaks down completely and cannot produce a next guess at all.

**Geometrically:** a derivative of $0$ means the tangent line at $x_0$ is perfectly **horizontal**. A horizontal line either never crosses the x-axis (if it's not already sitting on it) or lies exactly along the x-axis (an extremely rare coincidence) — either way, there's no well-defined single crossing point for the method to use as its next guess. In practice, if this happens, you simply need to choose a different starting guess where the derivative isn't zero.

**17.** $f(x)=\sin x$, $f'(x)=\cos x$, $x_0=3$.

$f(3)=\sin(3)\approx0.14112$. $f'(3)=\cos(3)\approx-0.98999$.

$$x_1 = 3-\frac{0.14112}{-0.98999} \approx 3+0.14255 \approx 3.14255$$

Now for $x_2$: $x_1\approx3.14255$ is already very close to $\pi\approx3.14159265$.

$f(3.14255)=\sin(3.14255)$. Since $3.14255-\pi\approx0.00096$, and $\sin(\pi+\varepsilon)\approx-\varepsilon$ for small $\varepsilon$: $f(3.14255)\approx-0.00096$.

$f'(3.14255)=\cos(3.14255)\approx\cos(\pi+0.00096)\approx-1$ (very close to $-1$).

$$x_2 = 3.14255 - \frac{-0.00096}{-1} \approx 3.14255-0.00096 \approx 3.14159$$

**$x_1\approx3.14255$; $x_2\approx3.14159$** — remarkably close to the true value of $\pi\approx3.14159265$ after just two iterations, showing how quickly Newton's Method can converge.

---

### 🌍 Applied

**18.** Approximate $\sqrt7$: $f(x)=x^2-7$, $f'(x)=2x$, $x_0=2.5$.

$f(2.5)=6.25-7=-0.75$. $f'(2.5)=5$.

$$x_1 = 2.5-\frac{-0.75}{5} = 2.5+0.15 = 2.65$$

**$x_1=2.65$** (true value $\sqrt7\approx2.645751$ — very close).

**19.** $f(x)=x^2-50x+200$, $f'(x)=2x-50$, $x_0=5$.

$f(5)=25-250+200=-25$. $f'(5)=10-50=-40$.

$$x_1 = 5-\frac{-25}{-40} = 5-0.625 = 4.375$$

**Answer: $x_1=4.375$ units** — this approximates the lower break-even production level. (Using the quadratic formula for comparison, the exact lower root is $\dfrac{50-\sqrt{1700}}{2}\approx4.3846$ — Newton's Method already lands remarkably close after a single step.)

**20.** $f(x)=x^3-2x-5$, $f'(x)=3x^2-2$, $x_0=2$.

$f(2)=8-4-5=-1$. $f'(2)=12-2=10$.

$$x_1 = 2-\frac{-1}{10} = 2+0.1=2.1$$

$f(2.1)=9.261-4.2-5=0.061$. $f'(2.1)=3(4.41)-2=13.23-2=11.23$.

$$x_2 = 2.1-\frac{0.061}{11.23} \approx 2.1-0.005432 \approx 2.094568$$

**$x_1=2.1$; $x_2\approx2.094568$** (the true root is $\approx2.0945515$ — this is actually the exact historical example Isaac Newton himself first used to demonstrate the method!).

**21.** Approximate $\sqrt[3]{10}$: $f(x)=x^3-10$, $f'(x)=3x^2$, $x_0=2$.

$f(2)=8-10=-2$. $f'(2)=12$.

$$x_1 = 2-\frac{-2}{12} = 2+\frac16 = \frac{13}{6} \approx 2.1667$$

**$x_1=\dfrac{13}{6}\approx2.1667$** (true value $\sqrt[3]{10}\approx2.15443$ — already close after one step).
