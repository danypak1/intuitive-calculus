# Unit 40: Integration by Partial Fractions — Full Solutions

### 🟢 Warm-up

**1.** $\displaystyle\int \frac{dx}{(x-1)(x+1)}$

Decompose: $\dfrac{1}{(x-1)(x+1)} = \dfrac{A}{x-1}+\dfrac{B}{x+1}$. Clear denominators: $1=A(x+1)+B(x-1)$.

$x=1$: $1=2A \Rightarrow A=\frac12$. $x=-1$: $1=-2B \Rightarrow B=-\frac12$.

$$\int \frac{dx}{(x-1)(x+1)} = \frac12\ln|x-1| - \frac12\ln|x+1| + C = \frac12\ln\left|\frac{x-1}{x+1}\right|+C$$

**2.** $\displaystyle\int \frac{dx}{(x-2)(x+3)}$

$1=A(x+3)+B(x-2)$. $x=2$: $1=5A\Rightarrow A=\frac15$. $x=-3$: $1=-5B\Rightarrow B=-\frac15$.

$$= \frac15\ln|x-2| - \frac15\ln|x+3| + C$$

**3.** $\displaystyle\int \frac{3x+5}{(x+1)(x+2)}\,dx$

$3x+5=A(x+2)+B(x+1)$. $x=-1$: $2=A\Rightarrow A=2$. $x=-2$: $-1=-B\Rightarrow B=1$.

$$= 2\ln|x+1| + \ln|x+2| + C$$

**4.** $\displaystyle\int \frac{5x-1}{(x-1)(x-3)}\,dx$

$5x-1=A(x-3)+B(x-1)$. $x=1$: $4=-2A\Rightarrow A=-2$. $x=3$: $14=2B\Rightarrow B=7$.

$$= -2\ln|x-1| + 7\ln|x-3| + C$$

**5.** $\displaystyle\int \frac{dx}{x^2-4}$

$x^2-4=(x-2)(x+2)$. $1=A(x+2)+B(x-2)$. $x=2$: $A=\frac14$. $x=-2$: $B=-\frac14$.

$$= \frac14\ln|x-2| - \frac14\ln|x+2| + C$$

**6.** $\displaystyle\int \frac{x+7}{x^2+x-6}\,dx$

Factor: $x^2+x-6=(x+3)(x-2)$. $x+7=A(x-2)+B(x+3)$. $x=-3$: $4=-5A\Rightarrow A=-\frac45$. $x=2$: $9=5B\Rightarrow B=\frac95$.

$$= -\frac45\ln|x+3| + \frac95\ln|x-2| + C$$

---

### 🟡 Standard

**7.** $\displaystyle\int \frac{dx}{(x-1)^2(x+1)}$

Decompose: $\dfrac{1}{(x-1)^2(x+1)} = \dfrac{A}{x-1}+\dfrac{B}{(x-1)^2}+\dfrac{C}{x+1}$.

Clear: $1 = A(x-1)(x+1) + B(x+1) + C(x-1)^2$.

$x=1$: $1=2B\Rightarrow B=\frac12$. $x=-1$: $1=4C\Rightarrow C=\frac14$.

Plug $x=0$ to find $A$: $1=A(-1)(1)+B(1)+C(1) = -A+B+C = -A+\frac12+\frac14 = -A+\frac34$. So $A=\frac34-1=-\frac14$.

$$\int \frac{dx}{(x-1)^2(x+1)} = -\frac14\ln|x-1| - \frac{1}{2(x-1)} + \frac14\ln|x+1| + C$$

**8.** $\displaystyle\int \frac{3x-1}{x^2(x+1)}\,dx$

Decompose: $\dfrac{3x-1}{x^2(x+1)} = \dfrac{A}{x}+\dfrac{B}{x^2}+\dfrac{C}{x+1}$.

Clear: $3x-1 = Ax(x+1) + B(x+1) + Cx^2$.

$x=0$: $-1=B\Rightarrow B=-1$. $x=-1$: $-4=C\Rightarrow C=-4$.

Plug $x=1$: $2=A(1)(2)+B(2)+C(1) = 2A+2B+C = 2A-2-4=2A-6$. So $2A=8\Rightarrow A=4$.

$$\int \frac{3x-1}{x^2(x+1)}\,dx = 4\ln|x| + \frac1x - 4\ln|x+1| + C$$

**9.** $\displaystyle\int \frac{dx}{(x-1)(x-2)(x-3)}$

Decompose: $\dfrac{A}{x-1}+\dfrac{B}{x-2}+\dfrac{C}{x-3}$. Clear: $1=A(x-2)(x-3)+B(x-1)(x-3)+C(x-1)(x-2)$.

