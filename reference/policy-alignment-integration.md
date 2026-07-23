# Policy Alignment Integration Guide

## Purpose

This guide shows how to incorporate the Texas HO-3 policy into the SIU Language Validator framework, adding a new validation layer: **Policy Alignment Validation**.

---

## Why Policy Alignment Matters

An investigator's job is to present findings. A claims adjuster's job is to apply policy language to those findings and make a coverage decision.

**But:** A good investigation report bridges these roles by explaining **which policy provisions the findings implicate**.

**Example:**

❌ **Poor Report:**
"The insured claims water damage. Damage was confirmed in the dwelling."

✅ **Good Report:**
"The insured claims water damage from a burst hot water heater in the dwelling (Coverage A). The policy covers sudden and accidental water damage from domestic appliances (Peril #12). Investigation confirmed: (1) water source was the hot water heater, not excluded water; (2) loss was sudden and not fungal; (3) property was the dwelling structure, not personal items. **Finding: Within Coverage A as a covered peril.**"

---

## The Policy Alignment Validation Layer

This is a new layer to add to the SIU Language Validator framework:

### Rule: Evidence must map to policy provisions

**Statement:** Every significant investigation finding should explain which policy coverage, peril, condition, or exclusion it relates to.

**Why:** 
- Investigators gather facts
- Claims adjusters apply policy language
- The connection should be explicit, not implicit

