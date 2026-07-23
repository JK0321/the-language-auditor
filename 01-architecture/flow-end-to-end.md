# End-to-End Flow: Using the The Language Auditor

## Stage 1: Investigator Prepares Report

**What the investigator does:**
- Completes their investigation (interviews, documents, analysis)
- Writes up findings in a report (email, Word doc, plain text — any format)
- Decides: "Is this report as good as it needs to be?"
- Opens Claude.ai
- Creates or opens the The Language Auditor project
- Pastes the report

---

## Stage 2: Validator Receives Report

**What Claude (running the validator) does:**

The system prompt activates. Claude is now:
- An expert in professional investigative language
- Armed with 11 specific rules (Observation ≠ Interpretation, Evidence ≠ Conclusion, etc.)
- Guided by 4 severity levels (Critical → High → Medium → Low)
- Grounded in case law authority (Arnold, Stoker, Giles, Menchaca)

Claude reads the report and displays:
```
"I'll review this investigative report for professional language violations. 
I'll look at:
- Evidence traceability (is every fact sourced?)
- Observation/interpretation boundaries (is conclusion separated from fact?)
- Professional language rules (are terms used correctly?)
- Professional boundaries (does the writer stay in role?)

Here are the violations I found:"
```

---

## Stage 3: Validator Scans All Text

**Layer 1: Source Attribution (Foundation Layer)**
- ✓ Does every material fact have a source?
- ✓ Can reader trace: who said this? when? where? how do we know?
- 🚩 **Violation found?** "The claimant made inconsistent statements" (missing: when, to whom, what exactly)

**Layer 2: Observation vs Interpretation (Separation Layer)**
- ✓ Are observations kept separate from conclusions?
- ✓ Does the writer report what they saw, then explain what it could mean?
- 🚩 **Violation found?** "The claimant appeared fraudulent" (mixes observation with psychological judgment)

**Layer 3: Evidence Standards (Documentation Layer)**
- ✓ Are only documented facts used as evidence?
- ✓ Is suspicion labeled as suspicion, not evidence?
- ✓ Does probability match the evidence quality?
- 🚩 **Violation found?** "I suspected fraud, and determined it happened" (suspicion ≠ evidence)

