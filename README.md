﻿# The Language Auditor

**An editor for SIU investigators that teaches the rules of professional investigative language.** Not a rewriter. Not a decision-maker. A language coach.

🌐 **[View the Landing Page](https://JK0321.github.io/the-language-auditor/landing.html)** — Interactive introduction to the system

---

## What It Solves

SIU investigators write reports in a high-pressure environment. Courts, juries, and claims adjusters evaluate your language, not just your facts.

**The problem:** You learn rules implicitly. Get corrected by supervisors. See cases thrown out. But the rules themselves aren't documented—so each investigator reinvents the wheel and makes similar mistakes across investigations.

**The system:** This validator externalizes the rules. It flags where your language violates professional standards and explains why it matters.

---

## How It Works

**Input:** Your investigative report (any format—email, Word, PDF, plain text).

**Output:** Structured feedback for each violation.
- **Where:** Line/paragraph
- **What:** The violation
- **Why:** The rule and authority behind it
- **How:** Specific rewrite suggestion

**Your role:** You decide what to fix. The report stays yours.

---

## What The Rules Are

The validator enforces **12 professional language distinctions** drawn from Texas case law, ACFE standards, and insurance policy language. These are the rules experienced investigators know but rarely write down.

| Rule | What It Prevents |
|------|-----------------|
| **Evidence != Conclusion** | Letting your interpretation override what the evidence actually shows |
| **Suspicion != Evidence** | Using gut feeling as proof |
| **Possibility != Probability != Proof** | Overstating certainty ("it's possible" → "it's proven") |
| **Intent != Motive** | Confusing "why someone wanted to" with "proof they deliberately did" |
| **Contradiction != Deception** | Treating inconsistent statements as proof of lying |
| **Finding != Allegation** | Using prosecutor language when you're an investigator |
| **Missing Evidence != Concealment** | Inferring someone's hiding something from absence of evidence |
| **Correlation != Causation** | Connecting two facts without proof one caused the other |
| **Authority Boundaries** | Staying in investigator role, not making adjuster decisions |

See: `rules.md` for full definitions and examples.

---

## Why These Rules Matter

**When you follow them:**
- [YES] Findings are legally defensible
- [YES] Adjusters can act on your work
- [YES] Reports hold up in court
- [YES] You stay in role (avoid liability)
- [YES] You catch mistakes before submission

**When you don't:**
- [NO] Conclusions get challenged
- [NO] Reports sent back for revision
- [NO] Cases thrown out on language grounds
- [NO] You create legal exposure
- [NO] Next investigation repeats the same errors

---

## The Foundation (4 Authority Sources)

Rules don't exist in a vacuum. They come from five authority layers that define what "professional" means:

1. **Texas Case Law** (Arnold, Stoker, Giles, Menchaca, Nicolau) — what courts require
2. **ACFE Professional Standards** — Certified Fraud Examiner best practices
3. **Texas Insurance Code** — statutory foundation
4. **Actual Policy Language** (HO-3) — what adjusters must follow
5. **Professional Language-Games** (Wittgenstein) — philosophical foundation explaining why rules exist

Each rule is anchored to specific case law or professional standard. When the validator flags a violation, it cites authority.

See: `identity.md` for full authority layer breakdown; `reference/LEGAL-FOUNDATION-SUMMARY.md` for master case law reference.

---

## Proof: How To Test It

**Official test case (included):**

1. Read `sample-reports/00-water-damage-official.md` (5 min) — Professional investigation
2. Note where language could be stronger (don't look ahead)
3. Paste it into Claude with this project and ask: `edit`
4. Compare to `sample-reports/01-official-case-critique.md` — See what the editor flags

This shows exactly how the system works on a real case.

**Real example: Contradiction != Deception**

[BAD] "The claimant's two statements contradicted each other. This proves the claimant was being deceptive."

[GOOD] "Statement 1 (date, to person): '[quote].' Statement 2 (date, to person): '[quote].' These contradict on [specific point]. Possible causes: (1) memory error, (2) misunderstanding, (3) intentional. Evidence to distinguish: [what would help]."

**Why:** Contradiction is observable. Deception is intent. You can't see intent. What you *can* do is investigate the gap between them.

---

## Design Choices (Why This Structure)

**Why 12 rules, not 50?** Because most violations fall into 12 core distinctions. Keeping the list short makes it memorable and applicable.

**Why authority sources?** Because "that's the rule" won't stick. "That's the rule *because Texas courts require it*" does. Rules with authority behind them are enforceable.

**Why examples?** Because abstract rules don't stick. Real violations with real fixes do.

**Why no rewriting?** Because if I rewrite, you become dependent. If I teach, you become independent. By month 3, you catch violations before you write them.

See: `identity.md` for full design philosophy.

---

## Similar Systems That Won

**Week 7 (Nightwatch):** Praised for "externalizing judgment into the folder" so the operator works without explanation. Rules lived in the structure, not in Gabriel's head.

**Week 8 (chalky-prd):** Praised for "shipping receipts"—real user transcripts with full context, showing the system works on actual work, not simulations.

**This system:** Externalizes the 12 rules into a repeatable structure. Includes receipts (real violations, real fixes). Makes judgment visible in the folder, not locked in explanations.

---

## Quick Start

**Fastest way to see this in action:**

1. **identity.md** (1 min) — Who we are
2. **sample-reports/00-water-damage-official.md** (5 min) — Read a real investigation  
3. **sample-reports/01-official-case-critique.md** (5 min) — See what the editor flags
4. **examples.md** (10 min) — More examples with case law citations
5. **Try it:** Paste your own report and ask: `edit`

**Total:** 20 minutes to proficiency.

---

## What This Is NOT

- [NO] A decision engine (won't tell you whether to deny a claim)
- [NO] A rewriter (won't rewrite your sentences)
- [NO] Generic feedback ("strengthen your intro")
- [NO] A compliance checkbox (though it ensures compliance)
- [NO] A replacement for your judgment (you make the final call)

---

## Status

**Status:** Complete with 12 rules, 8 validation layers, 5 authority layers, comprehensive reference materials, and real test cases

---

## How to Use It (Step-by-Step)

### Step 1: Try the official test case first

We've included a real investigation report (`sample-reports/00-water-damage-official.md`) showing a professional water damage claim investigation.

**Try this workflow:**
1. Read the official water damage report
2. Note the areas where it could be clearer (don't peek at the critique yet)
3. Paste it into Claude with this project
4. Ask: “edit”
5. See what the editor flags
6. Compare to the violations listed in `sample-reports/01-official-case-critique.md`

This shows you exactly how the system works on a real report.

### Step 2: Copy your own report

Copy your investigative report text. Any format is fine (email, Word doc, PDF—just plain text, or ask Claude/ChatGPT to generate one [it will still work]).

### Step 3: Drop it in Claude with the project

Open Claude and load the Investigative Language Validator project.

Paste your report.

Ask: “edit”

### Step 4: Read the feedback

For each violation flagged, you get:
- **Where:** Line number or paragraph
- **What:** The specific violation
- **Why:** The professional rule
- **Authority:** Where that rule comes from
- **Suggestion:** How you could improve it

### Step 5: Decide what to fix

You decide which suggestions make sense. You write the improvements. The report stays yours.

---

## What Good Feedback Looks Like

### Example: Contradiction !=!=  Deception

**Your original text:**
"The claimant's two statements contradicted each other. This proves the claimant was being deceptive."

**Our feedback:**

**FLAG: Contradiction !=!=  Deception**
- **Rule violated:** Professional Language Game, Rule #6
- **Explanation:** You observed a contradiction (good—”report it). But contradiction !=!=  proof of deception. Deception requires intent, which is not observable from contradiction alone. The contradiction could be memory error, misunderstanding, or intentional.
- **Authority:** Professional investigative standards; Arnold case law standard
- **Suggestion:** "The claimant's first statement (date, to person): '[quote or summary].' Second statement (date, to person): '[quote or summary].' These contradict on this point: [specific difference]. This is noteworthy. Possible explanations: (1) memory error, (2) misunderstanding, (3) intentional misstatement. Evidence to distinguish: [what would help]."

---

### Example: Source Attribution

**Your original text:**
"The neighbors reported suspicious activity on the loss date."

**Our feedback:**

**FLAG: Source Attribution Missing**
- **Rule violated:** Every fact must have a source (Rule #11)
- **Explanation:** Which neighbors? What specifically did they report? To whom? When? Without this, the statement is vague and non-verifiable.
- **Authority:** Professional standards; legal defensibility
- **Suggestion:** "Neighbor statement (name, date, documented interview): '[exact quote about what was observed].' Neighbor statement (name, date, documented interview): '[exact quote].' Pattern observed: [what multiple sources said]."

---

### Example: Finding !=!=  Policy Interpretation (NEW)

**Your original text:**
"The dwelling suffered water damage. The claim appears to be covered."

**Our feedback:**

**FLAG: Finding !=!=  Policy Interpretation**
- **Rule violated:** Finding must map to specific policy language (Rule #12)
- **Explanation:** Which coverage applies (A, B, or C)? What peril caused the loss? Are exclusions relevant? What limits apply? Without citing specific policy language, the adjuster has to reverse-engineer your reasoning. Professional reports map findings to policy.
- **Authority:** ACFE standards; Insurance policy language; Role boundaries
- **Suggestion:** "The insured reported water damage from burst hot water heater (Coverage A - Dwelling). Policy Peril #12 covers 'Sudden and Accidental Water Damage from domestic appliances.' Investigation verified: (1) water source is domestic appliance; (2) policy exclusions for below-ground water, backed-up water, and fungus do not apply; (3) insured gave prompt notice and cooperated fully. For adjuster: Findings support coverage under Coverage A, Peril #12."

---

## What Professional Language Looks Like

Professional investigative language:
- [YES] Sources every fact ("On 1/14, the adjuster noted...")
- [YES] Separates observation from interpretation ("I observed X. This could mean Y because...")
- [YES] Doesn't assume intent ("The discrepancy occurred. It could be error or intentional. Evidence distinguishing: ...")
- [YES] Quotes policy language ("Section 4 states: '[exact quote]'")
- [YES] Stays in role ("Findings: ... Recommendation for legal review: ...")
- [YES] Documents contradictions ("Statement 1: ... Statement 2: ... Difference: ...")

Non-professional language:
- [NO] Vague sourcing ("It was reported that...")
- [NO] Mixes observation/conclusion ("The claimant appears fraudulent")
- [NO] Assumes intent from circumstance ("The delay proves deception")
- [NO] Paraphrases policy ("The policy clearly means...")
- [NO] Makes coverage decisions ("I recommend we deny")
- [NO] Ignores alternatives ("The evidence proves fraud")


---

## The Rules We Check

We validate against **12 professional language rules:**

1. **Observation !=!=  Interpretation** —” Report what you saw. Then explain what it could mean.
2. **Evidence !=!=  Conclusion** —” Report facts. Let decision-makers decide what they mean.
3. **Suspicion !=!=  Evidence** —” Document specific facts, not gut feelings.
4. **Possibility !=!=  Probability !=!=  Proof** —” Be precise about certainty level.
5. **Intent !=!=  Motive** —” Motive (why) is not the same as intent (deliberate choice).
6. **Contradiction !=!=  Deception** —” Inconsistency is observable. Intent is not.
8. **Finding !=!=  Allegation** —” Distinguish verified facts from unverified claims.
9. **Missing Evidence !=!=  Concealment** —” Distinguish "couldn't find" from "someone is hiding."
10. **Correlation !=!=  Causation** —” Separate correlation from causal relationships.
11. **Authority Boundaries** —” Stay in investigator role. Don't make adjuster decisions.

See `rules.md` for full definitions and examples.

---

## The 8 Validation Layers

Beyond the 12 rules, the validator checks across 8 distinct dimensions:

1. **Evidentiary Chain** —” Facts must be traceable from evidence !=’ finding !=’ investigative issue !=’ recommendation
2. **Policy Alignment** —” Findings must map to specific coverage, perils, exclusions, limits, and conditions
3. **Alternative Hypothesis** —” Investigator must consider and document reasonable alternative explanations
4. **Precision** —” Use specific facts, dates, quotes, and measurements (not vague language)
5. **Language Integrity** —” Grammar, corruption detection, defined acronyms, clear pronoun references
6. **Confirmation Bias** —” Report objectively; don't write to prove a predetermined conclusion
7. **Inferential Ladder** —” Don't skip levels (observation !=’ conclusion without intermediate steps)
8. **Investigation Completeness** —” What investigative work should have been done? Is it documented?

Together, the 12 rules and 8 layers create a comprehensive framework for professional investigative writing.

The complete validation framework details are embedded in the Claude project instructions.

---

## Why This Matters

Professional investigative language has rules.

When you follow them:
- [YES] Your findings are legally defensible
- [YES] Decision-makers can act on your work
- [YES] Your reports are traceable and auditable
- [YES] You avoid overreach (stay in your role)
- [YES] You improve your judgment

When you don't:
- [NO] Conclusions get challenged
- [NO] Findings get questioned
- [NO] Reports lack traceability
- [NO] You overstep your role
- [NO] Your next investigation repeats mistakes


This editor helps you catch yourself. Over time, you internalize the rules and catch violations before you write them.

---

## The Complete Foundation (5 Authority Layers)

### 1. Wittgenstein's Philosophy
**Language-Games Theory:** Professional language gets meaning only through its use in professional practice. Words like "evidence," "fraud," and "finding" have determinate meaning because they're governed by professional rules—”not because meaning is arbitrary.

### 2. Texas Case Law (4 Foundational Cases)
- **Arnold v. National County** (1987) —” "Reasonable documented basis" for findings
- **Stoker v. State Farm** (1985) —” Coverage denial requires valid reason
- **Giles v. State Farm** (1995) —” Timely payment and clear liability
- **Menchaca v. State Farm** (2003) —” Reasonable investigation and clear explanation

### 3. ACFE Professional Standards
Association of Certified Fraud Examiners standards for professional fraud examination reporting. These validate and reinforce the 12 rules as industry best practice.

### 4. Texas Insurance Code
Statutory requirements for investigation, cooperation, proof of loss, and coverage decisions.

### 5. Actual Insurance Policy Language
Real HO-3 homeowners policy (not summaries or paraphrases). Investigators must map findings to specific coverage provisions, perils, exclusions, limits, and conditions.

---

## What's Included

- **identity.md** —“ Who we are and what we do (includes 5 authority layers)
- **rules.md** —“ The 12 professional language rules we check
- **examples.md** —“ What good/bad feedback looks like (with case law citations)
- **reference/** —“ Complete case law, policy language, rubrics, checklists, sample violations
  - 01-arnold-standard.md through 05-nicolau-standard.md (5 Texas cases: Arnold, Stoker, Giles, Menchaca, Nicolau)
  - texas-ho3-policy-structured.md (actual insurance policy)
  - policy-alignment-integration.md (how to map findings to policy)
  - acfe-alignment.md (professional standards mapping)
  - LEGAL-FOUNDATION-SUMMARY.md (comprehensive legal reference)

---

## Start Here

**Quickest way to understand this editor:**

1. Read `identity.md` (30 seconds) —” Who we are
2. Open `sample-reports/00-water-damage-official.md` (5 minutes) —” Read the official investigation report
3. Open `sample-reports/01-official-case-critique.md` (5 minutes) —” See what the editor flags
4. Review `examples.md` (10 minutes) —” See more examples
5. **Try it yourself:** Drop your report into Claude with this project

**The water damage report is your test case.** It shows a professional, well-structured investigation with 3 minor improvements the editor would recommend.

---

## Questions?

**Q: Will this change my report without asking?**
A: No. We only flag violations and suggest improvements. You stay in control.

**Q: What if I disagree with a flag?**
A: You're the expert on your investigation. If a rule doesn't apply, you decide. But we'll explain why the rule exists.

**Q: Does this tell me whether I should deny a claim?**
A: No. We validate language. Coverage and liability decisions are yours (or your manager's). We help your findings be as professional and defensible as possible.

**Q: Can I use this for other types of documents?**
A: This version is built for investigative reports. The rules could extend to other professional writing, but start here.






