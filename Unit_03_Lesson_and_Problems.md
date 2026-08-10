# Unit 3: The Precise Definition of a Limit

## 1. The idea, in plain words

Back in Unit 2, we said a limit is "the number $f(x)$ gets closer and closer to as $x$ gets closer and closer to $a$." That's a great starting picture, but "closer and closer" is a little fuzzy — closer by how much? This unit just makes that fuzzy idea *precise*, using a simple game: the **tolerance game**.

**Picture it like archery, or a factory quality check.** Suppose someone hands you a target number $L$ and says: "I want $f(x)$ to land within a tiny margin of $L$ — say, within $\varepsilon$ (the Greek letter *epsilon*) — no matter how small a margin I ask for." Your job is to find a matching rule for $x$: "As long as $x$ stays within some margin $\delta$ (the Greek letter *delta*) of $a$, I guarantee $f(x)$ will land inside your target band."

- $\varepsilon$ (epsilon) = **how close you want the output**, $f(x)$, to be to $L$. This lives on the **y-axis** (the output side).
- $\delta$ (delta) = **how close the input**, $x$, needs to be to $a$ to guarantee that. This lives on the **x-axis** (the input side).

**The picture:** draw two horizontal dashed lines at $L-\varepsilon$ and $L+\varepsilon$ — that's the "target band" for the output. Then find two vertical dashed lines at $a-\delta$ and $a+\delta$ — the "safe zone" for the input — such that any $x$ inside that safe zone (other than $x=a$ itself) produces an $f(x)$ that lands inside the target band.

**Saying "the limit is $L$" really just means:** no matter how thin someone makes that target band ($\varepsilon$), you can *always* find a safe zone ($\delta$) around $a$ that keeps you inside it. That's all the "precise definition" is doing — turning "gets closer and closer" into an actual tolerance-matching game you can play with real numbers.

**Good news for this unit:** we'll only play this game with straight-line functions ($f(x) = mx+b$), because for a line, there's a clean, simple shortcut for finding a matching $\delta$ — no formal proof-writing needed, just some algebra.

## 2. Toolbox

**What each symbol means:**

- $a$ = the input value we're approaching
- $L$ = the limit (the target output value), often $L = f(a)$ for our examples
- $\varepsilon$ = the allowed margin of error on the *output* (how close $f(x)$ must be to $L$)
- $\delta$ = the allowed margin of error on the *input* (how close $x$ must be to $a$)

**The tolerance-matching statement:** we want to guarantee

$$|f(x) - L| < \varepsilon \quad \text{whenever} \quad 0 < |x-a| < \delta$$

**The straight-line shortcut:** if $f(x) = mx+b$ and $L = f(a)$, then

$$|f(x)-L| = |m(x-a)| = |m|\cdot|x-a|$$

So $|f(x)-L| < \varepsilon$ exactly when $|x-a| < \dfrac{\varepsilon}{|m|}$. That means:

$$\delta = \frac{\varepsilon}{|m|}$$

