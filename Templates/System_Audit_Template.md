# System Design Audit Template

## COMPANY INFORMATION
**Company Name:**  
**Website:**  
**Industry/Domain:**  
**Size (employees):**  
**Contact Person:**  
**Person's Role:**  
**LinkedIn Profile:**  

---

## WORKFLOW ANALYSIS

### TRIGGER: What Starts This Process?
- Event-based (customer action, data arrival, scheduled time)?
- Frequency (hourly/daily/on-demand)?
- Volume (how many per day/week)?

Example:
```
Trigger: Customer submits insurance claim via web form
Frequency: ~200 claims/day
Peak times: End of month
```

---

### CURRENT WORKFLOW: Step-by-Step
Map out the entire process from trigger to output:

1. **Step 1:** [What happens first]
   - Who does it: [Role]
   - Tools used: [Software/systems]
   - Time taken: [Estimate]
   - Pain points: [What slows it down]

2. **Step 2:** [Next action]
   - Who does it:
   - Tools used:
   - Time taken:
   - Pain points:

3. **Step 3:** [Continue...]

---

### DECISION POINTS: Where Humans Make Choices
List every point where someone must decide something:

| Decision Point | Current Process | Criteria Used | Time Taken | Error Rate |
|----------------|----------------|---------------|------------|------------|
| Classify claim type | Manual review | Experience + checklist | 5-10 min | ~15% misclass |
| Approve/reject | Manager review | Policy rules + judgment | 20-30 min | Unknown |

---

### CURRENT OUTPUT & QUALITY
- What gets produced at the end?
- Quality metrics (accuracy, completeness, consistency)?
- Current SLA/turnaround time?
- Bottlenecks?

---

## AI SYSTEM DESIGN

### PROPOSED AGENTIC SYSTEM

**Architecture Level:** (Choose one)
- [ ] L1: Single LLM with prompt engineering
- [ ] L2: LLM + tools + planning layer
- [ ] L3: Multi-agent orchestration

### TRIGGER → DECISION → OUTPUT MAPPING

#### Layer 1: Data Intake & Preprocessing
- **What:** [Extract structured data from inputs]
- **How:** [NLP extraction / structured parsing / OCR]
- **Output:** [Structured JSON/data format]

#### Layer 2: Classification & Routing
- **What:** [Categorize and prioritize]
- **How:** [LLM classification / rule-based / hybrid]
- **Confidence threshold:** [When to escalate to human]

#### Layer 3: Decision Support
- **What:** [Generate recommendations]
- **How:** [RAG over policy docs / decision tree / ML model]
- **Human in loop:** [ALWAYS for: final approval, money decisions, legal]

#### Layer 4: Action Execution
- **What:** [Automated steps after approval]
- **How:** [API calls / database updates / notifications]
- **Rollback:** [How to undo if wrong]

#### Layer 5: Learning & Feedback
- **What:** [Track outcomes and improve]
- **How:** [Log decisions, human corrections, success metrics]
- **Memory:** [Session / Profile / System level]

---

### HUMAN-IN-THE-LOOP (GOLDEN RULE)
**LLM NEVER makes final calls on:**
- [ ] Money/financial decisions
- [ ] Legal/compliance decisions  
- [ ] Health/safety decisions
- [ ] [Add domain-specific critical decisions]

**Where human stays:**
- Review point 1: [When/where]
- Review point 2: [When/where]
- Override capability: [How human can correct]

---

### MEMORY REQUIREMENTS
- [ ] **Conversation memory:** Track this specific case across multiple interactions
- [ ] **Session memory:** Remember context within this workflow instance
- [ ] **Profile memory:** Learn user preferences and patterns
- [ ] **System memory:** Company policies, historical decisions, knowledge base

---

### EXPECTED VALUE

#### Time Savings
- Current time per workflow: [X hours/minutes]
- With AI system: [Y hours/minutes]
- **Time saved:** [X-Y per instance]
- **Scale:** [Volume × time saved = total impact]

#### Error Reduction
- Current error rate: [Z%]
- Expected with AI: [W%]
- **Errors prevented:** [Z-W % × volume]

#### Cost Impact
- Labor cost saved: [$X per instance × volume]
- Implementation cost: [$Y one-time + $Z ongoing]
- **ROI timeline:** [Months to break even]

---

## FAILURE MODES & HANDLING

### Failure Mode 1: [Most likely failure]
- **Cause:** [Why it would fail]
- **Detection:** [How system knows it failed]
- **Fallback:** [What happens when it fails]
- **Recovery:** [How to get back on track]

### Failure Mode 2: [Second likely failure]
- **Cause:**
- **Detection:**
- **Fallback:**
- **Recovery:**

---

## TECHNICAL REQUIREMENTS

### Data Requirements
- [ ] Access to: [Databases/APIs/documents needed]
- [ ] PII handling: [How sensitive data is protected]
- [ ] Retention: [How long data is kept]

### Integration Points
- [ ] System 1: [CRM/ERP/etc] - Purpose: [Why]
- [ ] System 2: [Platform] - Purpose: [Why]

### Security & Compliance
- [ ] Data isolation: [Multi-tenant if applicable]
- [ ] Audit trail: [What gets logged]
- [ ] Compliance: [GDPR/HIPAA/SOC2/etc]

---

## IMPLEMENTATION PHASES

### Phase 1: Proof of Concept (2-4 weeks)
- [ ] Build on 10-20 real examples
- [ ] Measure: [Key metric]
- [ ] Success criteria: [What proves it works]

### Phase 2: Pilot (1-2 months)
- [ ] Run on [X%] of workflows
- [ ] Side-by-side with current process
- [ ] Collect: [Human feedback, error rates, time savings]

### Phase 3: Scale (2-3 months)
- [ ] Roll out to [X%] → [Y%] → full
- [ ] Monitor: [Performance metrics]
- [ ] Iterate: [Based on feedback]

---

## OUTREACH MESSAGE (DRAFT)

**Subject:** [Workflow improvement opportunity for [Company]]

Hi [Name],

[Specific observation about their company/role - something real you noticed]

I mapped out what I think is your [specific workflow process] and designed an agentic AI system that could [specific benefit - time/accuracy/cost].

Here's the workflow audit and system design: [Attach or paste key points]

Key points:
- [Trigger]: [What starts it]
- [Current bottleneck]: [Specific pain point]
- [Proposed solution]: [2-3 sentences on the system]
- [Expected value]: [Concrete number - X hours saved, Y% fewer errors]

Let me know if this is useful or if I got something wrong about your process. Happy to discuss.

[Your name]

---

## NOTES & OBSERVATIONS
[Any additional insights, assumptions, or questions]
