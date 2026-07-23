# Wittgenstein: Professional Language-Games in Insurance Investigation

## What This Is (and What It Isn't)

**What this file is:**
- A philosophical framework for *why* the 12 rules work
- Deep-dive explanation of professional language-games theory
- Background reading for building judgment and internalization

**What this file is NOT:**
- ❌ The foundation of the system (the system works without it)
- ❌ A differentiator (case law is the differentiator)
- ❌ Required for using the validator
- ❌ What your boss cares about
- ❌ A guide to using the validator

**When to read this:** After you understand the 12 rules and want to internalize *why* they exist. Best used for building judgment, not memorizing rules.

**Better starting points:** Read `identity.md` and `rules.md` first. Try the official test case in `sample-reports/`. Then come back here if you want depth.

---

## The Core Principle

**Ludwig Wittgenstein:** "The meaning of a word is its use in the language."

**In Insurance Investigation:** Professional words like "evidence," "fraud," "finding," and "observation" have determinate meanings because they're used within a **professional language-game** with specific rules. When investigators violate those rules, they violate the meaning itself.

---

## What is a Language-Game?

A language-game is a rule-governed activity where:

1. **Words have determinate meanings** (not arbitrary)
2. **Meanings come from how words are used** (in practice, not in isolation)
3. **Rules govern the use** (professional standards define what counts)
4. **Violating rules breaks meaning** (and creates language violations)

**Example:** The word "fraud" in insurance investigation is a language-game with these rules:
- Requires proven INTENT to deceive
- Requires documented MISREPRESENTATION
- Requires MATERIALITY (the lie matters to coverage)
- Cannot be used based on suspicion alone
- Cannot be inferred from mere contradiction

When an investigator writes "The insured committed fraud because he said the loss occurred on Tuesday but also said Wednesday," they've violated the language-game. They used "fraud" (which requires INTENT and MISREPRESENTATION) in a context where only CONTRADICTION is present.

---

## How the 12 Rules Enforce Language-Games

Each validation rule enforces proper use within specific language-games. Here are the key patterns:

### Rule 1: Observation ≠ Interpretation

**Two language-games:**

**OBSERVATION:**
- What you perceived directly
- What is documented
- What is repeatable
- Uses: "I saw," "I heard," "I documented"
- Rules: Must be specific, must have a source, must be verifiable

**INTERPRETATION:**
- What you concluded from observations
- What requires reasoning
- What may be challenged
- Uses: "This suggests," "Could mean," "Indicates"
- Rules: Must be traceable to observations, must acknowledge alternatives

**Violation:** ❌ "The insured appeared nervous, which indicates he was lying."
- "Appeared nervous" = OBSERVATION (valid)
- "Indicates he was lying" = INTERPRETATION (invalid jump)
- Nervousness in the OBSERVATION game does NOT translate to "lying" in the INTERPRETATION game

**Proper use:** ✅ "OBSERVATION: The insured paused 8 seconds before answering and spoke hesitantly. INTERPRETATION: This could indicate (1) nervousness, (2) careful thought, (3) anxiety, or (4) awareness of inconsistency. Evidence distinguishing these: [what would help]."

---

### Rule 2: Evidence ≠ Conclusion

**Two language-games:**

**EVIDENCE:**
- Facts that are documented
- Sources that can be traced
- Information that exists independently
- Rules: Must be verifiable, must be specific, must have source attribution

**CONCLUSION:**
- What the evidence means
- The investigator's determination
- What others might dispute
- Rules: Must be traceable to evidence, must acknowledge gaps, must avoid overreach

**Violation:** ❌ "The insured is committing fraud. Investigation shows he is lying about the loss date."
- Neither statement has EVIDENCE behind it
- The investigator treated conclusions as if they were evidence

**Proper use:** ✅ "EVIDENCE: Statement 1 said loss occurred Tuesday. Statement 2 said Wednesday. Police report confirms Wednesday. CONCLUSION: The Tuesday statement appears inaccurate. Possible explanations: (1) memory error, (2) misunderstanding, (3) intentional misstatement. Additional evidence needed: [what would help]."

---

### Rule 3: Suspicion ≠ Evidence

**Two language-games:**

**SUSPICION:**
- Personal gut feeling
- Preliminary impression
- Justifies further investigation
- Rules: Private to investigator, cannot be cited as proof, triggers work

**EVIDENCE:**
- Documented facts
- Third-party verifiable
- Stands on its own
- Rules: Must be specific, must have source, must be reproducible

**Violation:** ❌ "I suspected the loss was exaggerated. Investigation confirmed my suspicion that this claim is fraudulent."
- The investigator moved from suspicion to conclusion by relabeling it

**Proper use:** ✅ "Initial observation: The claim amount seems high. This raised questions worth investigating. Investigation findings: [what I actually found]. The amount appears [reasonable/inflated] based on [specific evidence]."

---

### Rule 5: Intent ≠ Motive

**Two language-games:**

