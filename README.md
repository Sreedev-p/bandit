# DBMS Exam Study Plan: Modules 2 & 3

## Block 1: Dependency Math & Advanced Normalization
**Topics Covered:** 
* Functional dependencies: inference rules, equivalence, and minimal cover[cite: 8].
* Axioms on functional dependencies[cite: 8].
* Normalization: 1NF, 2NF, 3NF, BCNF, multi-valued dependency (4NF), and join dependency (5NF)[cite: 8].

**Execution Strategy:**
* Skim 1NF through BCNF using your recent practical schema design experience.
* Focus on **Armstrong's Axioms** (reflexivity, augmentation, transitivity).
* Practice calculating the **minimal cover** of a functional dependency set.
* Master identifying multi-valued and join dependencies for 4NF and 5NF.

## Block 2: Physical Storage & Indexing
**Topics Covered:** 
* File structures: operations on files, unordered/ordered records[cite: 8].
* Hashing techniques: static and dynamic[cite: 8].
* Indexing: single/multi-level, dynamic multilevel, B+ trees, LSM trees and variants[cite: 8].

**Execution Strategy:**
* Map the time complexities of searching ordered vs. unordered records.
* Diagram the mechanics of **B+ tree node splitting and merging**.
* Compare write-heavy operation handling in **LSM trees** versus traditional B+ trees.

## Block 3: Relational Algebra & Calculus
**Topics Covered:** 
* Relational Algebra: operators, translating SQL queries into relational algebra[cite: 8].
* Tuple Relational Calculus[cite: 8].

**Execution Strategy:**
* Translate SQL syntax into mathematical notation (Select $\sigma$, Project $\pi$, Join $\bowtie$).
* Write **Tuple Relational Calculus (TRC)** expressions focusing on "FOR ALL" ($\forall$) and "EXISTS" ($\exists$) conditions.

## Block 4: Query Optimization
**Topics Covered:** 
* Query Optimization: query trees and heuristic optimization of query trees[cite: 8].

**Execution Strategy:**
* Trace how the database engine executes the relational algebra from Block 3.
* Apply **heuristic rules**: practice pushing "Select" (filtering) and "Project" operations down the query tree to mathematically reduce join computation costs.