$x=1$: $1=2A\Rightarrow A=\frac12$. $x=2$: $1=-B\Rightarrow B=-1$. $x=3$: $1=2C\Rightarrow C=\frac12$.

$$= \frac12\ln|x-1| - \ln|x-2| + \frac12\ln|x-3| + C$$

**10.** $\displaystyle\int \frac{2x+1}{(x-2)^2(x+1)}\,dx$

Decompose: $\dfrac{A}{x-2}+\dfrac{B}{(x-2)^2}+\dfrac{C}{x+1}$. Clear: $2x+1=A(x-2)(x+1)+B(x+1)+C(x-2)^2$.

$x=2$: $5=3B\Rightarrow B=\frac53$. $x=-1$: $-1=9C\Rightarrow C=-\frac19$.

Plug $x=0$: $1=A(-2)(1)+B(1)+C(4) = -2A+B+4C = -2A+\frac53-\frac49$.

Convert to ninths: $\frac53=\frac{15}{9}$, so $-2A+\frac{15}{9}-\frac{4}{9}=-2A+\frac{11}{9}$. Set equal to $1=\frac99$: $-2A=\frac99-\frac{11}{9}=-\frac29 \Rightarrow A=\frac19$.

$$\int \frac{2x+1}{(x-2)^2(x+1)}\,dx = \frac19\ln|x-2| - \frac{5}{3(x-2)} - \frac19\ln|x+1| + C$$

**11.** Long division: $\dfrac{x^3+2x^2-5}{x+3}$

$$x^3+2x^2+0x-5 \div (x+3)$$

$x^3\div x=x^2$; $x^2(x+3)=x^3+3x^2$; subtract: $(x^3+2x^2)-(x^3+3x^2)=-x^2$, bring down $0x$: $-x^2+0x$.

$-x^2\div x=-x$; $-x(x+3)=-x^2-3x$; subtract: $(-x^2+0x)-(-x^2-3x)=3x$, bring down $-5$: $3x-5$.

$3x\div x=3$; $3(x+3)=3x+9$; subtract: $(3x-5)-(3x+9)=-14$.

$$\frac{x^3+2x^2-5}{x+3} = x^2-x+3 - \frac{14}{x+3}$$

**12.** $\displaystyle\int \frac{x^2+1}{x-1}\,dx$

Long division: $x^2+0x+1 \div (x-1)$.

$x^2\div x=x$; $x(x-1)=x^2-x$; subtract: $(x^2+0x)-(x^2-x)=x$, bring down $1$: $x+1$.

$x\div x=1$; $1(x-1)=x-1$; subtract: $(x+1)-(x-1)=2$.

$$\frac{x^2+1}{x-1} = x+1+\frac{2}{x-1}$$

$$\int \frac{x^2+1}{x-1}\,dx = \int \left(x+1+\frac{2}{x-1}\right)dx = \frac{x^2}{2}+x+2\ln|x-1|+C$$

---

### 🔴 Challenge

**13.** $\displaystyle\int \frac{2x-6}{x^2-6x+8}\,dx$

Notice: $\dfrac{d}{dx}[x^2-6x+8] = 2x-6$ — an **exact match** with the numerator! No partial fractions needed:

$$\int \frac{2x-6}{x^2-6x+8}\,dx = \ln|x^2-6x+8|+C$$

(Since $x^2-6x+8=(x-2)(x-4)$, this is equivalent to $\ln|(x-2)(x-4)|+C$.)

**14.** $\displaystyle\int \frac{2x-7}{x^2-7x+12}\,dx$

Notice: $\dfrac{d}{dx}[x^2-7x+12]=2x-7$ — another exact match!

$$\int \frac{2x-7}{x^2-7x+12}\,dx = \ln|x^2-7x+12|+C$$

(Equivalent to $\ln|(x-3)(x-4)|+C$.)

**15.** $\displaystyle\int \frac{2x+6}{(x+1)(x-1)^2}\,dx$

This numerator does **not** match the derivative of the denominator, so genuine partial fractions are needed.

Decompose: $\dfrac{A}{x+1}+\dfrac{B}{x-1}+\dfrac{C}{(x-1)^2}$. Clear: $2x+6 = A(x-1)^2+B(x+1)(x-1)+C(x+1)$.

$x=-1$: $4=4A\Rightarrow A=1$. $x=1$: $8=2C\Rightarrow C=4$.

Plug $x=0$: $6=A(1)+B(-1)+C(1) = A-B+C = 1-B+4=5-B$. So $B=5-6=-1$.

