# Unit 16: Linearization and Differentials — Full Solutions

### 🟢 Warm-up

**1.** $f(x)=x^2$ at $a=3$.

$f(3)=9$. $f'(x)=2x$, so $f'(3)=6$.

$$L(x) = 9+6(x-3)$$

Estimate $f(3.1)$: $L(3.1) = 9+6(0.1) = 9+0.6 = 9.6$.

**$L(x)=9+6(x-3)$, and $f(3.1)\approx 9.6$.** (The true value is $9.61$ — very close.)

**2.** $f(x)=x^3$ at $a=2$.

$f(2)=8$. $f'(x)=3x^2$, so $f'(2)=12$.

$$L(x) = 8+12(x-2)$$

Estimate $f(2.05)$: $L(2.05) = 8+12(0.05) = 8+0.6 = 8.6$.

**$L(x)=8+12(x-2)$, and $f(2.05)\approx 8.6$.** (The true value is $8.615125$.)

**3.** $f(x)=\dfrac1x$ at $a=4$.

$f(4)=0.25$. $f'(x)=-\dfrac{1}{x^2}$, so $f'(4)=-\dfrac{1}{16}=-0.0625$.

$$L(x) = 0.25-0.0625(x-4)$$

Estimate $f(4.2)$: $L(4.2) = 0.25-0.0625(0.2) = 0.25-0.0125 = 0.2375$.

**$L(x)=0.25-0.0625(x-4)$, and $f(4.2)\approx 0.2375$.** (The true value is $\approx0.2381$.)

**4.** $f(x)=\sqrt{x}$ at $a=9$.

$f(9)=3$. $f'(x)=\dfrac{1}{2\sqrt{x}}$, so $f'(9)=\dfrac16$.

$$L(x) = 3+\frac16(x-9)$$

Estimate $f(9.3)$: $L(9.3) = 3+\dfrac16(0.3) = 3+0.05 = 3.05$.

**$L(x)=3+\dfrac16(x-9)$, and $\sqrt{9.3}\approx 3.05$.** (The true value is $\approx3.0496$.)

**5.** $f(x)=x^2+3x$ at $a=1$.

$f(1)=1+3=4$. $f'(x)=2x+3$, so $f'(1)=5$.

$$L(x) = 4+5(x-1)$$

Estimate $f(1.1)$: $L(1.1) = 4+5(0.1) = 4+0.5 = 4.5$.

**$L(x)=4+5(x-1)$, and $f(1.1)\approx 4.5$.** (The true value is $4.51$.)

**6.** $f(x)=\sqrt{x}$ at $a=25$.

$f(25)=5$. $f'(25)=\dfrac{1}{2\sqrt{25}}=\dfrac{1}{10}=0.1$.

$$L(x) = 5+0.1(x-25)$$

Estimate $f(24.7)$: here $dx = 24.7-25=-0.3$.

$$L(24.7) = 5+0.1(-0.3) = 5-0.03 = 4.97$$

**$L(x)=5+0.1(x-25)$, and $\sqrt{24.7}\approx 4.97$.** (The true value is $\approx4.9699$.)

---

### 🟡 Standard

**7.** $y=x^3$, $x=2$, $dx=0.1$.

$$dy = f'(x)\,dx = 3x^2\,dx$$

$$dy = 3(2)^2(0.1) = 3(4)(0.1) = 1.2$$

**$dy = 1.2$.**

**8.** $y=\sqrt{x}$, $x=16$, $dx=-0.2$.

$$dy = \frac{1}{2\sqrt{x}}\,dx$$

$$dy = \frac{1}{2\sqrt{16}}(-0.2) = \frac{1}{8}(-0.2) = -0.025$$

**$dy = -0.025$.**

**9.** Estimate $\sqrt{50}$ using $a=49$.

$f(x)=\sqrt{x}$. $f(49)=7$. $f'(49) = \dfrac{1}{2\sqrt{49}} = \dfrac{1}{14}$.

$dx = 50-49=1$.

$$L(50) = 7+\frac{1}{14}(1) = 7+\frac{1}{14} \approx 7+0.0714 = 7.0714$$

**$\sqrt{50}\approx 7.0714$.** (The true value is $\approx7.0711$.)

**10.** Estimate $\sqrt[3]{26}$ using $a=27$.

$f(x)=x^{1/3}$. $f(27)=3$. $f'(x)=\dfrac13x^{-2/3}$, so $f'(27) = \dfrac13(27)^{-2/3} = \dfrac13\cdot\dfrac19 = \dfrac{1}{27}$.

$dx = 26-27=-1$.

$$L(26) = 3+\frac{1}{27}(-1) = 3-\frac{1}{27} \approx 3-0.037 = 2.963$$

**$\sqrt[3]{26}\approx 2.963$.** (The true value is $\approx2.9625$.)

**11.** $y=\dfrac{1}{x^2}=x^{-2}$, $x=5$, $dx=0.05$.

$$f'(x) = -2x^{-3} = -\frac{2}{x^3}$$

$$dy = -\frac{2}{5^3}(0.05) = -\frac{2}{125}(0.05) = -0.016(0.05) = -0.0008$$

**$dy = -0.0008$.**

**12.** Estimate $(3.98)^2$ using $a=4$.

$f(x)=x^2$. $f(4)=16$. $f'(4)=8$.