**Layer 4: Professional Boundaries (Role Layer)**
- ✓ Did investigator stay in role (reporting facts, not making decisions)?
- ✓ Does the report recommend findings for review, not make coverage decisions?
- ✓ Are allegations clearly marked as unverified?
- 🚩 **Violation found?** "I recommend we deny this claim" (that's a coverage decision, not an investigative finding)

**Layer 5: Language Precision (Terminology Layer)**
- ✓ Are professional terms used correctly?
- ✓ Is "contradiction" mistaken for "deception"?
- ✓ Is "missing evidence" mistaken for "concealment"?
- ✓ Is policy language quoted, not interpreted?
- 🚩 **Violations found?** Multiple misuses of professional terminology

---

## Stage 4: Validator Prioritizes Violations

**Sorting by severity:**

🔴 **CRITICAL** (professional boundary violations)
- Makes coverage decision instead of recommending findings
- Confuses intent with motive in fraud determination
- Oversteps investigator role

🟠 **HIGH** (evidence standard violations)
- Conclusion exceeds evidence
- Suspicion presented as fact
- Facts without sources

🟡 **MEDIUM** (clarity violations)
- Unclear traceability
- Vague terminology
- Missing context

🟢 **LOW** (style/organization)
- Could be clearer
- Better organization possible
- Not professionally wrong, just could improve

**Validator lists violations in this order** (Critical first, Low last).

---

## Stage 5: Validator Explains Each Violation

For each violation found, Claude provides:

### Example Violation Report:

**🔴 FLAG: Contradiction ≠ Deception** (Line 12, High Severity)

**Rule Violated:** Rule #6 (Contradiction ≠ Deception)

**Your Original Text:**
```
"The claimant's two statements contradicted each other. 
This proves the claimant was being deceptive."
```

**Explanation:** 
You observed a contradiction (good—report it). But contradiction ≠ proof of deception. Deception requires intent, which is not observable from contradiction alone. The contradiction could be:
- Memory error (innocent)
- Misunderstanding (innocent)  
- Intentional misstatement (culpable)

**Authority:** 
Arnold v. National County requires documented basis. Courts distinguish between observable contradiction and inferred intent. See reference/03-GILES-STANDARD.md.

**Suggestion for Improvement:**
```
"Claimant's first statement (Date, to Person): '[exact quote].'
Claimant's second statement (Date, to Person): '[exact quote].'
These statements contradict on this point: [specific difference].
This inconsistency is noteworthy. 

Possible explanations: 
(1) Memory lapse, (2) Misunderstanding, (3) Intentional misstatement.

Evidence that would distinguish between them:
[List what additional facts would clarify which scenario applies]"
```

---

## Stage 6: Investigator Reads Feedback

**What happens now:**

The investigator gets back:
- A prioritized list of violations (worst first)
- For each: specific line/paragraph reference
- The actual language that violated the rule
- WHY the rule exists (not just "you're wrong")
- A concrete example of how to fix it
- Authority for the rule (case law reference)

**Investigator's decision point:**
- "Do I agree this is a violation?" (Usually yes—rules are based on case law)
- "Do I want to fix it?" (Their call)
- "How should I fix it?" (They write the improvement; validator only suggests)

---

## Stage 7: Investigator Revises (Optional Loop)

**Option A: Ignore the feedback**
- Investigator decides a flag isn't relevant to their case
- They submit the report as-is
- That's fine. Validator is advisory, not mandatory.

**Option B: Fix some violations**
- Investigator revises the sentences the validator flagged
- They improve sourcing, separate observation from interpretation, etc.
- They decide *how* to fix it (validator only suggests)
- Report gets stronger

**Option C: Fix all violations**
- Investigator systematically addresses every flag
- Report now passes all 11 professional language rules
- Findings are legally defensible, traceable, professionally sound

**Optional: Re-submit for another pass**
- Investigator can paste the revised report back into the validator
- Validator flags any remaining violations
- Loop continues until investigator is satisfied

---

## Stage 8: Investigator Submits Final Report

**What's different now:**

**Before validator:**
- Report might have vague sources
- Observations blurred with interpretations
- Suspicion presented as evidence
- Coverage decisions mixed into findings
- Vulnerable to challenge in court

**After validator:**
- Every fact has a documented source
- Observations clearly separated from conclusions
- Evidence is hard evidence, suspicion is labeled suspicion
- Investigator stays in role (recommends, doesn't decide)
- Report survives appellate review because it follows case law

---

## Stage 9: Report in the Real World

**Who reviews it:**
- Claims manager (can act on the findings)
- Coverage specialist (can make policy decisions)
- Legal team (can defend it if challenged)
- Judge (if case goes to trial)

**What they see:**
- Professional, traceable investigation
- Clear distinction between fact and interpretation
- Well-documented evidence
- Investigator stayed in role
- **Follows Arnold, Stoker, Giles, Menchaca standards**

**What doesn't happen:**
- "Where did this come from?"
- "What does this actually prove?"
- "Did the investigator step out of role here?"
- "Is this defensible?"
- → All answered. No gaps.

---

## The Loop Over Time

**One report:**
- Investigator learns 1-3 rules through practice
- Next report, they catch 1-3 of those violations themselves
- Validator still flags new violations

**10 reports:**
- Investigator has internalized 5-6 rules
- Writes better the first time
- Validator flags fewer violations
- Process gets faster

**30-50 reports:**
- Investigator has internalized most/all 11 rules
- Thinks like a professional investigator
- Uses the validator less as a corrector, more as a final audit
- Judgment has improved dramatically

---

## Summary: What Actually Happens

```
REPORT → VALIDATOR SCANS (5 layers) → PRIORITIZES BY SEVERITY → 
EXPLAINS EACH VIOLATION → INVESTIGATOR DECIDES WHAT TO FIX → 
INVESTIGATOR REVISES → [LOOP OR SUBMIT] → 
LEGALLY DEFENSIBLE FINDINGS → REAL WORLD USE
```

**The validator doesn't:**
- Rewrite sentences
- Make investigative decisions
- Decide coverage outcomes
- Force compliance

**The validator does:**
- Identify where language violates professional standards
- Explain why the standard exists (case law)
- Show what better language looks like
- Let the investigator own the improvement

**The result:**
- Investigator learns professional reasoning, not just compliance
- Reports survive scrutiny because they follow case law
- SIU teams produce higher-quality work over time
- Claims decisions are defensible

