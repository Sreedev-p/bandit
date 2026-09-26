Let’s get you fully prepared to ace CAT 2! Looking over your syllabus image, Module 3 shifts into **Context-Free Grammars (CFGs), Parsing, Normal Forms, and Pushdown Automata (PDAs)**. This part of the course has very high-scoring, procedural numericals (like grammar conversions and stack traces) where you can easily secure 100% if your steps are clean.

Here is a structured, high-yield study plan broken down into 4 logical phases to help you master everything efficiently.

---

### Phase 1: CFG Foundations & Grammar Derivations

Target Topics: CFG Construction, CFL, LMD, RMD, Parse Trees, and Ambiguity.

* **What to master:**
* **CFG Construction:** Practice building grammars for standard patterns (e.g., $a^n b^n$, balanced parentheses, palindromes, expressions with operators).
* **Derivations:** Learn how to write **Leftmost Derivations (LMD)** (always expanding the leftmost non-terminal) and **Rightmost Derivations (RMD)** (expanding the rightmost).
* **Parse Trees:** Practice drawing the tree structure corresponding to LMD and RMD.
* **Ambiguity:** Understand how a grammar is ambiguous if a string has *two or more distinct parse trees* (or multiple LMDs/RMDs). Learn how to prove ambiguity or rewrite the grammar to remove it.



---

### Phase 2: Grammar Simplification & Normal Forms

Target Topics: Simplification (NULL, UNIT, Useless), Normal Forms (CNF, GNF), CFG to CNF, CFG to GNF.

* **What to master:**
* **Simplification (The Clean-up Phase):** Learn the strict chronological order for cleaning a grammar:
1. Remove $\epsilon$-productions ($\nu$-productions / NULL).
2. Remove Unit productions ($A \to B$).
3. Remove Useless symbols (symbols that cannot reach terminals or cannot be reached from the start symbol).


* **Chomsky Normal Form (CNF):** Every production must be in the form $A \to BC$ or $A \to a$. Practice the step-by-step conversion algorithm (handling mixed terminals, long RHS chains, and $\epsilon$/unit rules first).
* **Greibach Normal Form (GNF):** Every production must start with a single terminal followed by zero or more variables ($A \to a \alpha$). This one requires careful substitution and handling of left recursion.



---

### Phase 3: Compiler Front-End Essentials

Target Topics: First & Follow, Left Recursion, and Left Factoring.

* **What to master:**
* **Left Recursion Elimination:** Learn how to rewrite immediate and indirect left-recursive rules ($A \to A\alpha \mid \beta$) into right-recursive forms to prevent infinite loops in top-down parsers.
* **Left Factoring:** Learn how to factor out common prefixes ($A \to \alpha\beta_1 \mid \alpha\beta_2$) so a parser knows which production to choose without lookahead conflicts.
* **FIRST and FOLLOW Sets:** Master the exact rules for computing FIRST (the set of terminal symbols that begin strings derived from a variable) and FOLLOW (the set of terminals that can appear immediately to the right of a variable). *This is a guaranteed long-answer question in exams!*



---

### Phase 4: Advanced Theory & Machines

Target Topics: CFL Pumping Lemma, DPDA & NPDA.

* **What to master:**
* **Pumping Lemma for CFLs:** Understand the Ogden's/CFL Pumping Lemma structure ($s = uvwxy$, $\vert{}vx\vert{} > 0$, $\vert{}vwx\vert{} \le p$, $uv^i wx^i y \in L$) and how to use proof-by-contradiction to show a language is not context-free (e.g., $a^n b^n c^n$).
* **Pushdown Automata (PDA):**
* Understand how a PDA extends an NFA with a **Stack** (Last-In, First-Out memory).
* Learn how to design **Non-Deterministic PDAs (NPDA)** using empty stack acceptance ($\mathcal{N}(\mathcal{A})$) or final state acceptance ($\mathcal{F}(\mathcal{A})$).
* Learn the conversion nuances for **Deterministic PDAs (DPDA)** where no conflicts exist between transitions or $\epsilon$-moves.





---

### Your Daily Execution Strategy

1. **Day 1 (Phases 1 & 2):** Spend a few hours practicing CFG construction, writing LMD/RMDs, and drilling the strict step-by-step algorithm for **Simplification $\to$ CNF conversion**.
2. **Day 2 (Phase 3):** Focus purely on compiler parsing techniques: **Left Recursion, Left Factoring, and computing FIRST & FOLLOW sets**. Do at least 4-5 full numerical problems.
3. **Day 3 (Phase 4):** Tackle **CFG Pumping Lemma proofs** and practice designing **transition functions and ID (Instantaneous Description) traces for NPDAs and DPDAs**.

Which of these topics would you like to start practicing or reviewing first?