**What to Flag:**
1. Findings that don't reference which coverage applies
2. Findings that don't explain if loss is included or excluded
3. Findings that ignore relevant policy limits or special limits
4. Findings that don't address policy conditions (cooperation, proof of loss, etc.)
5. Findings that reach coverage conclusions (that's the adjuster's job, not investigator's)

---

## Integration Points

### 1. Coverage Identification

**Investigator should identify:**
- Which Coverage applies (A, B, or C)?
- For Coverage C, which category of personal property?
- Are there special limits involved?

**Example for Water Damage:**
"The loss involves Coverage A (Dwelling Coverage) because the damage is to the structure of the dwelling, not personal property inside."

**Example for Theft of Jewelry:**
"The loss involves Coverage C (Personal Property) with a special limit of $1,500 for loss by theft of jewelry (per policy definition)."

---

### 2. Peril/Cause of Loss Mapping

**Investigator should identify:**
- What caused the loss? (fire, water, theft, wind, etc.)
- Is that peril listed in Section I – Perils Insured Against?
- If water, is it covered water or excluded water?
- If theft, does excluded theft apply?

**Example for Water Damage:**
"The cause of loss is water from a burst hot water heater. Policy Peril #12 (Sudden and Accidental Water Damage from domestic appliances) covers this. Policy exclusions for water do not apply because: (1) water is not below-ground surface; (2) water is not backed-up water; (3) loss does not involve fungus."

**Example for Theft:**
"The cause of loss is theft of jewelry. Coverage C applies. Special limit of $1,500 for loss by theft of jewelry applies. Theft exclusion for theft by resident under age 21 does not apply because [reason]."

---

### 3. Condition Verification

**Investigator should verify and report on:**
- Was prompt notice given? (investigate timing and prejudice)
- Did insured cooperate with investigation?
- Did insured protect property from further damage?
- Did insured provide detailed inventory?
- Did insured provide bills, receipts, documentation?
- Did insured file proof of loss within 60 days of request?

**Example for Reporting Delay:**
"The insured discovered loss on [date] and reported to insurer on [date], representing a delay of [X hours/days]. Policy requires 'prompt notice.' We have not identified any prejudicial impact from this delay because [reason]. The investigation proceeded normally and obtained all necessary evidence."

**Example for Cooperation:**
"The insured cooperated fully with investigation: (1) answered investigator's questions on [date]; (2) provided requested documentation on [date]; (3) allowed property inspection on [date]; (4) submitted to recorded statement on [date]. No cooperation issues identified."

---

### 4. Limit Verification

**Investigator should verify:**
- Does claim exceed the limit for this coverage?
- If special limit applies (jewelry $1,500, firearms $2,500, etc.), does claim exceed it?
- If replacement cost settlement, is insurance 80%+ of replacement cost?

**Example:**
"The insured claims $800 for stolen jewelry. Coverage C has a special limit of $1,500 for loss by theft of jewelry. The claimed amount is within the special limit."

---

### 5. Exclusion Analysis

**Investigator should evaluate:**
- Could this loss fall under an exclusion?
- Has the investigator considered alternative interpretations?
- Are there facts that would exclude coverage?

**Example for Water Damage:**
"Investigation examined whether the water damage might fall under the policy exclusion for 'water below the surface of the ground.' The water source was an indoor hot water heater at [location], and water damage was confined to [area], confirming this is not below-ground water and the exclusion does not apply."

**Example for Business Property:**
"Investigation examined whether damaged property might be classified as 'business property' under the policy exclusion. The insured stated the damaged items were [personal property description]. No evidence of business use was found. Coverage C applies without business property exclusion."

---

## What NOT to Do

❌ **Don't reach coverage conclusions**
- Investigator should NOT say "Coverage applies" or "Coverage does not apply"
- That's for claims adjuster to decide
- Investigator should present facts and policy language, not conclusions

❌ **Don't ignore policy language**
- If policy has a specific exclusion, address it
- If special limits apply, cite them
- If conditions must be met, verify them

❌ **Don't use vague policy references**
- Don't say "covered under the policy"
- DO say "Coverage A - Dwelling"
- DO say "Peril #12 - Sudden and Accidental Water Damage"

---

## Validation Template for Report Review

### Policy Section Checklist

When reviewing an investigation report, ask:

**Coverage & Peril:**
- [ ] Does report identify which Coverage applies (A, B, or C)?
- [ ] If Coverage C, does it identify the property category?
- [ ] Does report identify the cause of loss (fire, water, theft, etc.)?
- [ ] Does report reference the specific peril in policy (Peril #X)?
- [ ] Does report explain if peril is covered or excluded?

**Special Limits:**
- [ ] Are there special limits that apply?
- [ ] Does report cite the specific limit amount?
- [ ] Does report show claim is within or exceeds the limit?

**Exclusions:**
- [ ] Does report address relevant exclusions?
- [ ] Does report explain why exclusions don't apply (if applicable)?
- [ ] For water damage, does report address water exclusions?
- [ ] For theft, does report address theft exclusions?

**Policy Conditions:**
- [ ] Does report address timing of notice (prompt notice requirement)?
- [ ] Does report address cooperation with investigation?
- [ ] Does report address proof of loss (60-day requirement)?
- [ ] Does report address insured's duties after loss?

**Valuation:**
- [ ] If dwelling loss, does report confirm 80% coinsurance test?
- [ ] If personal property, does report cite actual cash value approach?
- [ ] Are valuations supported by documentation?

---

## Example Reports with Policy Alignment

### Example 1: Water Damage Claim — GOOD

**Report Finding:**
"The insured reported water damage to the dwelling from an apparent burst hot water heater located in the utility room. Investigation verified:

1. **Coverage:** This loss involves Coverage A (Dwelling) because the damage is to the structure of the dwelling.

2. **Cause of Loss:** The cause is water from a burst domestic appliance (hot water heater). Policy Peril #12 provides coverage for 'Sudden and Accidental Water Damage from plumbing, heating, air conditioning systems, or domestic appliances.'

3. **Exclusion Analysis:** The policy excludes water damage that (a) exerts pressure below the surface of the ground, (b) backs up from plumbing, or (c) involves fungus. Investigation findings: Water was confined to the interior utility room and adjacent areas. No evidence of below-ground water, backed-up water, or fungus. The water exclusions do not apply.

4. **Policy Condition:** Notice of loss was provided within [timeframe]. No cooperation issues identified.

5. **Valuation:** Damage to dwelling structure is settled at replacement cost. Building replacement cost documentation supports the claim amount.

**Conclusion for Adjuster:** Findings support coverage under Coverage A, Peril #12. Exclusions do not appear to apply. Claim is within policy limits."

### Example 2: Water Damage Claim — POOR

**Report Finding:**
"The insured claims water damage to the dwelling. Investigation confirmed water damage exists. The claim appears to be covered."

**Problems:**
- Doesn't identify which coverage (A, B, or C)
- Doesn't identify the cause (source of water)
- Doesn't reference specific policy peril
- Doesn't address water exclusions
- Reaches coverage conclusion (investigator's job is to present facts, not make coverage decisions)
- Doesn't cite policy language at all

---

## How This Integrates with Existing Validator

The SIU Language Validator v2.0 has 8 validation layers. Policy Alignment is the 9th:

| Layer | Focus | Example |
|-------|-------|---------|
| 1 | Observation ≠ Interpretation | "Appeared nervous" vs "suggesting deception" |
| 2 | Evidence ≠ Conclusion | "Found vs concluded" |
| 3 | Suspicion ≠ Evidence | "Suspicious" vs proven |
| 4 | Possibility ≠ Probability ≠ Proof | Certainty levels |
| 5 | Motive ≠ Intent | "Financial difficulty" vs "intentional fraud" |
| 6 | Contradiction ≠ Deception | Inconsistency explanation |
| 7 | Precision | Specific facts vs vague language |
| 8 | Language Integrity | Grammar, corruption, accuracy |
| **9** | **Policy Alignment** | **New layer: findings map to policy** |

---

## New Validation Rule for Policy Alignment

### Rule 12: Finding ≠ Policy Interpretation

**Principle:**
Investigators gather facts and explain findings. Policy interpretation belongs to claims adjusters.

**What to Flag:**

1. **Missing Coverage Citation**
   - ❌ "The claim is covered."
   - ✅ "Coverage A applies because the damage is to the dwelling structure."

2. **Missing Peril Reference**
   - ❌ "Water damage to the dwelling."
   - ✅ "Water damage caused by burst hot water heater (Peril #12 - Sudden and Accidental Water Damage from domestic appliances)."

3. **Unaddressed Exclusions**
   - ❌ Report discusses water damage but doesn't address water exclusions
   - ✅ Report discusses water damage AND explains why exclusions don't apply

4. **Unverified Policy Conditions**
   - ❌ No discussion of cooperation, proof of loss, notice, etc.
   - ✅ "Insured cooperated fully. Proof of loss was submitted within 60 days. No condition issues identified."

5. **Reaching Coverage Conclusions**
   - ❌ "Based on investigation, coverage applies."
   - ✅ "The following facts may be relevant to a coverage determination: [facts]."

6. **Ignoring Special Limits**
   - ❌ Report shows jewelry claim of $2,000 without mentioning special limit
   - ✅ "Coverage C applies with a special limit of $1,500 for loss by theft of jewelry. The claim is $2,000, exceeding the limit."

---

## Implementation Steps

### Step 1: Make Policy Accessible
- ✅ Done: TEXAS-HO3-POLICY-STRUCTURED.md created
- Contains quick reference index
- Organized by coverage, peril, exclusion, condition

### Step 2: Add Policy Alignment Rule to Validator
- [ ] Add Rule 12 to siu-language-validator-v2-0.md
- [ ] Include policy-specific examples
- [ ] Explain investigator vs adjuster boundary

### Step 3: Create Policy-Specific Examples
- [ ] Water damage: good vs bad report
- [ ] Theft: good vs bad report
- [ ] Fire/property damage: good vs bad report

### Step 4: Update Validation Findings Template
- [ ] Add policy section to validation reports
- [ ] Include policy citation for each finding
- [ ] Explain relevant coverage/peril/exclusion

### Step 5: Test on Example Reports
- [ ] Apply policy alignment validation to test-report-random-4.md
- [ ] Verify policy gaps are identified
- [ ] Refine criteria as needed

---

## Benefits of Policy Alignment Validation

✅ **For Investigators:**
- Clearer handoff to claims
- Reduces back-and-forth questions
- Demonstrates thoroughness

✅ **For Claims Adjusters:**
- Faster coverage determination
- Clear evidence of policy analysis
- Easier to explain denial to insured

✅ **For Disputes:**
- Investigator findings are well-grounded in policy
- Easy to defend coverage decision
- Insured can see reasoning

✅ **For Compliance:**
- Demonstrates reasonable investigation
- Shows policy terms were considered
- Reduces bad-faith claims

---

## Next Steps

1. **Review** this integration guide
2. **Validate** test-report-random-4.md against both SIU Validator AND policy alignment criteria
3. **Create examples** showing policy-aligned reports
4. **Update validator framework** to include Rule 12 (Policy Alignment)
5. **Test** on all example cases (water damage, theft, fire)

---

**Document Status:** Ready for implementation  
**Date Created:** 2026-07-22  
**Policy Referenced:** Texas HO-3 (HO 00 03 10 00)  
**Integration:** SIU Language Validator v2.0 + Policy Alignment Layer