$dx = 3.98-4=-0.02$.

$$L(3.98) = 16+8(-0.02) = 16-0.16 = 15.84$$

**$(3.98)^2 \approx 15.84$.** (The true value is $15.8404$ — an excellent match.)

---

### 🔴 Challenge

**13.** Sphere, $V=\dfrac43\pi r^3$, $r=10$, $dr=\pm0.1$.

$$dV = 4\pi r^2\,dr$$

$$dV = 4\pi(10)^2(0.1) = 4\pi(100)(0.1) = 40\pi \approx 125.66 \text{ cm}^3$$

**The estimated possible error in the computed volume is about $40\pi \approx 125.7$ cm³.**

**14.** Circle, $A=\pi r^2$, $r=5$, $dr=\pm0.05$.

$$dA = 2\pi r\,dr = 2\pi(5)(0.05) = 0.5\pi \approx 1.5708 \text{ cm}^2$$

Percentage error: divide $dA$ by the actual area $A=\pi(5)^2=25\pi$, then multiply by $100\%$:

$$\frac{dA}{A}\times 100\% = \frac{0.5\pi}{25\pi}\times 100\% = \frac{0.5}{25}\times 100\% = 2\%$$

**The estimated error in the computed area is about $1.57$ cm², or approximately $2\%$.**

**15.** $f(x)=\tan x$ at $a=\dfrac{\pi}{4}$.

$f\left(\dfrac{\pi}{4}\right) = \tan\left(\dfrac{\pi}{4}\right) = 1$.

$f'(x)=\sec^2x$. At $x=\dfrac{\pi}{4}$: $\cos\left(\dfrac{\pi}{4}\right)=\dfrac{\sqrt2}{2}$, so $\cos^2\left(\dfrac{\pi}{4}\right)=\dfrac12$, and $\sec^2\left(\dfrac{\pi}{4}\right) = \dfrac{1}{1/2}=2$.

$$L(x) = 1+2\left(x-\frac{\pi}{4}\right)$$

Estimate $f\left(\dfrac{\pi}{4}+0.01\right)$: here $dx=0.01$.

$$L\left(\frac{\pi}{4}+0.01\right) = 1+2(0.01) = 1.02$$

**$\tan\left(\dfrac{\pi}{4}+0.01\right) \approx 1.02$.** (The true value is $\approx1.0203$.)

**16.** $f(x)=\sin x$ at $a=0$.

$f(0)=0$. $f'(x)=\cos x$, so $f'(0)=1$.

$$L(x) = 0+1(x-0) = x$$

Estimate $\sin(0.05)$: $L(0.05)=0.05$.

**$\sin(0.05)\approx 0.05$.** (The true value is $\approx0.049979$ — remarkably close. This is the classic "small angle approximation" $\sin x \approx x$ for small $x$ measured in radians.)

**17.** Cube, $V=s^3$, $s=6$, $ds=\pm0.05$.

$$dV = 3s^2\,ds = 3(6)^2(0.05) = 3(36)(0.05) = 5.4 \text{ cm}^3$$

Percentage error: the actual volume is $V=6^3=216$ cm³.

$$\frac{dV}{V}\times 100\% = \frac{5.4}{216}\times 100\% = 2.5\%$$

**The estimated error in the computed volume is about $5.4$ cm³, or approximately $2.5\%$.**

---

### 🌍 Applied

**18.** $C(x)=0.01x^2+5x+200$.

$$C'(x) = 0.02x+5$$

At $x=100$: $C'(100) = 0.02(100)+5 = 2+5 = 7$.

Using the differential with $dx=1$:

$$dC = 7(1) = 7$$

**Estimated change: $\$7$.**

Now the exact change: $C(100) = 0.01(10000)+500+200 = 100+500+200=800$. $C(101) = 0.01(10201)+505+200 = 102.01+505+200 = 807.01$.

$$\Delta C = 807.01-800 = 7.01$$

**Comparison: the differential estimate ($\$7.00$) is extremely close to the exact change ($\$7.01$).**

**19.** $P(t)=500+20t+t^2$.

$$P'(t) = 20+2t$$

At $t=10$: $P'(10) = 20+20 = 40$.

Using $dt=0.2$:

$$dP = 40(0.2) = 8$$

**Estimated change in population: about $8$ individuals.**

**20.** $h(t)=-16t^2+200t+10$.

$$h'(t) = -32t+200$$

At $t=3$: $h'(3) = -96+200 = 104$.

Using $dt=0.1$:

$$dh = 104(0.1) = 10.4$$

**Estimated change in height: about $10.4$ feet.**

**21.** $R(x)=100x-0.5x^2$.

$$R'(x) = 100-x$$

At $x=50$: $R'(50) = 100-50 = 50$.

Using $dx=1$:

$$dR = 50(1) = 50$$

**Estimated change: $\$50$.**

Now the exact change: $R(50) = 100(50)-0.5(2500) = 5000-1250=3750$. $R(51) = 100(51)-0.5(2601) = 5100-1300.5=3799.5$.

$$\Delta R = 3799.5-3750 = 49.5$$

**Comparison: the differential estimate ($\$50.00$) is very close to the exact change ($\$49.50$) — the small gap is expected since $dx=1$ isn't infinitesimally small, but the estimate is still quite good.**