**MOTIVE:**
- "Why someone might do something"
- "Need, desire, pressure"
- Rules: Can be inferred from circumstances

**INTENT:**
- "Someone deliberately chose to do it"
- "Proved by action"
- Rules: Requires evidence of deliberate choice

**Violation:** ❌ "The insured had financial difficulties, so he staged the loss. This proves fraud."
- Financial difficulties = MOTIVE (why someone might act)
- But millions with financial difficulties don't commit fraud
- Motive doesn't establish intent

**Proper use:** ✅ "MOTIVE: The insured had financial difficulties [documented]. This creates possible motive for fraud. INTENT: To establish intent, we need evidence the insured deliberately staged the loss. Evidence: [what we found]. This is [consistent with/inconsistent with] deliberate staging. Additional evidence needed: [what would help]."

---

### Rule 6: Contradiction ≠ Deception

**Two language-games:**

**CONTRADICTION:**
- Two statements that conflict
- Observable and documentable
- Rules: Just report what was said when

**DECEPTION:**
- Intentional false statement
- Requires knowledge of intent
- Rules: Must establish awareness and deliberate choice

**Violation:** ❌ "The claimant gave two different stories. This proves she was lying."
- Contradiction = observable fact
- Lying = requires proof of intent
- They're different language-games with different rules

**Proper use:** ✅ "CONTRADICTION: Statement 1 [date]: Loss occurred Tuesday. Statement 2 [date]: Loss occurred Wednesday. When asked about inconsistency, claimant stated: [explanation]. Possible causes: (1) memory error, (2) misunderstanding, (3) deliberate misstatement. Evidence distinguishing: [what would help]."

---

### Rule 4: Possibility ≠ Probability ≠ Proof

**Three language-games:**

**POSSIBILITY:**
- "Could occur"
- "Might be"
- Rules: Very low bar, just needs logical coherence

**PROBABILITY:**
- "More likely than not"
- "Evidence points toward"
- Rules: Evidence tips the balance

**PROOF:**
- "Established by evidence"
- "Beyond reasonable doubt"
- Rules: High bar, evidence is decisive

**Violation:** ❌ "It's possible the insured staged the loss. Therefore, the loss is fraudulent."
- Jumps from POSSIBILITY (very low bar) to PROOF (very high bar)
- Can't move between games without showing the work

**Proper use:** ✅ "POSSIBILITY: Staging is theoretically possible. PROBABILITY: Evidence is mixed. Factors for staging: [list]. Factors against staging: [list]. PROOF: Additional evidence needed: [what would help]."

---

## The Authority Chain (Wittgenstein's Place)

| What | Source | What It Does |
|------|--------|-------------|
| **Which rules exist** | Case law (Arnold, Stoker, Giles, Menchaca, Nicolau) | Defines legal standards |
| **Why follow them** | State law, professional ethics | Makes violations consequential |
| **How to follow them** | ACFE standards, examples, practice | Provides methods and best practices |
| **Why rules are real** | Wittgenstein's philosophy | Explains that meaning emerges from rule-governed use |
| **How to apply them** | Insurance policy language | Shows how findings map to coverage decisions |

Wittgenstein is at the bottom: he explains the *philosophical foundation* that makes all the others possible. He doesn't provide the rules themselves.

---

## Why Wittgenstein Matters for Judgment

**Investigators often ask:** "Why do I have to follow these rules?"

**Case law answers:** "Because courts require it."

**Wittgenstein explains:** "Because meaning in professional language comes from use. These rules are what make your use of words like 'evidence' and 'fraud' meaningful in the first place. Without the rules, the words are just noise."

This philosophical understanding helps investigators see rules not as arbitrary restrictions, but as the *structure that makes professional communication possible*.

By understanding that language-games have rules, you begin to internalize the rules instead of just memorizing them. You catch violations before you write them because you start seeing language through the framework.

---

## How to Use This in Practice

**In teaching:**
- Mention once: "Professional language has rules because meaning comes from how words are used in professional practice."
- Then move on to the actual rules (case law + examples)

**In feedback:**
- Don't cite Wittgenstein directly
- Cite the rule that was broken
- Cite the case law or standard that backs it up
- The philosophical foundation is the underscore, not the argument

**In design:**
- Wittgenstein justifies why we can extract implicit rules from practice
- But the actual rules come from case law and professional standards
- He explains the system; he's not the system

---

## One-Sentence Summary

Wittgenstein explains why professional language has rules at all. The other four sources (case law, professional standards, policy language, and philosophy) define what those rules are and how to follow them.

---

## For Future Development

If someone asks "Where does that rule come from?" the answer is:

1. **First level:** "From [case law name] or [professional standard]"
2. **Second level:** "Because the system requires it (courts, professional practice)"
3. **Third level (philosophy):** "Because professional language only makes sense when it follows rule-governed use"

Wittgenstein is the third level. Don't skip to him. Start with the first two levels, then add philosophical depth only if the person wants it.
