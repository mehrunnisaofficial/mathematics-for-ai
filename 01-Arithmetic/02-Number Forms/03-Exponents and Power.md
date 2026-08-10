# Exponents & Powers
### *Mathematics for AI — Study Notes by Mehrunnisa*

Okay, so this is literally the very first topic in my math notes. I'm starting from zero here — like, actual zero. If you've forgotten everything about exponents, don't worry, so had I. Let's rebuild it together from scratch.

---

## Table of Contents

- [1. What Are Exponents and Powers?](#1-what-are-exponents-and-powers)
- [2. Base and Exponent](#2-base-and-exponent)
- [3. Understanding Powers](#3-understanding-powers)
- [4. Laws of Exponents](#4-laws-of-exponents)
- [5. Product of Powers](#5-product-of-powers)
- [6. Quotient of Powers](#6-quotient-of-powers)
- [7. Power of a Power](#7-power-of-a-power)
- [8. Power of a Product](#8-power-of-a-product)
- [9. Special Powers](#9-special-powers)
- [10. Common Mistakes](#10-common-mistakes)
- [11. Quick Revision](#11-quick-revision)
- [12. Mini Quiz](#12-mini-quiz)
- [13. End Concept Map](#13-end-concept-map)

---

## 1. What Are Exponents and Powers?

First, I need to understand why this even exists.

Imagine I have to write this out:

```
2 × 2 × 2 × 2 × 2 × 2 × 2 × 2 × 2 × 2
```

That's ten 2's multiplied together. Writing that every time is annoying and takes up space. So mathematicians made a shortcut for "multiply this number by itself a bunch of times."

That shortcut is a **power**.

So instead of writing `2 × 2 × 2 × 2 × 2 × 2 × 2 × 2 × 2 × 2`, I can just write:

```
2^10
```

This basically means "multiply 2 by itself 10 times." That's it. That's the whole idea. A power is just a compressed way of writing repeated multiplication.

> **The important thing here is:** a power is not a new operation like addition or multiplication. It's just a *notation* — a shorter way of writing something we already know how to do (multiplying).

---

## 2. Base and Exponent

Now let's look at the pieces of a power. Take `2^4`.

```mermaid
flowchart TD
    E["exponent = 4"] --> P["2⁴"]
    B["base = 2"] --> P
    P --> V["means: multiply 2 by itself 4 times"]
```

- **Base** → the number being multiplied (here, 2)
- **Exponent** → how many times the base is multiplied by itself (here, 4)

So `2^4` is read as **"2 raised to the power 4"** or just **"2 to the 4th."**

Let's actually work it out:

```
2^4 = 2 × 2 × 2 × 2 = 16
```

Base = 2
Exponent = 4
Value = 16

The easiest way to think about this is: the exponent tells the base "copy yourself this many times, then multiply all the copies together."

### A few more examples to get comfortable

```
5^3 = 5 × 5 × 5 = 125
3^2 = 3 × 3 = 9
10^5 = 10 × 10 × 10 × 10 × 10 = 100000
```

### Powers of 1

Here's a nice pattern. What is `1^100`?

```
1^100 = 1 × 1 × 1 × ... × 1 (100 times) = 1
```

No matter how many times I multiply 1 by itself, I still get 1. So **1 raised to any power is always 1**. Makes sense — multiplying by 1 never changes anything.

### Powers of 0 (with a positive exponent)

```
0^5 = 0 × 0 × 0 × 0 × 0 = 0
```

Same logic — if the base is 0, the answer is always 0 (as long as the exponent is a positive number).

### What about an exponent of 0?

This one feels weird at first: **any non-zero number raised to the power 0 equals 1.**

```
5^0 = 1
100^0 = 1
```

I won't fully prove this now (we'll actually see *why* this is true naturally once we hit the Quotient Law in Section 6 — it falls right out of the pattern). For now, just remember it as a rule: **anything^0 = 1** (except 0 itself, which is a special case usually left undefined at this level).

### A tiny peek at negative exponents

I'm only mentioning this because it'll help the laws make sense later. A negative exponent just means "flip it into a fraction":

```
2^-1 = 1/2
2^-3 = 1/2^3 = 1/8
```

This basically means a negative exponent doesn't make the number negative — it makes it a **reciprocal**. We won't go deep into this here; just recognize it when it shows up.

---

## 3. Understanding Powers Visually

Let's really lock this in with pictures, because seeing it helps more than just reading it.

```mermaid
flowchart TD
    A["2³"] --> B["base = 2"]
    A --> C["exponent = 3"]
    C --> D["multiply 2 by itself 3 times"]
    D --> E["2 × 2 × 2"]
    E --> F["= 8"]
```

Another way to see it — like "unpacking" the power:

```mermaid
flowchart LR
    A["2⁴"] --> B["2 × 2 × 2 × 2"] --> C["16"]
```

Now I can see why powers are so useful — `2^4` is just a compact box, and expanding it gives me back the full multiplication.

### One more visual: comparing bases and exponents

| BASE changes, exponent stays 3 | | EXPONENT changes, base stays 2 |
|---|---|---|
| 2³ = 8 | | 2¹ = 2 |
| 3³ = 27 | | 2² = 4 |
| 4³ = 64 | | 2³ = 8 |
| | | 2⁴ = 16 |

*Bigger base → bigger jump. Bigger exponent → each step **doubles** the last one.*

This helps me notice something important: increasing the **exponent** grows the number *way* faster than increasing the **base**. That's the whole idea behind "exponential growth."

---

## 4. Laws of Exponents

Okay, now for the actual reason we're here. There are 4 basic laws that let us simplify powers without expanding everything out every single time. I'm not going to just hand you the formulas — I want to *build* each one from scratch so it actually makes sense.

```mermaid
flowchart TD
    L["Laws of Exponents"] --> P["Product of Powers<br/>aᵐ × aⁿ = a⁽ᵐ⁺ⁿ⁾"]
    L --> Q["Quotient of Powers<br/>aᵐ ÷ aⁿ = a⁽ᵐ⁻ⁿ⁾"]
    L --> R["Power of a Power<br/>(aᵐ)ⁿ = a⁽ᵐⁿ⁾"]
    L --> S["Power of a Product<br/>(ab)ⁿ = aⁿ × bⁿ"]
```

---

## 5. Product of Powers

**a^m × a^n = a^(m+n)**

Let's not memorize this yet — let's *see* it happen.

```
2^3 × 2^2
```

I'll expand both powers fully:

```
2^3 × 2^2
= (2 × 2 × 2) × (2 × 2)
```

Now if I remove the brackets, I just have one long multiplication:

```
= 2 × 2 × 2 × 2 × 2
```

Now count how many 2's there are — one, two, three, four, five:

```
= 2^5
```

So:

```
2^3 × 2^2 = 2^(3+2) = 2^5 = 32
```

**Now I can see why** the exponents get added — because multiplying powers of the same base is just *piling up* more copies of that base. 3 copies plus 2 more copies = 5 copies total.

### The shortcut

```
2^3 × 2^2 = 2^(3+2) = 2^5
```

No need to expand every time — just add the exponents, as long as the **base is the same**.

### More examples

```
5^2 × 5^4 = 5^(2+4) = 5^6
x^3 × x^5 = x^(3+5) = x^8
a^1 × a^4 = a^(1+4) = a^5
```

> **A common mistake I can make here** is multiplying the bases together too, like writing `2^3 × 2^2 = 4^5`. That's wrong! The base stays exactly the same — only the exponents add.

---

## 6. Quotient of Powers

**a^m / a^n = a^(m-n)**  (where a ≠ 0)

Same idea, but for division. Let's build it from scratch again.

```
2^5 / 2^2
```

Expand fully:

```
2^5 / 2^2 = (2 × 2 × 2 × 2 × 2) / (2 × 2)
```

Now here's the key step — common factors on top and bottom **cancel out**:

```mermaid
flowchart LR
    A["2 × 2 × 2 × 2 × 2  (top)"] --> C["2 pairs cancel with the bottom"]
    B["2 × 2  (bottom)"] --> C
    C --> D["2 × 2 × 2 left over = 2³"]
```

So:

```
2^5 / 2^2 = 2^(5-2) = 2^3 = 8
```

This basically means: when I divide powers with the same base, the bottom copies cancel out the top copies, leaving only the "extra" ones on top. That's why we **subtract** the exponents instead of adding them.

### The shortcut

```
2^5 / 2^2 = 2^(5-2) = 2^3
```

### More examples

```
7^6 / 7^4 = 7^(6-4) = 7^2
x^9 / x^3 = x^(9-3) = x^6
```

### Quick restriction to remember

The denominator (bottom base) **cannot be zero**, since we can't divide by 0. So this law only works when `a ≠ 0`.

### Why does anything^0 = 1? (the mystery from Section 2, solved)

Watch what happens when the top and bottom exponents are equal:

```
2^3 / 2^3 = 2^(3-3) = 2^0
```

But I also know that any number divided by itself is 1:

```
2^3 / 2^3 = 8/8 = 1
```

So `2^0` must equal `1`. Now I can see exactly why the "anything to the power 0 is 1" rule is true — it's not random, it just falls naturally out of the subtraction rule.

---

## 7. Power of a Power

**(a^m)^n = a^(mn)**

This one is about what happens when a power itself gets raised to another power — like a power wrapped inside another power.

```
(2^3)^2
```

The outer exponent (2) tells me to multiply `2^3` by itself 2 times:

```
(2^3)^2 = 2^3 × 2^3
```

And now I already know this part — it's the Product Law from Section 5! I just add the exponents:

```
= 2^(3+3) = 2^6
```

So:

```
(2^3)^2 = 2^(3×2) = 2^6 = 64
```

**Now I can see why** the exponents get *multiplied* here — because "squaring `2^3`" literally means adding `3 + 3`, which is the same as `3 × 2`. If it were `(2^3)^4`, I'd be adding four 3's together, which is `3 × 4`.

```mermaid
flowchart TD
    A["(2³)²"] --> B["2³ × 2³"]
    B --> C["2⁽³⁺³⁾ = 2⁶"]
    C --> D["same as 2⁽³ˣ²⁾"]
```

### More examples

```
(5^2)^3 = 5^(2×3) = 5^6
(x^4)^2 = x^(4×2) = x^8
```

> **A common mistake I can make here** is confusing this with the Product Law and adding instead of multiplying. Remember: powers *multiplying* each other (like `a^m × a^n`) → **add** exponents. A power *raised to* another power (like `(a^m)^n`) → **multiply** exponents.

---

## 8. Power of a Product

**(ab)^n = a^n × b^n**

Last law! This is about what happens when there are two numbers multiplied *inside* the brackets, and the whole thing is raised to a power.

```
(2 × 3)^2
```

Let's just calculate it directly first — the normal way:

```
(2 × 3)^2 = 6^2 = 36
```

Now let's try applying the exponent to *each* factor separately and see if we get the same answer:

```
2^2 × 3^2 = 4 × 9 = 36
```

Same answer! So:

```
(2 × 3)^2 = 2^2 × 3^2 = 36
```

This basically means when a **product** (two things multiplied) is inside the brackets, the exponent outside applies to *both* factors individually — not just one of them.

```mermaid
flowchart TD
    A["(2 × 3)²"] --> B["2²"]
    A --> C["3²"]
    B --> D["4"]
    C --> E["9"]
    D --> F["4 × 9 = 36"]
    E --> F
```

### More examples

```
(3 × 5)^2 = 3^2 × 5^2 = 9 × 25 = 225
(x × y)^3 = x^3 × y^3
```

> **A common mistake I can make here** is forgetting to apply the exponent to *both* factors — like writing `(2×3)^2 = 2^2 × 3` instead of `2^2 × 3^2`. Every factor inside the brackets gets the exponent.

---

## 9. Special Powers

We already touched two of these back in Section 2, but now that I know the laws, I can actually understand *why* they work instead of just accepting them. Let's go through all three "special" types of exponents one by one.

```mermaid
flowchart TD
    S["Special Powers"] --> Z["Zero Exponent<br/>a⁰"]
    S --> N["Negative Exponent<br/>a⁻ⁿ"]
    S --> F["Fractional Exponent<br/>a^(1/n)"]
```

### 9.1 Zero Exponent

**Rule: a⁰ = 1** (for a ≠ 0)

I already proved this back in Section 6 using the Quotient Law, but here's the quick recap of *why* it makes sense:

```
2^3 / 2^3 = 2^(3-3) = 2^0
```

But anything divided by itself is 1:

```
2^3 / 2^3 = 8/8 = 1
```

So `2^0 = 1`. The important thing here is: this isn't a special exception someone made up — it just naturally falls out of the subtraction rule.

```
5^0 = 1
100^0 = 1
```

### 9.2 Negative Exponent

**Rule: a⁻ⁿ = 1 / aⁿ**

The easiest way to think about this is: a negative sign in the exponent doesn't make the *number* negative — it flips the power into a fraction (its reciprocal).

Let's actually see why, using the Quotient Law again. What happens if the top exponent is *smaller* than the bottom one?

```
2^2 / 2^5 = 2^(2-5) = 2^-3
```

Now let's expand it the long way and simplify by cancelling:

```
2^2 / 2^5 = (2 × 2) / (2 × 2 × 2 × 2 × 2)
```

Cancel the two matching pairs on top and bottom:

```mermaid
flowchart LR
    A["2 × 2  (top)"] --> C["both 2's cancel with the bottom"]
    B["2 × 2 × 2 × 2 × 2  (bottom)"] --> C
    C --> D["1 / (2 × 2 × 2) = 1/2³"]
```

So:

```
2^2 / 2^5 = 2^-3 = 1/2^3 = 1/8
```

**Now I can see why** a negative exponent means "flip it" — it's just what happens naturally when the bottom of the fraction has *more* copies of the base than the top.

#### Example: `2^-3`

```
2^-3 = 1/2^3 = 1/8
```

> **A common mistake I can make here** is thinking `2^-3 = -8`. It does NOT make the answer negative — it makes it a fraction: `1/8`.

### 9.3 Fractional Exponent

**Rule: a^(1/n) = ⁿ√a**  (the n-th root of a)

This one looks strange at first, but the Power of a Power law (Section 7) actually explains it perfectly. Watch this:

If `a^(1/2)` squared should just give me back `a` (because squaring undoes a "half power"):

```
(a^(1/2))^2 = a^((1/2)×2) = a^1 = a
```

But I also know that **squaring a square root gives back the original number**:

```
(√a)^2 = a
```

Since both `a^(1/2)` and `√a` do the exact same thing when squared, they must be the same thing:

```
a^(1/2) = √a
```

This basically means: a fractional exponent like `1/2` isn't multiplication or division at all — it's asking "what number, multiplied by itself the right number of times, gives me this?" In other words, it's a **root** in disguise.

```mermaid
flowchart TD
    A["a^(1/n)"] --> B["means: the n-th root of a"]
    B --> C["ⁿ√a"]
```

The denominator of the fraction tells me *which* root to take:

- `a^(1/2)` → square root of a
- `a^(1/3)` → cube root of a
- `a^(1/n)` → n-th root of a

#### Example: `16^(1/2)`

I need a number that, multiplied by itself once (squared), gives 16.

```
16^(1/2) = √16 = 4      (because 4 × 4 = 16)
```

#### Example: `27^(1/3)`

I need a number that, multiplied by itself twice more (cubed), gives 27.

```
27^(1/3) = ³√27 = 3      (because 3 × 3 × 3 = 27)
```

### Quick summary table

| Exponent Type | Rule | Example |
|---|---|---|
| Zero | a⁰ = 1 | 5⁰ = 1 |
| Negative | a⁻ⁿ = 1/aⁿ | 2⁻³ = 1/8 |
| Fractional (1/2) | a^(1/2) = √a | 16^(1/2) = 4 |
| Fractional (1/3) | a^(1/3) = ³√a | 27^(1/3) = 3 |

> **A common mistake I can make here** is treating a fractional exponent like normal division — `16^(1/2)` does NOT mean `16 ÷ 2 = 8`. It means "take the square root of 16," which is `4`.

---

## 10. Common Mistakes

Quick round-up of the slip-ups I need to watch out for:

- ❌ `2^3 × 2^2 = 4^5` → ✅ base stays the same, only add exponents: `2^5`
- ❌ `(2^3)^2 = 2^5` (adding instead of multiplying) → ✅ `2^6`
- ❌ `(2×3)^2 = 2^2 × 3` → ✅ apply exponent to **both** factors: `2^2 × 3^2`
- ❌ Adding exponents when the **bases are different** (e.g., `2^3 × 3^2` cannot be simplified this way — the laws only work for the *same base*)
- ❌ Thinking `a^0 = 0` → ✅ it's actually `1` (for a ≠ 0)
- ❌ Thinking `2^-3 = -8` → ✅ it's `1/8` — a negative exponent flips to a fraction, it doesn't make the value negative
- ❌ Thinking `16^(1/2) = 8` (treating it as division) → ✅ it's `√16 = 4` — a fractional exponent means a root

---

## 11. Quick Revision

| Law | Rule |
|---|---|
| Product of Powers | aᵐ × aⁿ = a⁽ᵐ⁺ⁿ⁾ |
| Quotient of Powers | aᵐ ÷ aⁿ = a⁽ᵐ⁻ⁿ⁾ |
| Power of a Power | (aᵐ)ⁿ = a⁽ᵐⁿ⁾ |
| Power of a Product | (ab)ⁿ = aⁿ × bⁿ |

| Special Case | Value |
|---|---|
| a⁰ | 1 &nbsp;(a ≠ 0) |
| a¹ | a |
| 1ⁿ | 1 |
| 0ⁿ &nbsp;(n > 0) | 0 |
| a⁻ⁿ | 1/aⁿ |
| a^(1/2) | √a |
| a^(1/3) | ³√a |

**Memory trick:**
- Multiplying same-base powers → **ADD**
- Dividing same-base powers → **SUBTRACT**
- Power on a power → **MULTIPLY**
- Product inside brackets → **DISTRIBUTE** the exponent to each factor
- Negative exponent → **FLIP** it into a fraction
- Fractional exponent → **ROOT** (denominator tells you which root)

---

## 12. Mini Quiz

Try these before checking the answers below — no peeking!

1. `3^2 × 3^4 = ?`
2. `5^7 / 5^3 = ?`
3. `(2^2)^3 = ?`
4. `(4 × 2)^2 = ?` (solve two ways and check they match)
5. `9^0 = ?`
6. `1^250 = ?`
7. What's wrong with this step: `2^3 × 2^2 = 4^5`?
8. `2^-3 = ?`
9. `16^(1/2) = ?`
10. `27^(1/3) = ?`

<details>
<summary>Click to check answers</summary>

1. `3^(2+4) = 3^6 = 729`
2. `5^(7-3) = 5^4 = 625`
3. `2^(2×3) = 2^6 = 64`
4. `(4×2)^2 = 8^2 = 64` and `4^2 × 2^2 = 16 × 4 = 64` ✅ matches
5. `9^0 = 1`
6. `1^250 = 1`
7. The base should stay as `2`, not become `4`. Correct answer: `2^5 = 32`
8. `2^-3 = 1/2^3 = 1/8`
9. `16^(1/2) = √16 = 4`
10. `27^(1/3) = ³√27 = 3`

</details>

---

## 13. End Concept Map

```mermaid
flowchart TD
    Root["Powers & Exponents"] --> Basics["Base & Exponent<br/>aⁿ = a × a × ... × a"]
    Root --> Laws["Laws of Exponents"]
    Root --> SP["Special Powers"]

    Laws --> P["Product<br/>aᵐ×aⁿ = a⁽ᵐ⁺ⁿ⁾"]
    Laws --> Qt["Quotient<br/>aᵐ÷aⁿ = a⁽ᵐ⁻ⁿ⁾"]
    Laws --> Pw["Power of Power<br/>(aᵐ)ⁿ = a⁽ᵐⁿ⁾"]
    Laws --> Pd["Power of Product<br/>(ab)ⁿ = aⁿ×bⁿ"]

    SP --> Z["Zero: a⁰ = 1"]
    SP --> N["Negative: a⁻ⁿ = 1/aⁿ"]
    SP --> F["Fractional: a^(1/n) = ⁿ√a"]
```

That's the full picture — start with what a power even *is*, then build every law from first principles instead of memorizing it blind. Next up: putting these laws into more mixed practice problems.

---

<div align="center">

⋆˚꩜｡

### Follow Me

If you enjoyed these notes, you'll probably enjoy the rest too.

| Platform | Link |
|---|---|
| Instagram | @mehrunnisa.ai |
| SubStack | The Epoch |
| YouTube | @mehrunnisa.ai |


**Usage Terms**
These notes are free to use for personal learning, revision, and study. Please do not:
- Sell or redistribute for profit.
- Claim them as your own work.
- Modify and republish without permission.
- Use for any unethical or unauthorized purpose.

Thank you for respecting the effort behind these notes. Happy learning. ♡

</div>
