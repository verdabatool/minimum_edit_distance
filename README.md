# Minimum Edit Distance: The Detective's Toolkit 🕵️‍♂️

This notebook is a hands-on journey into the **Minimum Edit Distance (MED)** algorithm, framed as a series of detective cases. I've started by implementing the foundational algorithm and progressively apply it to solve more complex, real-world NLP mysteries like spell correction and language identification.

Each part of the notebook builds on the last, turning a classic algorithm into a powerful tool for text analysis.

---

## 📜 Case Files: What's Inside

### Part 1: Setting up the Foundation

The first step for any detective is to master the basics. This section covers the implementation of the classic **Minimum Edit Distance** algorithm using dynamic programming.

**In this part, we will:**
* Implement a `min_edit_distance` function from scratch.
* Visualize the dynamic programming matrix for sample words (`kitten` → `sitting`) to understand how the algorithm works.

---

### Part 2: The Weighted Typo Mystery

Not all mistakes are created equal. A good detective knows that some clues are more significant than others. Here, we extend the basic MED to account for the fact that certain typos (like adjacent keys on a keyboard) are more common.

**In this part, we will:**
* Modify the MED function to support a **custom cost matrix**.
* Implement weighted costs based on keyboard character adjacency (`q` ↔ `w` is cheaper than `q` ↔ `b`).
* Compare the results of standard vs. weighted MED to see the impact of nuanced costs.

---

### Part 3: The Spell-Crime Case

A manuscript full of errors has landed on your desk. Your mission is to identify the intended words. This part applies the MED algorithm to build a practical spell checker.

**In this part, we will:**
* Build a function to suggest the **top N candidate corrections** for a given word from a dictionary.
* Generate and compare correction suggestions using both the standard and weighted MED functions.
* Analyze how different cost functions change the final suggestions.

---

### Part 4: The Language Identification Mystery

The final case involves a single, typo-ridden word from a spy's message. The word itself is a clue to the spy's native language. This section uses MED in a creative way to perform language identification.

**In this part, we will:**
* Use MED to calculate the "distance" of a misspelled word to entire language corpuses.
* Determine the most likely language of origin by finding the one with the lowest average edit distance.