always works. (Any *smaller* delta than this also works — it's not the one "correct" answer, just a safe one.)

**Working backward:** if you're told a $\delta$ was used, the guaranteed output tolerance is

$$\varepsilon = |m|\cdot \delta$$

## 3. Common mistakes

- **Mixing up which axis epsilon and delta belong to.** Epsilon is always about the output ($y$), delta is always about the input ($x$).
- **Thinking there's only one "correct" delta.** Any delta smaller than or equal to $\varepsilon/|m|$ works. If a smaller window on $x$ works, a slightly larger one that's still $\le \varepsilon/|m|$ works too — there isn't a single magic number.
- **Forgetting to use the absolute value / size of the slope.** A steep negative slope (like $m=-5$) still needs $|m|=5$ in the formula — the sign of the slope doesn't matter here, only its size.
- **Assuming a bigger epsilon needs a bigger delta — that part's true — but forgetting that a *steeper* line needs a *smaller* delta for the same epsilon.** A steep line amplifies small changes in $x$ into big changes in $y$, so you need to control $x$ more tightly.
- **Forgetting to double-check by plugging the boundary values back in.** Plugging in $x=a+\delta$ and $x=a-\delta$ is a great way to confirm your delta actually lands $f(x)$ right at (or inside) the tolerance band.

## 4. Problem Set

### 🟢 Warm-up

1. For $f(x)=2x$ at $a=3$ (so $L=6$): if we want $f(x)$ to stay within $\varepsilon=0.4$ of $6$, how close must $x$ be to $3$? Find a valid $\delta$.
2. For $f(x)=5x$ at $a=2$ (so $L=10$), with $\varepsilon=1$: find a valid $\delta$.
3. For $f(x)=-3x$ at $a=1$ (so $L=-3$), with $\varepsilon=0.6$: find a valid $\delta$.
4. For $f(x)=x+4$ at $a=5$ (so $L=9$), with $\varepsilon=0.3$: find a valid $\delta$.
5. In plain words: if two lines have the same $\varepsilon$ requirement, but one line is steeper (larger $|m|$) than the other, which one needs the *smaller* $\delta$? Explain why, using the "amplifying" idea from the Common Mistakes section.
6. In plain words: if someone tightens their tolerance request (makes $\varepsilon$ smaller), does the matching $\delta$ need to get smaller too, stay the same, or get bigger? Explain.

### 🟡 Standard

7. For $f(x)=4x-1$ at $a=2$ (so $L=7$), with $\varepsilon=0.8$: find a valid $\delta$.
8. For $f(x)=-2x+5$ at $a=3$ (so $L=-1$), with $\varepsilon=0.5$: find a valid $\delta$.
9. For $f(x)=6x+2$ at $a=-1$ (so $L=-4$), with $\varepsilon=1.2$: find a valid $\delta$.
10. For $f(x)=3x$ at $a=0$, with $\varepsilon=0.09$: find a valid $\delta$.
11. For $f(x)=2x+1$ at $a=4$: if you use $\delta=0.15$, what is the resulting $\varepsilon$ this guarantees? Describe the output tolerance band in words (i.e., "$f(x)$ stays between ___ and ___").
12. For $f(x)=-4x+3$ at $a=1$: if you use $\delta=0.1$, what is the resulting $\varepsilon$? Describe the output tolerance band in words.

### 🔴 Challenge

13. For $f(x)=7x-3$ at $a=2$, with $\varepsilon=0.35$: find the delta given by the shortcut formula, then check your answer by plugging $x=a+\delta$ and $x=a-\delta$ into $f(x)$ and confirming both land exactly on the edge of the tolerance band around $L$.
14. For $f(x)=3x+1$ at $a=2$ (so $L=7$), with $\varepsilon=0.6$: the shortcut formula gives one delta. But suppose there's also a *separate* physical requirement that $x$ must stay within $0.15$ units of $a=2$ no matter what. What overall $\delta$ should you use, and why?
15. For $f(x)=-5x+2$ at $a=-2$ (so $L=12$), with $\varepsilon=0.25$: find the delta given by the shortcut formula. Then, is $\delta=0.02$ *also* a valid choice? Explain why or why not, using the "smaller delta" idea from the Toolbox.
16. Suppose you're told that for $f(x)=2x$ near $a=3$, the output $f(x)$ must stay strictly between $5.7$ and $6.3$. Figure out what $\varepsilon$ was being used, and then find the matching $\delta$.

### 🌍 Applied

17. A machine cuts metal rods, and the rod length (in meters) depends on a dial setting $x$ according to $f(x) = 2x$. The target length is $6$ meters (at dial setting $a=3$), and a rod is acceptable only if it's within $0.02$ m of $6$ m. How precisely must the dial be set (find $\delta$) to guarantee an acceptable rod?
18. A thermostat's resulting room temperature (in °F) is $T(x) = 3x+65$, where $x$ is a dial setting. The target temperature is $71°F$ at dial setting $a=2$. The room must stay within $0.9°F$ of the target. How precisely must the dial be set?
19. A pharmacist mixes a solution whose concentration (in mg/mL) is $C(x) = 4x+10$, where $x$ is the amount (in mL) of a stock solution added. The target concentration is $26$ mg/mL at $x=4$ mL. Safety rules require the concentration to stay within $0.5$ mg/mL of the target. How precisely must $x$ be measured?
20. A drone's altitude (in meters) is modeled by $h(x) = 10x$, where $x$ is a throttle setting near $a=5$ (giving a target altitude of $L=50$ m). To stay clear of a restricted zone, the altitude must stay within $2$ m of $50$ m. How precisely must the throttle setting be controlled?
