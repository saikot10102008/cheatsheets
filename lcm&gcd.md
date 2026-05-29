When you are dealing with purely algebraic terms (variables) instead of numbers, the logic for finding the **GCD** and **LCM** actually becomes more consistent because you are simply "counting" the variables.

Think of each variable ($a, b, c, d$) as a **prime number**.

---

## 1. Finding the GCD (Greatest Common Divisor)

The GCD is the "Shared Minimum." It represents the factors that **every single term** has in common.

* **The Rule:** Look at each variable one by one. Take the **lowest** power of that variable found in any of the terms.
* **The Catch:** If even *one* term is missing a variable, the "lowest power" of that variable is $0$ (which equals $1$). Therefore, that variable cannot be part of the GCD.

### Example: $a^2b, b^2a, d$

* **Variable $a$:** Power is $2$ in the first term, $1$ in the second, but **$0$** in the third. $\rightarrow$ Result: $a^0 = 1$.
* **Variable $b$:** Power is $1$ in the first, $2$ in the second, but **$0$** in the third. $\rightarrow$ Result: $b^0 = 1$.
* **Variable $d$:** Power is $0$ in the first two, $1$ in the last. $\rightarrow$ Result: $d^0 = 1$.
* **Final GCD:** $1 \cdot 1 \cdot 1 = \mathbf{1}$.

---

## 2. Finding the LCM (Least Common Multiple)

The LCM is the "All-Inclusive Maximum." It must be a "container" large enough to hold any of the individual terms.

* **The Rule:** Look at each variable one by one. Take the **highest** power of that variable found in **any** of the terms.
* **The Logic:** Even if a variable only appears once in the entire list, it *must* be included in the LCM to account for that specific term.

### Example: $a^2b, b^2a, d$

* **Variable $a$:** Highest power found is $a^2$.
* **Variable $b$:** Highest power found is $b^2$.
* **Variable $d$:** Highest power found is $d^1$.
* **Final LCM:** $a^2 \cdot b^2 \cdot d^1 = \mathbf{a^2b^2d}$.

---

## Quick Reference Summary

| Case | Terms | GCD (Lowest Powers) | LCM (Highest Powers) |
| --- | --- | --- | --- |
| **Simple Mix** | $a, b, cd$ | **$1$** (Nothing shared) | **$abcd$** (Need all three) |
| **Overlap** | $ab, c, d$ | **$1$** (Nothing shared) | **$abcd$** |
| **Shared Factors** | $ab, ac, ad$ | **$a$** (Every term has an $a$) | **$abcd$** |
| **Power Play** | $a^2b, b^2a, d$ | **$1$** | **$a^2b^2d$** |

### The "Mental Checklist"

1. **For GCD:** Ask, "Is this letter in *every* single pile?" If yes, what is the smallest amount of it in any one pile?
2. **For LCM:** Ask, "What is the most I see of this letter in *any* pile?" Collect those maximums and multiply them.

Does this make it easier to visualize why the GCD often ends up being $1$ when you start adding unrelated variables like $d$?