$$\int \frac{2x+6}{(x+1)(x-1)^2}\,dx = \ln|x+1| - \ln|x-1| - \frac{4}{x-1} + C$$

**16.** $\displaystyle\int \frac{x+1}{(x-1)(x-2)(x-3)}\,dx$

Decompose: $\dfrac{A}{x-1}+\dfrac{B}{x-2}+\dfrac{C}{x-3}$. Clear: $x+1=A(x-2)(x-3)+B(x-1)(x-3)+C(x-1)(x-2)$.

$x=1$: $2=2A\Rightarrow A=1$. $x=2$: $3=-B\Rightarrow B=-3$. $x=3$: $4=2C\Rightarrow C=2$.

$$\int \frac{x+1}{(x-1)(x-2)(x-3)}\,dx = \ln|x-1| - 3\ln|x-2| + 2\ln|x-3| + C$$

**17.** $\displaystyle\int \frac{x^3+3x^2+2x-7}{x+2}\,dx$

Long division: $x^3+3x^2+2x-7 \div (x+2)$.

$x^3\div x=x^2$; $x^2(x+2)=x^3+2x^2$; subtract: $(x^3+3x^2)-(x^3+2x^2)=x^2$, bring down $2x$: $x^2+2x$.

$x^2\div x=x$; $x(x+2)=x^2+2x$; subtract: $(x^2+2x)-(x^2+2x)=0$, bring down $-7$: $0-7=-7$.

$$\frac{x^3+3x^2+2x-7}{x+2} = x^2+x - \frac{7}{x+2}$$

$$\int \frac{x^3+3x^2+2x-7}{x+2}\,dx = \frac{x^3}{3}+\frac{x^2}{2}-7\ln|x+2|+C$$

---

### 🌍 Applied

**18.** $\displaystyle\int \frac{dx}{(x-2)(x-5)}$

$1=A(x-5)+B(x-2)$. $x=2$: $A=-\frac13$. $x=5$: $B=\frac13$.

$$= -\frac13\ln|x-2| + \frac13\ln|x-5| + C = \frac13\ln\left|\frac{x-5}{x-2}\right|+C$$

**19.** $\displaystyle\int \frac{dP}{P(100-P)}$

Decompose: $\dfrac{A}{P}+\dfrac{B}{100-P}$. $1=A(100-P)+BP$. $P=0$: $A=\frac{1}{100}$. $P=100$: $B=\frac{1}{100}$.

$$= \frac{1}{100}\ln|P| - \frac{1}{100}\ln|100-P| + C = \frac{1}{100}\ln\left|\frac{P}{100-P}\right|+C$$

(This is exactly the building-block integral needed to solve the logistic growth differential equation, $\frac{dP}{dt}=kP(100-P)$.)

**20.** $\displaystyle\int_0^2 \frac{x+3}{(x+1)(x+2)}\,dx$

Decompose: $\dfrac{A}{x+1}+\dfrac{B}{x+2}$. $x+3=A(x+2)+B(x+1)$. $x=-1$: $A=2$. $x=-2$: $B=-1$.

Antiderivative: $2\ln|x+1|-\ln|x+2|$.

At $x=2$: $2\ln3-\ln4$. At $x=0$: $2\ln1-\ln2 = 0-\ln2 = -\ln2$.

$$(2\ln3-\ln4) - (-\ln2) = 2\ln3-\ln4+\ln2$$

Simplify using $\ln4=2\ln2$: $2\ln3-2\ln2+\ln2 = 2\ln3-\ln2 = \ln9-\ln2 = \ln\left(\frac92\right)$.

**Answer: $\ln\left(\dfrac92\right) \approx 1.504$.**

**21.** $\displaystyle\int_4^5 \frac{dx}{(x-3)(x-6)}$

$1=A(x-6)+B(x-3)$. $x=3$: $A=-\frac13$. $x=6$: $B=\frac13$.

Antiderivative: $-\frac13\ln|x-3| + \frac13\ln|x-6| = \frac13\ln\left|\frac{x-6}{x-3}\right|$.

At $x=5$: $\frac13\ln\left|\frac{-1}{2}\right| = \frac13\ln\left(\frac12\right) = -\frac{\ln2}{3}$.

At $x=4$: $\frac13\ln\left|\frac{-2}{1}\right| = \frac13\ln2$.

$$-\frac{\ln2}{3} - \frac{\ln2}{3} = -\frac{2\ln2}{3}$$

**Answer: $-\dfrac{2\ln2}{3} \approx -0.462$.** (The negative sign makes sense: on $[4,5]$, $x-3>0$ but $x-6<0$, so the integrand is negative throughout this interval.)
