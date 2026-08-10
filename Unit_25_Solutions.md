# Unit 25: Sigma Notation and Limits of Finite Sums — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\sum_{i=1}^{5} i = 1+2+3+4+5 = 15$

**2.** $\displaystyle\sum_{i=1}^{4} i^2 = 1+4+9+16 = 30$

**3.** $\displaystyle\sum_{i=1}^{4} (2i+1)$: at $i=1,2,3,4$: $3,5,7,9$.

$$3+5+7+9 = 24$$

**4.** $\displaystyle\sum_{i=1}^{3} i^3 = 1+8+27 = 36$

**5.** $\displaystyle\sum_{i=1}^{6} 3 = 3\times6 = 18$

**6.** $\displaystyle\sum_{i=1}^{5} (i-1)$: at $i=1,2,3,4,5$: $0,1,2,3,4$.

$$0+1+2+3+4 = 10$$

---

### 🟡 Standard

**7.** $\displaystyle\sum_{i=1}^{10} i = \frac{10(11)}{2} = 55$

**8.** $\displaystyle\sum_{i=1}^{10} i^2 = \frac{10(11)(21)}{6} = \frac{2310}{6} = 385$

**9.** $\displaystyle\sum_{i=1}^{6} i^3 = \left[\frac{6(7)}{2}\right]^2 = [21]^2 = 441$

**10.** $\displaystyle\sum_{i=1}^{8} (3i-2)$

$$= 3\sum_{i=1}^8 i - \sum_{i=1}^8 2 = 3\left(\frac{8(9)}{2}\right) - 2(8) = 3(36) - 16 = 108-16 = 92$$

**11.** $\displaystyle\sum_{i=1}^{5} (i^2+2i)$

$$= \sum_{i=1}^5 i^2 + 2\sum_{i=1}^5 i = \frac{5(6)(11)}{6} + 2\left(\frac{5(6)}{2}\right) = \frac{330}{6}+2(15) = 55+30 = 85$$

**12.** $\displaystyle\sum_{i=1}^{20} 5 = 5\times20 = 100$

---

### 🔴 Challenge

**13.** Exact area under $f(x)=x^2$ on $[0,3]$.

$\Delta x = \dfrac{3}{n}$, and $x_i = \dfrac{3i}{n}$.

$$f(x_i)\cdot\Delta x = \left(\frac{3i}{n}\right)^2\cdot\frac{3}{n} = \frac{9i^2}{n^2}\cdot\frac{3}{n} = \frac{27i^2}{n^3}$$

$$R_n = \sum_{i=1}^n \frac{27i^2}{n^3} = \frac{27}{n^3}\sum_{i=1}^n i^2 = \frac{27}{n^3}\cdot\frac{n(n+1)(2n+1)}{6} = \frac{27(n+1)(2n+1)}{6n^2}$$

Expand $(n+1)(2n+1) = 2n^2+3n+1$:

$$R_n = \frac{27(2n^2+3n+1)}{6n^2} = \frac{27}{6}\left(2+\frac3n+\frac{1}{n^2}\right) = 4.5\left(2+\frac3n+\frac{1}{n^2}\right)$$

Take the limit as $n\to\infty$ (the $\frac3n$ and $\frac{1}{n^2}$ terms vanish):

$$\lim_{n\to\infty} R_n = 4.5(2) = 9$$

**Exact area $=9$.**

**14.** Exact area under $f(x)=x$ on $[0,4]$.

$\Delta x = \dfrac4n$, $x_i=\dfrac{4i}{n}$.

$$f(x_i)\Delta x = \frac{4i}{n}\cdot\frac4n = \frac{16i}{n^2}$$

$$R_n = \frac{16}{n^2}\sum_{i=1}^n i = \frac{16}{n^2}\cdot\frac{n(n+1)}{2} = \frac{8(n+1)}{n} = 8+\frac8n$$

$$\lim_{n\to\infty} R_n = 8$$

**Exact area $=8$.**

**15.** Exact area under $f(x)=2x+1$ on $[0,2]$.

$\Delta x=\dfrac2n$, $x_i=\dfrac{2i}{n}$.

$$f(x_i) = 2\left(\frac{2i}{n}\right)+1 = \frac{4i}{n}+1$$

$$f(x_i)\Delta x = \left(\frac{4i}{n}+1\right)\cdot\frac2n = \frac{8i}{n^2}+\frac2n$$

$$R_n = \frac{8}{n^2}\sum_{i=1}^n i + \frac2n\sum_{i=1}^n 1 = \frac{8}{n^2}\cdot\frac{n(n+1)}{2} + \frac2n\cdot n$$

$$= \frac{4(n+1)}{n} + 2 = 4+\frac4n+2 = 6+\frac4n$$

$$\lim_{n\to\infty} R_n = 6$$

**Exact area $=6$.**

**16.** Exact area under $f(x)=x^2$ on $[1,2]$.

$\Delta x = \dfrac1n$, $x_i = 1+\dfrac{i}{n}$.

$$f(x_i) = \left(1+\frac{i}{n}\right)^2 = 1+\frac{2i}{n}+\frac{i^2}{n^2}$$

$$f(x_i)\Delta x = \left(1+\frac{2i}{n}+\frac{i^2}{n^2}\right)\cdot\frac1n = \frac1n+\frac{2i}{n^2}+\frac{i^2}{n^3}$$

$$R_n = \sum_{i=1}^n\frac1n + \frac{2}{n^2}\sum_{i=1}^n i + \frac{1}{n^3}\sum_{i=1}^n i^2$$

$$= n\cdot\frac1n + \frac{2}{n^2}\cdot\frac{n(n+1)}{2} + \frac{1}{n^3}\cdot\frac{n(n+1)(2n+1)}{6}$$

$$= 1 + \frac{n+1}{n} + \frac{(n+1)(2n+1)}{6n^2}$$

Simplify each piece: $\dfrac{n+1}{n} = 1+\dfrac1n$. And $\dfrac{(n+1)(2n+1)}{6n^2} = \dfrac{2n^2+3n+1}{6n^2} = \dfrac13+\dfrac{1}{2n}+\dfrac{1}{6n^2}$.

$$R_n = 1 + \left(1+\frac1n\right) + \left(\frac13+\frac{1}{2n}+\frac{1}{6n^2}\right) = \frac73 + \frac{3}{2n} + \frac{1}{6n^2}$$

$$\lim_{n\to\infty} R_n = \frac73$$

**Exact area $=\dfrac73$.**

**17.** $\displaystyle\lim_{n\to\infty} \frac1n\sum_{i=1}^{n} \left(\frac{i}{n}\right)^2$

Rewrite the summand:

$$\frac1n\left(\frac{i}{n}\right)^2 = \frac{i^2}{n^3}$$

$$\frac1n\sum_{i=1}^n\left(\frac{i}{n}\right)^2 = \frac{1}{n^3}\sum_{i=1}^n i^2 = \frac{1}{n^3}\cdot\frac{n(n+1)(2n+1)}{6} = \frac{(n+1)(2n+1)}{6n^2}$$

Expand: $\dfrac{2n^2+3n+1}{6n^2} = \dfrac13+\dfrac{1}{2n}+\dfrac{1}{6n^2}$.

$$\lim_{n\to\infty}\left(\frac13+\frac{1}{2n}+\frac{1}{6n^2}\right) = \frac13$$

**Answer: $\dfrac13$.** (This is secretly the exact area under $f(x)=x^2$ on $[0,1]$, written entirely in limit-of-sums form.)

---

### 🌍 Applied

**18.** $v(t)=2t$ on $[0,5]$.

$\Delta t = \dfrac5n$, $t_i=\dfrac{5i}{n}$.

$$v(t_i)\Delta t = 2\left(\frac{5i}{n}\right)\cdot\frac5n = \frac{50i}{n^2}$$

$$R_n = \frac{50}{n^2}\sum_{i=1}^n i = \frac{50}{n^2}\cdot\frac{n(n+1)}{2} = \frac{25(n+1)}{n} = 25+\frac{25}{n}$$

$$\lim_{n\to\infty} R_n = 25$$

**Answer: exact total distance $=25$ ft.**

**19.** $r(t)=t^2$ on $[0,4]$.

$\Delta t=\dfrac4n$, $t_i=\dfrac{4i}{n}$.

$$r(t_i)\Delta t = \left(\frac{4i}{n}\right)^2\cdot\frac4n = \frac{16i^2}{n^2}\cdot\frac4n = \frac{64i^2}{n^3}$$

$$R_n = \frac{64}{n^3}\sum_{i=1}^n i^2 = \frac{64}{n^3}\cdot\frac{n(n+1)(2n+1)}{6} = \frac{64(n+1)(2n+1)}{6n^2}$$

Expand: $\dfrac{64(2n^2+3n+1)}{6n^2} = \dfrac{32}{3}\left(2+\dfrac3n+\dfrac{1}{n^2}\right)$.

$$\lim_{n\to\infty} R_n = \frac{32}{3}(2) = \frac{64}{3}$$

**Answer: exact total water collected $=\dfrac{64}{3}$ gallons.**

**20.** $MR(x)=6x$ on $[0,10]$.

$\Delta x=\dfrac{10}{n}$, $x_i=\dfrac{10i}{n}$.

$$MR(x_i)\Delta x = 6\left(\frac{10i}{n}\right)\cdot\frac{10}{n} = \frac{600i}{n^2}$$

$$R_n = \frac{600}{n^2}\sum_{i=1}^n i = \frac{600}{n^2}\cdot\frac{n(n+1)}{2} = \frac{300(n+1)}{n} = 300+\frac{300}{n}$$

$$\lim_{n\to\infty} R_n = 300$$

**Answer: exact total revenue $=\$300$.**

**21.** $v(t)=3t^2$ on $[0,4]$.

$\Delta t = \dfrac4n$, $t_i=\dfrac{4i}{n}$.

$$v(t_i)\Delta t = 3\left(\frac{4i}{n}\right)^2\cdot\frac4n = 3\cdot\frac{16i^2}{n^2}\cdot\frac4n = \frac{192i^2}{n^3}$$

$$R_n = \frac{192}{n^3}\sum_{i=1}^n i^2 = \frac{192}{n^3}\cdot\frac{n(n+1)(2n+1)}{6} = \frac{32(n+1)(2n+1)}{n^2}$$

Expand: $\dfrac{32(2n^2+3n+1)}{n^2} = 32\left(2+\dfrac3n+\dfrac{1}{n^2}\right) = 64+\dfrac{96}{n}+\dfrac{32}{n^2}$.

$$\lim_{n\to\infty} R_n = 64$$

**Answer: exact total distance traveled $=64$ ft.**
