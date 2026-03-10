# **Agentic Sales System:**

# **Simplified Illustrations**

Table of Content

[**Agentic Sales Systems: Simplified Illustrations	1**](#agentic-sales-system)

[**SYSTEM 1: Opportunity Generation Engine	2**](#system-1-opportunity-generation-engine)

[**SYSTEM 2: Opportunity Pursuit System	4**](#system-2-opportunity-pursuit-system)

[**HOW THE TWO SYSTEMS CONNECT	7**](#how-the-two-systems-connect)

[**EXPAND WORKFLOW: Detailed Example	8**](#expand-workflow-detailed-example)

[**ACQUIRE WORKFLOW: Detailed Example	14**](#acquire-workflow-detailed-example)

[**ENTER WORKFLOW: Detailed Example	22**](#enter-workflow-detailed-example)

[**SUMMARY: Three Ways to Communicate	33**](#summary-three-ways-to-communicate)

[**Value Proposition	34**](#value-proposition)

## **Overview**

The full Agentic Sales System contains 26 AI agents across three layers (Strategy, Management, Execution). For practical implementation, these agents are organized into two core systems that every B2B sales organization needs:

1. **Opportunity Generation Engine** — systematically creates qualified opportunities aligned with strategy  
2. **Opportunity Pursuit System** — systematically converts qualified opportunities into closed deals

Each system can be implemented independently, though they deliver maximum value when connected.

---

# **SYSTEM 1: Opportunity Generation Engine**

## **Purpose**

Transform strategy into a predictable flow of qualified sales opportunities.

## **The Problem It Solves**

Most sales teams chase whatever comes in the door. Pipeline is unpredictable. Salespeople waste time on wrong-fit prospects. Marketing generates leads that sales ignores. There's no systematic way to create opportunities aligned with company strategy.

## **Simplified Agent Architecture**

```
┌─────────────────────────────────────────────────────────────────────┐
│                        STRATEGY LAYER                               │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐  │
│  │ Segment Strategy │  │    Offering      │  │ Value Proposition│  │
│  │      Agent       │→ │  Configuration   │→ │   Optimization   │  │
│  │                  │  │      Agent       │  │      Agent       │  │
│  │ WHO to target    │  │ WHAT to offer    │  │ WHY they buy     │  │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘  │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│                       EXECUTION LAYER                               │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐  │
│  │    Prospect      │  │    Outreach      │  │    Discovery     │  │
│  │  Intelligence    │→ │   Automation     │→ │      Agent       │  │
│  │      Agent       │  │      Agent       │  │                  │  │
│  │ Research targets │  │ Engage at scale  │  │ Understand needs │  │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘  │
│                                                       │             │
│                                                       ▼             │
│                                    ┌──────────────────┐             │
│                                    │  Qualification   │             │
│                                    │      Agent       │             │
│                                    │                  │             │
│                                    │ Go / No-Go       │             │
│                                    └──────────────────┘             │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                          ┌─────────┴─────────┐
                          ▼                   ▼
                   ┌────────────┐      ┌────────────┐
                   │  QUALIFIED │      │    LEAD    │
                   │OPPORTUNITY │      │  NURTURING │
                   │            │      │   AGENT    │
                   │ → Pursuit  │      │            │
                   │   System   │      │ Not ready  │
                   └────────────┘      │ yet, stay  │
                                       │ in touch   │
                                       └────────────┘
```

## **Core Agents (7 agents)**

| \# | Agent | Function | Key Output |
| ----- | ----- | ----- | ----- |
| 1 | Segment Strategy Agent | Define WHO to target | ICPs, segment priorities, target lists |
| 2 | Offering Configuration Agent | Define WHAT to offer each segment | Packages, pricing, engagement models |
| 3 | Value Proposition Optimization Agent | Define WHY they should buy | Segment-specific messaging |
| 4 | Prospect Intelligence Agent | Research target accounts | Company profiles, buying signals |
| 5 | Outreach Automation Agent | Engage prospects at scale | Personalized multi-channel outreach |
| 6 | Discovery Agent | Understand needs and stakeholders | Needs analysis, DMU mapping |
| 7 | Qualification Agent | Decide go/no-go | Opportunity scores, qualification decisions |

**\+1 Supporting Agent:** | 8 | Lead Nurturing Agent | Maintain not-yet-ready prospects | Nurture sequences, re-engagement triggers |

## **Key Metrics**

* Number of qualified opportunities created per month  
* Qualification rate (% of engaged prospects that qualify)  
* Cost per qualified opportunity  
* Strategy alignment score (% of opportunities matching ICP)  
* Time from first contact to qualified opportunity

## **Business Impact**

* **Predictable pipeline**: Know how many opportunities you'll generate  
* **Higher quality**: Only qualified, strategy-aligned opportunities enter pipeline  
* **Lower waste**: Stop chasing wrong-fit prospects  
* **Sales focus**: Salespeople work opportunities, not hunt for them

---

# **SYSTEM 2: Opportunity Pursuit System**

## **Purpose**

Convert qualified opportunities into closed deals efficiently and consistently.

## **The Problem It Solves**

Salespeople reinvent the wheel on every deal. Proposals take too long. Value arguments are generic. Deals stall without clear next steps. Win rates are low because qualification was weak and execution is inconsistent.

## **Simplified Agent Architecture**

```
┌─────────────────────────────────────────────────────────────────────┐
│                     FROM OPPORTUNITY GENERATION                     │
│                    ┌──────────────────────────┐                     │
│                    │   QUALIFIED OPPORTUNITY  │                     │
│                    │   - Needs identified     │                     │
│                    │   - DMU mapped           │                     │
│                    │   - Fit confirmed        │                     │
│                    └──────────────────────────┘                     │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│                    VALUE & ARGUMENTATION                            │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐  │
│  │   Value Selling  │  │      Sales       │  │   Competitive    │  │
│  │      Agent       │→ │  Argumentation   │→ │  Intelligence    │  │
│  │                  │  │      Agent       │  │      Agent       │  │
│  │ Quantify value   │  │ Tailor message   │  │ Differentiate    │  │
│  │ Build bus. case  │  │ per stakeholder  │  │ from competitors │  │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘  │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│                      PROPOSAL & CONTENT                             │
│         ┌──────────────────┐  ┌──────────────────┐                  │
│         │    Proposal      │  │  Sales Content   │                  │
│         │   Generation     │← │      Agent       │                  │
│         │      Agent       │  │                  │                  │
│         │ Create proposal  │  │ Supporting       │                  │
│         │ customized to    │  │ materials        │                  │
│         │ customer context │  │ and collateral   │                  │
│         └──────────────────┘  └──────────────────┘                  │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│                    DEAL MANAGEMENT & CLOSING                        │
│  ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐  │
│  │ Sales Process    │  │   Deal Risk      │  │ Deal Acceleration│  │
│  │  Coach Agent     │→ │   Management     │→ │      Agent       │  │
│  │                  │  │      Agent       │  │                  │  │
│  │ Next best action │  │ Identify risks   │  │ Accelerate close │  │
│  │ Real-time guide  │  │ Mitigate issues  │  │ Optimize velocity│  │
│  └──────────────────┘  └──────────────────┘  └──────────────────┘  │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
                    ┌──────────────────────────┐
                    │   Customer Handoff       │
                    │        Agent             │
                    │                          │
                    │   Smooth transition      │
                    │   to delivery/success    │
                    └──────────────────────────┘
                                    │
                                    ▼
                           ┌──────────────┐
                           │  CLOSED WON  │
                           └──────────────┘
```

## **Core Agents (10 agents)**

| \# | Agent | Function | Key Output |
| ----- | ----- | ----- | ----- |
| 1 | Value Selling Agent | Quantify customer-specific value | ROI calculations, business cases |
| 2 | Sales Argumentation Agent | Tailor messaging per stakeholder | Stakeholder-specific value arguments |
| 3 | Competitive Intelligence Agent | Differentiate from competition | Battle cards, competitive positioning |
| 4 | Proposal Generation Agent | Create customized proposals | Tailored proposals aligned to needs |
| 5 | Sales Content Agent | Provide supporting materials | Presentations, case studies, collateral |
| 6 | Sales Process Coach Agent | Guide next best actions | Real-time coaching, call preparation |
| 7 | Deal Risk Management Agent | Identify and mitigate risks | Risk scores, mitigation strategies |
| 8 | Deal Acceleration Agent | Speed up deal closure | Closing strategies, stakeholder engagement |
| 9 | Customer Handoff Agent | Ensure smooth transition | Handoff packages, implementation plans |

## **Key Metrics**

* Win rate (% of qualified opportunities won)  
* Sales cycle length (days from qualified to closed)  
* Average deal size  
* Proposal turnaround time  
* Forecast accuracy

## **Business Impact**

* **Higher win rates**: Better qualification \+ better execution  
* **Faster cycles**: Reduce time from qualified opportunity to close  
* **Larger deals**: Value-based selling increases deal size  
* **Consistent execution**: Every deal follows best practices  
* **Accurate forecasting**: Data-driven pipeline visibility

---

# **HOW THE TWO SYSTEMS CONNECT**

```
┌────────────────────────┐         ┌────────────────────────┐
│                        │         │                        │
│  OPPORTUNITY           │         │  OPPORTUNITY           │
│  GENERATION            │────────▶│  PURSUIT               │
│  ENGINE                │◀ ─ ─ ─ │  SYSTEM                │
│                        │ pull/  │                        │
│  Strategy → Qualified  │ stop   │  Qualified → Closed    │
│  Opportunity           │ signal │  Won                   │
│                        │         │                        │
│  7 agents              │         │  10 agents             │
│                        │         │                        │
└────────────────────────┘         └────────────────────────┘
         │         ▲                         │
         │         │ buffer                  │
         │         │ levels                  │
         ▼         │                         ▼
┌─────────────────────────────────────────────────────────────┐
│                    MANAGEMENT LAYER                         │
│                    (Shared across both systems)             │
│                                                             │
│  • Sales Operations Management Agent                        │
│    - Monitors constraint utilization & buffer levels        │
│    - Sends pull/stop signals to Generation Engine           │
│    - Calculates opportunity priority index                  │
│    - Enforces WIP limits per pipeline stage                 │
│  • Sales Analytics & Forecasting Agent                      │
│  • Performance Coaching Agent                               │
│  • Quality Assurance Agent                                  │
│  • Continuous Improvement Agent                             │
│                                                             │
│  5 agents providing oversight, analytics, and optimization  │
└─────────────────────────────────────────────────────────────┘
```

## **Flow Control Between Systems**

The two systems are not simply connected by a handoff — they are governed by a pull-based flow control mechanism managed by the Sales Operations Management Agent:

* **The Pursuit System signals its available capacity** (constraint units available, such as salesperson selling time slots) back to the Generation Engine via the Sales Operations Management Agent
* **The Generation Engine adjusts its output rate** based on this signal. When the Pursuit System's opportunity buffer is full, the Generation Engine reduces output. When buffer levels drop below threshold, the Generation Engine increases output.
* **The Qualification Agent uses buffer-level awareness** when routing: when the buffer is full, it applies stricter qualification thresholds and routes more opportunities to Lead Nurturing. When capacity opens up, it loosens thresholds and pulls from the nurture pool.
* **The Lead Nurturing Agent serves as the strategic buffer stock** between the two systems — not just a parking lot for unready leads, but a managed inventory of opportunities that can be released on pull signals when the Pursuit System has capacity.
* **Each qualified opportunity receives a priority index** calculated by the Sales Operations Management Agent, ensuring the constraint resource (typically the salesperson) always works the highest-yield opportunity next. The priority index factors deal value, win probability, remaining effort, and opportunity age.

This pull mechanism ensures that opportunity flow is synchronized with selling capacity — preventing both pipeline starvation and the waste of opportunities going cold in an overloaded queue.

## **Implementation Options**

| Option | What You Get | Best For |
| ----- | ----- | ----- |
| **Opportunity Generation Only** | Predictable pipeline of qualified opportunities | Companies with strong sales execution but weak pipeline |
| **Opportunity Pursuit Only** | Consistent, high-quality deal execution | Companies with enough opportunities but low win rates |
| **Both Systems** | End-to-end sales transformation | Companies seeking full sales optimization |
| **Selected Agents** | Targeted capability improvement | Companies with specific pain points |

---

# **EXPAND WORKFLOW: Detailed Example**

## **Use Case: Growing Revenue from Existing Customers (Upsell \+ Cross-sell)**

This workflow shows how selected agents work together to systematically identify and capture expansion opportunities within your current customer base.

## **Why This Workflow?**

* **Highest ROI**: Selling to existing customers costs 5-25x less than acquiring new ones  
* **Fastest time to value**: Relationships exist, trust is established  
* **Proves the system**: Quick wins demonstrate agentic AI value before tackling harder problems

## **The Expand Workflow**

### **Phase 1: Identify Expansion Opportunities**

```
┌─────────────────────────────────────────────────────────────────────┐
│  ACCOUNT PLANNING AGENT                                             │
│                                                                     │
│  Inputs:                                                            │
│  • Customer data from CRM (revenue, products, engagement)           │
│  • Usage data (if available)                                        │
│  • Contract renewal dates                                           │
│  • Organizational changes (new hires, restructuring)                │
│                                                                     │
│  Activities:                                                        │
│  • Analyze whitespace: what else could this customer buy?           │
│  • Score expansion potential by account                             │
│  • Identify trigger events (growth signals, pain indicators)        │
│  • Map additional stakeholders not yet engaged                      │
│                                                                     │
│  Outputs:                                                           │
│  • Prioritized list of expansion opportunities                      │
│  • Account-specific expansion strategies                            │
│  • Recommended offerings per account                                │
│  • Stakeholder map updates                                          │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output:**

"Acme Corp is using our basic analytics package. They've hired 3 new data scientists in Q3, expanded their BI team, and their contract renews in 90 days. Whitespace analysis shows 85% fit for our Advanced Analytics Suite. Expansion potential: €150K ARR. Priority: High. Recommended action: Discovery conversation with new VP of Data (hired 60 days ago)."

---

### **Phase 2: Discovery & Qualification**

```
┌─────────────────────────────────────────────────────────────────────┐
│  DISCOVERY AGENT                                                    │
│                                                                     │
│  Inputs:                                                            │
│  • Account Planning Agent expansion recommendations                 │
│  • Existing customer context and history                            │
│  • Current solution usage and satisfaction data                     │
│                                                                     │
│  Activities:                                                        │
│  • Generate discovery questions tailored to expansion opportunity   │
│  • Identify new stakeholders and their priorities                   │
│  • Map decision-making unit for expansion purchase                  │
│  • Assess urgency and timeline for expansion                        │
│                                                                     │
│  Outputs:                                                           │
│  • Updated needs analysis for expansion scope                       │
│  • New DMU map (who decides on expansion?)                          │
│  • Buying process for expansion vs. new purchase                    │
│  • Stakeholder-specific priorities and concerns                     │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  QUALIFICATION AGENT                                                │
│                                                                     │
│  Inputs:                                                            │
│  • Discovery findings                                               │
│  • Historical win/loss data for expansion deals                     │
│  • Account health metrics                                           │
│                                                                     │
│  Activities:                                                        │
│  • Score expansion opportunity against qualification criteria       │
│  • Assess competitive risk (are they looking at alternatives?)      │
│  • Evaluate timing alignment with budget cycles                     │
│  • Calculate probability-weighted pipeline value                    │
│                                                                     │
│  Outputs:                                                           │
│  • Go/No-go recommendation with rationale                           │
│  • Opportunity score and win probability                            │
│  • Risk factors and mitigation recommendations                      │
│  • Resource allocation recommendation                               │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output:**

"Acme Corp expansion QUALIFIED (Score: 78/100)

* Budget: Confirmed, VP Data has discretionary budget up to €200K  
* Authority: VP Data is economic buyer, needs CFO sign-off above €100K  
* Need: Validated — current solution limiting their ML initiatives  
* Timeline: Want decision before contract renewal (90 days)  
* Competition: Low risk — switching costs high, satisfaction with current solution  
* Recommendation: PURSUE — assign senior account manager"

---

### **Phase 3: Value Development**

```
┌─────────────────────────────────────────────────────────────────────┐
│  VALUE SELLING AGENT                                                │
│                                                                     │
│  Inputs:                                                            │
│  • Discovery findings (needs, current state, desired outcomes)      │
│  • Customer's actual usage data and results                         │
│  • Industry benchmarks and similar customer outcomes                │
│                                                                     │
│  Activities:                                                        │
│  • Calculate ROI based on customer-specific data                    │
│  • Quantify cost of status quo (what are they losing by not         │
│    expanding?)                                                      │
│  • Model scenarios: basic vs. advanced adoption                     │
│  • Develop CFO-ready business case                                  │
│                                                                     │
│  Outputs:                                                           │
│  • Customer-specific ROI calculation                                │
│  • Business case document                                           │
│  • Value realization timeline                                       │
│  • Success metrics and measurement plan                             │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output:**

"Acme Corp Value Analysis:

* Current state: 3 data scientists spending 40% of time on data prep  
* With Advanced Analytics Suite: Reduce data prep to 15%  
* Value: 2,400 hours/year recovered × €85/hour \= €204,000 annual value  
* Investment: €150,000 ARR  
* ROI: 136% Year 1, payback in 8.8 months  
* Additional value: Faster time-to-insight enables 2 additional ML projects/quarter"

---

### **Phase 4: Tailored Argumentation**

```
┌─────────────────────────────────────────────────────────────────────┐
│  SALES ARGUMENTATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • Value Selling Agent outputs (ROI, business case)                 │
│  • DMU mapping (who needs what message)                             │
│  • Stakeholder priorities from Discovery                            │
│                                                                     │
│  Activities:                                                        │
│  • Create VP Data messaging (productivity, team capability)         │
│  • Create CFO messaging (ROI, cost avoidance, risk)                 │
│  • Create Data Scientist messaging (features, ease of use)          │
│  • Develop objection handling for each stakeholder                  │
│                                                                     │
│  Outputs:                                                           │
│  • Stakeholder-specific talk tracks                                 │
│  • Email templates per stakeholder                                  │
│  • Presentation decks tailored to audience                          │
│  • Objection handling scripts                                       │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output:**

**For VP Data (Economic Buyer):**

"Your team is spending 40% of their time on data prep instead of building models. That's 2,400 hours per year of your most expensive talent doing work that should be automated. Our Advanced Analytics Suite cuts that to 15%, giving you the equivalent of 1.2 additional data scientists without hiring. That's €204K in recovered productivity — more than covering the €150K investment in year one."

**For CFO (Approver):**

"This is a productivity investment with 8.8-month payback. The €150K investment recovers €204K in year one through reduced data preparation time. It also de-risks your ML initiatives — right now they're delayed because the team is capacity-constrained. Faster time-to-insight means faster time-to-value on your data strategy."

**For Data Scientists (Users):**

"You'll get automated data pipelines, pre-built connectors to your existing stack, and a feature store that eliminates redundant work across projects. Other teams using this report spending 60% less time on data prep and 40% more time on actual modeling."

---

### **Phase 5: Proposal & Close**

```
┌─────────────────────────────────────────────────────────────────────┐
│  PROPOSAL GENERATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • All outputs from Value Selling and Sales Argumentation           │
│  • Offering Configuration (pricing, packaging, terms)               │
│  • Customer-specific requirements from Discovery                    │
│                                                                     │
│  Activities:                                                        │
│  • Generate customized proposal document                            │
│  • Include customer-specific business case and ROI                  │
│  • Align pricing with value delivered                               │
│  • Include implementation timeline and success metrics              │
│                                                                     │
│  Outputs:                                                           │
│  • Complete proposal document                                       │
│  • Executive summary for CFO                                        │
│  • Technical appendix for data team                                 │
│  • Contract terms aligned with renewal timeline                     │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  DEAL ACCELERATION AGENT                                            │
│                                                                     │
│  Inputs:                                                            │
│  • Deal status and timeline                                         │
│  • Stakeholder engagement tracking                                  │
│  • Contract renewal deadline                                        │
│                                                                     │
│  Activities:                                                        │
│  • Monitor deal velocity against benchmarks                         │
│  • Identify stalled stakeholders and recommend re-engagement        │
│  • Optimize timing of proposal delivery and follow-up               │
│  • Recommend closing incentives if needed                           │
│                                                                     │
│  Outputs:                                                           │
│  • Daily/weekly deal status updates                                 │
│  • Recommended actions to accelerate                                │
│  • Closing strategy adjustments                                     │
│  • Final negotiation guidance                                       │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
                           ┌──────────────┐
                           │ EXPANSION    │
                           │ CLOSED WON   │
                           │              │
                           │ €150K ARR    │
                           │ added        │
                           └──────────────┘
```

---

## **Expand Workflow: Agent Summary**

| Agent | Role in Expand Workflow |
| ----- | ----- |
| Account Planning Agent | Identifies which customers have expansion potential |
| Discovery Agent | Validates expansion needs and maps new stakeholders |
| Qualification Agent | Scores opportunity and recommends go/no-go |
| Value Selling Agent | Quantifies customer-specific ROI and builds business case |
| Sales Argumentation Agent | Tailors messaging for each stakeholder in the DMU |
| Proposal Generation Agent | Creates customized expansion proposal |
| Deal Acceleration Agent | Monitors progress and accelerates closing |

**7 agents working together to systematically capture expansion revenue.**

---

## **Business Impact of Expand Workflow**

| Metric | Without Agentic System | With Agentic System | Impact |
| ----- | ----- | ----- | ----- |
| Expansion opportunities identified | Ad hoc, salesperson-dependent | Systematic, data-driven | 3-5x more opportunities surfaced |
| Time to create business case | 4-8 hours per opportunity | 30 minutes | 90% faster |
| Stakeholder coverage | Often single-threaded | Multi-threaded by design | Higher win rate |
| Proposal turnaround | 2-5 days | Same day | Faster cycle |
| Win rate on expansion | 30-40% | 50-60% | \+50% improvement |

---

## **Why Start with Expand?**

1. **Existing relationships reduce risk** — you're not testing with prospects, you're testing with customers who already trust you

2. **Data is available** — you have CRM data, usage data, and relationship history to work with

3. **Quick wins build momentum** — closing an expansion deal in 30-60 days proves the system works

4. **Learns your context** — the agents learn your offerings, customers, and winning patterns before you apply them to harder problems (new customer acquisition)

5. **Funds further investment** — expansion revenue can fund the buildout of opportunity generation for new customers

---

# **ACQUIRE WORKFLOW: Detailed Example**

## **Use Case: Winning New Customers (New Customer Acquisition \+ Displacement Plays)**

This workflow shows how selected agents work together to systematically identify, engage, and win new customers — including taking customers from competitors.

## **Why This Workflow?**

* **Core growth engine**: Most companies need new customer acquisition to hit growth targets  
* **Most common need**: "We need more pipeline" is the \#1 sales complaint  
* **Competitive necessity**: If you're not acquiring, competitors are taking share

## **The Acquire Workflow**

### **Phase 1: Market & Target Identification**

```
┌─────────────────────────────────────────────────────────────────────┐
│  STRATEGIC MARKET INTELLIGENCE AGENT                                │
│                                                                     │
│  Inputs:                                                            │
│  • Market data, industry reports, news feeds                        │
│  • Competitor customer lists and case studies                       │
│  • Technology adoption signals (job postings, tech stack data)      │
│  • Economic indicators and industry trends                          │
│                                                                     │
│  Activities:                                                        │
│  • Identify market segments with highest growth potential           │
│  • Track competitor vulnerabilities (pricing changes, service       │
│    issues, product gaps)                                            │
│  • Detect category shifts creating switching opportunities          │
│  • Monitor trigger events (M&A, leadership changes, funding)        │
│                                                                     │
│  Outputs:                                                           │
│  • Market opportunity assessment                                    │
│  • Competitor vulnerability report                                  │
│  • Target segment recommendations                                   │
│  • Trigger event alerts                                             │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  SEGMENT STRATEGY AGENT                                             │
│                                                                     │
│  Inputs:                                                            │
│  • Market intelligence outputs                                      │
│  • Historical win/loss data by segment                              │
│  • Capacity and resource constraints                                │
│  • Strategic priorities from leadership                             │
│                                                                     │
│  Activities:                                                        │
│  • Define ICP criteria for new customer acquisition                 │
│  • Prioritize segments based on fit and win probability             │
│  • Set targeting rules: who to pursue, who to avoid                 │
│  • Allocate resources across acquisition segments                   │
│                                                                     │
│  Outputs:                                                           │
│  • ICP definitions with scoring criteria                            │
│  • Segment priority rankings                                        │
│  • Target account lists by segment                                  │
│  • Resource allocation recommendations                              │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output:**

"Mid-market manufacturing segment (500-2000 employees) shows highest acquisition potential:

* 340 companies in territory matching ICP  
* Competitor X raised prices 15% last quarter — 45 accounts showing dissatisfaction signals  
* Industry trend: 67% planning digital transformation investment in next 12 months  
* Our win rate in this segment: 34% (vs. 22% overall)  
* Recommended focus: 45 displacement targets \+ 60 greenfield accounts  
* Resource allocation: 2 dedicated hunters \+ SDR support"

---

### **Phase 2: Prospect Research & Outreach**

```
┌─────────────────────────────────────────────────────────────────────┐
│  PROSPECT INTELLIGENCE AGENT                                        │
│                                                                     │
│  Inputs:                                                            │
│  • Target account lists from Segment Strategy                       │
│  • Company databases (LinkedIn, ZoomInfo, etc.)                     │
│  • News and social media monitoring                                 │
│  • Technology stack data                                            │
│                                                                     │
│  Activities:                                                        │
│  • Research each target account in depth                            │
│  • Identify key stakeholders and reporting structures               │
│  • Detect buying signals and trigger events                         │
│  • Assess current vendor relationships and contract timing          │
│  • Score accounts by engagement readiness                           │
│                                                                     │
│  Outputs:                                                           │
│  • Detailed account profiles                                        │
│  • Stakeholder maps with contact information                        │
│  • Buying signal scores                                             │
│  • Recommended engagement timing                                    │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  OUTREACH AUTOMATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • Account profiles and stakeholder data                            │
│  • Segment-specific messaging from Value Proposition Agent          │
│  • Buying signal scores and timing recommendations                  │
│  • Channel preferences by persona                                   │
│                                                                     │
│  Activities:                                                        │
│  • Generate personalized outreach sequences                         │
│  • Execute multi-channel campaigns (email, LinkedIn, phone)         │
│  • A/B test messaging variations                                    │
│  • Track engagement and optimize timing                             │
│  • Identify and escalate hot responses                              │
│                                                                     │
│  Outputs:                                                           │
│  • Personalized outreach messages                                   │
│  • Engagement tracking and scoring                                  │
│  • Response categorization                                          │
│  • Meeting-ready leads for Discovery                                │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output (Displacement Target):**

"Outreach to Nordic Manufacturing AB:

**Account Context:** €50M revenue, 800 employees, currently using Competitor X for 3 years. Contract renewal in 6 months. Posted 2 negative reviews about Competitor X support on G2 last quarter. New VP Operations hired 90 days ago.

**Personalized Email to VP Operations:** 'Saw you joined Nordic Manufacturing from \[Previous Company\]. At \[Previous Company\], your ops team was known for cutting production downtime by 30%. Nordic's current setup with \[Competitor X\] likely isn't giving you the real-time visibility you had before.

We helped \[Similar Company\] make that transition — they cut unplanned downtime by 40% in the first 6 months.

Worth a 20-minute call to see if there's a fit?'

**Sequence:** Email Day 1 → LinkedIn connect Day 3 → Follow-up email Day 7 → Phone Day 10"

---

### **Phase 3: Discovery & Qualification**

```
┌─────────────────────────────────────────────────────────────────────┐
│  DISCOVERY AGENT                                                    │
│                                                                     │
│  Inputs:                                                            │
│  • Engaged prospects from Outreach                                  │
│  • Account research from Prospect Intelligence                      │
│  • Competitive intelligence on current vendor                       │
│                                                                     │
│  Activities:                                                        │
│  • Conduct structured discovery conversations                       │
│  • Identify pain points with current solution/vendor                │
│  • Map decision-making unit and buying process                      │
│  • Understand switching barriers and concerns                       │
│  • Assess timeline and urgency                                      │
│                                                                     │
│  Outputs:                                                           │
│  • Needs analysis (current state, desired state, gap)               │
│  • DMU map with influence levels                                    │
│  • Switching barrier assessment                                     │
│  • Competitive displacement strategy inputs                         │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  QUALIFICATION AGENT                                                │
│                                                                     │
│  Inputs:                                                            │
│  • Discovery findings                                               │
│  • Historical win/loss data for similar deals                       │
│  • Competitive displacement success patterns                        │
│                                                                     │
│  Activities:                                                        │
│  • Score opportunity against acquisition criteria                   │
│  • Assess competitive win probability                               │
│  • Evaluate switching cost vs. value gap                            │
│  • Identify deal-breaker risks                                      │
│                                                                     │
│  Outputs:                                                           │
│  • Go/No-go recommendation                                          │
│  • Win probability score                                            │
│  • Competitive strategy recommendation                              │
│  • Resource investment recommendation                               │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                          ┌─────────┴─────────┐
                          ▼                   ▼
                   ┌────────────┐      ┌────────────┐
                   │  QUALIFIED │      │    LEAD    │
                   │  Continue  │      │  NURTURING │
                   │  to Value  │      │   Not yet  │
                   │  Selling   │      │   ready    │
                   └────────────┘      └────────────┘
```

**Example Output:**

"Nordic Manufacturing AB — QUALIFIED (Score: 72/100)

**Strengths:**

* Clear pain with current vendor (support issues documented)  
* New VP Operations is change agent with mandate to improve  
* Contract renewal creates natural switching window  
* Budget confirmed at €200K range

**Risks:**

* CFO is risk-averse, concerned about migration disruption  
* IT team has relationship with Competitor X account manager  
* 3-year historical data migration required

**Recommendation:** PURSUE with displacement strategy

* Lead with risk mitigation and migration support  
* Engage CFO early with ROI business case  
* Offer proof-of-concept to reduce perceived risk  
* Target decision before contract auto-renewal (5 months)"

---

### **Phase 4: Competitive Value Development**

```
┌─────────────────────────────────────────────────────────────────────┐
│  COMPETITIVE INTELLIGENCE AGENT                                     │
│                                                                     │
│  Inputs:                                                            │
│  • Current vendor identified (Competitor X)                         │
│  • Discovery findings on pain points                                │
│  • Market intelligence on competitor                                │
│                                                                     │
│  Activities:                                                        │
│  • Analyze competitor's specific weaknesses in this account         │
│  • Identify proof points from similar displacement wins             │
│  • Develop counter-positioning for competitor strengths             │
│  • Prepare objection handling for switching concerns                │
│                                                                     │
│  Outputs:                                                           │
│  • Account-specific competitive battle card                         │
│  • Displacement proof points and references                         │
│  • Objection handling for switching barriers                        │
│  • Competitive trap-setting questions                               │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  VALUE SELLING AGENT                                                │
│                                                                     │
│  Inputs:                                                            │
│  • Discovery findings                                               │
│  • Competitive intelligence                                         │
│  • Switching cost estimates                                         │
│                                                                     │
│  Activities:                                                        │
│  • Calculate total cost of ownership vs. current vendor             │
│  • Quantify cost of status quo (ongoing pain)                       │
│  • Model switching ROI including migration costs                    │
│  • Develop risk-adjusted business case                              │
│                                                                     │
│  Outputs:                                                           │
│  • Competitive TCO comparison                                       │
│  • Cost of inaction analysis                                        │
│  • Migration ROI model                                              │
│  • CFO-ready business case                                          │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  SALES ARGUMENTATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • Value Selling outputs                                            │
│  • Competitive positioning                                          │
│  • DMU map and stakeholder concerns                                 │
│                                                                     │
│  Activities:                                                        │
│  • Create displacement messaging per stakeholder                    │
│  • Address switching fears for risk-averse stakeholders             │
│  • Develop "why change now" urgency arguments                       │
│  • Prepare internal champion enablement materials                   │
│                                                                     │
│  Outputs:                                                           │
│  • Stakeholder-specific displacement arguments                      │
│  • Risk mitigation messaging for CFO                                │
│  • Champion enablement toolkit                                      │
│  • "Why us vs. Competitor X" talk tracks                            │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output:**

**Competitive Battle Card (vs. Competitor X at Nordic Manufacturing):**

**Their weakness:** Support response time averaging 48 hours (Nordic experiencing this pain) **Our strength:** 4-hour SLA with dedicated CSM — reference: Similar Company resolved critical issue in 2 hours

**Their weakness:** No real-time production visibility **Our strength:** Live dashboard with predictive alerts — reference: \[Customer\] caught equipment failure 6 hours before breakdown

**Switching objection:** "Migration is risky and disruptive" **Our response:** "We've done 40+ migrations from Competitor X. Average migration time: 6 weeks. We run parallel systems until you're 100% confident. \[Reference Customer\] had zero production impact during switchover."

**For CFO (Risk-Averse Approver):**

"I understand the concern about switching costs. Let me share the full picture:

* Current annual cost with Competitor X: €180K \+ estimated €95K in downtime costs from slow support response  
* Our solution: €200K annually with 4-hour support SLA  
* Net year-one impact: \-€75K (savings)  
* Migration cost: €40K (one-time)  
* Payback on migration investment: 6 months

More importantly, three companies your size made this exact switch last year. Happy to connect you with their CFOs."

---

### **Phase 5: Proposal & Close**

```
┌─────────────────────────────────────────────────────────────────────┐
│  PROPOSAL GENERATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • Value Selling outputs (TCO comparison, ROI)                      │
│  • Competitive positioning                                          │
│  • Migration requirements from Discovery                            │
│  • Offering configuration and pricing                               │
│                                                                     │
│  Activities:                                                        │
│  • Generate displacement-focused proposal                           │
│  • Include migration plan and timeline                              │
│  • Incorporate risk mitigation elements                             │
│  • Structure pricing to ease switching decision                     │
│                                                                     │
│  Outputs:                                                           │
│  • Complete proposal with migration plan                            │
│  • Executive summary for CFO                                        │
│  • Technical migration appendix                                     │
│  • Reference customer contacts                                      │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  DEAL ACCELERATION AGENT                                            │
│                                                                     │
│  Inputs:                                                            │
│  • Deal status and competitor activity                              │
│  • Contract renewal deadline                                        │
│  • Stakeholder engagement levels                                    │
│                                                                     │
│  Activities:                                                        │
│  • Create urgency around contract renewal window                    │
│  • Monitor for competitive counter-moves                            │
│  • Orchestrate reference calls and site visits                      │
│  • Recommend closing incentives if needed                           │
│                                                                     │
│  Outputs:                                                           │
│  • Closing timeline and action plan                                 │
│  • Competitive response strategies                                  │
│  • Final negotiation guidance                                       │
│  • Contract terms optimization                                      │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
                           ┌──────────────┐
                           │   NEW        │
                           │   CUSTOMER   │
                           │   WON        │
                           │              │
                           │   €200K ARR  │
                           │   acquired   │
                           └──────────────┘
```

---

## **Acquire Workflow: Agent Summary**

| Agent | Role in Acquire Workflow |
| ----- | ----- |
| Strategic Market Intelligence Agent | Identifies market opportunities and competitor vulnerabilities |
| Segment Strategy Agent | Defines ICPs and prioritizes target segments |
| Prospect Intelligence Agent | Researches target accounts and identifies stakeholders |
| Outreach Automation Agent | Executes personalized multi-channel outreach |
| Discovery Agent | Validates needs and maps decision-making unit |
| Qualification Agent | Scores opportunity and recommends go/no-go |
| Competitive Intelligence Agent | Develops displacement strategy and battle cards |
| Value Selling Agent | Builds competitive TCO and switching ROI |
| Sales Argumentation Agent | Creates stakeholder-specific displacement messaging |
| Proposal Generation Agent | Creates proposal with migration plan |
| Deal Acceleration Agent | Drives closing against contract renewal deadline |
| Lead Nurturing Agent | Maintains not-yet-ready prospects |

**12 agents working together to systematically acquire new customers.**

---

## **Business Impact of Acquire Workflow**

| Metric | Without Agentic System | With Agentic System | Impact |
| ----- | ----- | ----- | ----- |
| Target accounts researched/month | 20-30 (manual) | 200+ (automated) | 10x coverage |
| Personalized outreach per rep/day | 10-15 | 50-100 | 5x activity |
| Response rate | 2-5% | 8-15% | 3x engagement |
| Competitive win rate | 25-30% | 40-50% | \+60% improvement |
| Time to build competitive business case | 1-2 days | 2 hours | 80% faster |
| New customers acquired/quarter | Baseline | \+40-60% | Significant growth |

---

# **ENTER WORKFLOW: Detailed Example**

## **Use Case: Entering New Markets (New Market Penetration \+ New Market Entry \+ Category Shifts)**

This workflow shows how selected agents work together to systematically enter new markets where you have limited presence, relationships, or brand recognition.

## **Why This Workflow?**

* **Strategic growth**: Sometimes existing markets are saturated or declining  
* **Diversification**: Reduce dependence on single market or segment  
* **Opportunity capture**: Category shifts and technology changes create windows

## **Key Differences from Acquire**

| Aspect | Acquire | Enter |
| ----- | ----- | ----- |
| Brand awareness | Known in market | Unknown or limited |
| References | Have relevant case studies | May lack segment-specific proof |
| ICP confidence | Validated | Hypothesis to test |
| Sales cycle | Predictable | Longer, more uncertain |
| Competitive position | Understood | Learning |

## **The Enter Workflow**

### **Phase 1: Market Analysis & Strategy**

```
┌─────────────────────────────────────────────────────────────────────┐
│  STRATEGIC MARKET INTELLIGENCE AGENT                                │
│                                                                     │
│  Inputs:                                                            │
│  • Target market definition (geography, industry, segment)          │
│  • Market research and industry reports                             │
│  • Competitive landscape in new market                              │
│  • Regulatory and compliance requirements                           │
│                                                                     │
│  Activities:                                                        │
│  • Size the addressable market opportunity                          │
│  • Map competitive landscape (who are the incumbents?)              │
│  • Identify market-specific buying patterns and cycles              │
│  • Detect entry timing signals (category shifts, disruption)        │
│  • Assess barriers to entry and success factors                     │
│                                                                     │
│  Outputs:                                                           │
│  • Market size and growth assessment                                │
│  • Competitive landscape map                                        │
│  • Entry barrier analysis                                           │
│  • Timing and readiness assessment                                  │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  SEGMENT STRATEGY AGENT                                             │
│                                                                     │
│  Inputs:                                                            │
│  • Market intelligence outputs                                      │
│  • Company capabilities and adjacencies                             │
│  • Resource availability for market entry                           │
│                                                                     │
│  Activities:                                                        │
│  • Define beachhead segment (where to start)                        │
│  • Create hypothesis ICP for new market                             │
│  • Identify potential lighthouse/reference customers                │
│  • Set realistic penetration targets and timeline                   │
│                                                                     │
│  Outputs:                                                           │
│  • Beachhead segment definition                                     │
│  • Hypothesis ICP (to be validated)                                 │
│  • Target lighthouse account list                                   │
│  • Market entry plan and milestones                                 │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  VALUE PROPOSITION OPTIMIZATION AGENT                               │
│                                                                     │
│  Inputs:                                                            │
│  • Segment strategy outputs                                         │
│  • Existing value propositions from other markets                   │
│  • New market-specific pain points and priorities                   │
│  • Competitive positioning in new market                            │
│                                                                     │
│  Activities:                                                        │
│  • Adapt value propositions for new market context                  │
│  • Identify messaging gaps (what resonates here?)                   │
│  • Create hypothesis messaging to test                              │
│  • Develop market-specific proof points and analogies               │
│                                                                     │
│  Outputs:                                                           │
│  • Market-adapted value propositions                                │
│  • Hypothesis messaging for testing                                 │
│  • Proof point substitutes (adjacent references)                    │
│  • Messaging test plan                                              │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  OFFERING CONFIGURATION AGENT                                       │
│                                                                     │
│  Inputs:                                                            │
│  • Market-specific requirements                                     │
│  • Competitive offering analysis                                    │
│  • Pricing expectations in new market                               │
│  • Entry strategy (penetration vs. premium)                         │
│                                                                     │
│  Activities:                                                        │
│  • Configure offering for new market requirements                   │
│  • Develop market entry pricing and packaging                       │
│  • Create pilot/POC offerings to reduce buyer risk                  │
│  • Define success metrics for market entry deals                    │
│                                                                     │
│  Outputs:                                                           │
│  • Market-specific offering configuration                           │
│  • Entry pricing and packaging                                      │
│  • Pilot program structure                                          │
│  • Reference deal economics                                         │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output (Healthcare Market Entry):**

"Healthcare Vertical Entry Assessment:

**Market Opportunity:**

* TAM: €2.4B for our solution category in European healthcare  
* Current penetration: 0% (no healthcare customers)  
* Market growth: 12% CAGR driven by digital health mandates

**Competitive Landscape:**

* Incumbent A: 45% share, strong but expensive, slow innovation  
* Incumbent B: 30% share, good product, weak services  
* Gap: No strong player combining our automation \+ compliance capabilities

**Beachhead Strategy:**

* Start with: Private hospital groups (500-2000 beds)  
* Why: Faster decisions than public sector, similar pain points to our existing customers  
* Hypothesis ICP: Private hospital group, €100M+ revenue, undergoing digital transformation  
* Target lighthouse accounts: 5 specific hospital groups identified

**Entry Offering:**

* Pilot program: 90-day POC at 50% of standard pricing  
* Success metrics: Defined upfront, convert to full contract if met  
* Reference commitment: Lighthouse customers agree to be references if successful"

---

### **Phase 2: Beachhead Targeting & Outreach**

```
┌─────────────────────────────────────────────────────────────────────┐
│  PROSPECT INTELLIGENCE AGENT                                        │
│                                                                     │
│  Inputs:                                                            │
│  • Lighthouse target list from Segment Strategy                     │
│  • Market-specific research sources                                 │
│  • Industry events and conferences                                  │
│                                                                     │
│  Activities:                                                        │
│  • Deep research on lighthouse targets                              │
│  • Identify innovation leaders and early adopters                   │
│  • Map industry relationships and influence networks                │
│  • Find warm introduction paths (investors, advisors, partners)     │
│  • Track industry events for engagement opportunities               │
│                                                                     │
│  Outputs:                                                           │
│  • Detailed lighthouse account profiles                             │
│  • Early adopter identification                                     │
│  • Relationship mapping and intro paths                             │
│  • Event-based engagement opportunities                             │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  OUTREACH AUTOMATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • Lighthouse account profiles                                      │
│  • Market-adapted messaging                                         │
│  • Entry offer (pilot program)                                      │
│                                                                     │
│  Activities:                                                        │
│  • Create thought leadership-led outreach (not sales-led)           │
│  • Engage around industry challenges, not product features          │
│  • Leverage adjacent references and analogies                       │
│  • Test messaging variations to learn what resonates                │
│  • Build awareness before pushing for meetings                      │
│                                                                     │
│  Outputs:                                                           │
│  • Thought leadership outreach sequences                            │
│  • Messaging performance data (what resonates?)                     │
│  • Engaged prospects for Discovery                                  │
│  • Market learning insights                                         │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output (Healthcare Outreach):**

"Lighthouse Outreach Strategy for MedGroup (Private Hospital Chain):

**Why MedGroup:**

* 12 hospitals, €450M revenue, announced 'Digital Patient Journey' initiative  
* New CIO hired from retail (brings outside perspective)  
* Published article complaining about legacy system integration challenges

**Outreach Approach (Thought Leadership-Led):**

**Week 1-2:** Share content, build awareness

* Connect with CIO on LinkedIn  
* Share relevant article: 'How Retail-Experienced Leaders Are Transforming Healthcare Operations'  
* Comment thoughtfully on their Digital Patient Journey announcement

**Week 3:** Problem-focused outreach

* Email: 'We've helped organizations in \[adjacent industry\] solve the integration challenges you mentioned in \[article\]. The patterns are surprisingly similar. Would you be open to a 20-minute call to share what we've learned?'

**Week 4:** Value-add follow-up

* Share case study from adjacent industry (manufacturing → healthcare analogy)  
* Offer: 'Happy to walk through how \[Company\] approached this — no pitch, just sharing what worked.'

**Goal:** Earn a discovery conversation, not sell a product"

---

### **Phase 3: Discovery & Validation**

```
┌─────────────────────────────────────────────────────────────────────┐
│  DISCOVERY AGENT                                                    │
│                                                                     │
│  Inputs:                                                            │
│  • Engaged lighthouse prospects                                     │
│  • Market hypotheses to validate                                    │
│  • Adjacent market knowledge                                        │
│                                                                     │
│  Activities:                                                        │
│  • Conduct discovery with learning mindset (validate hypotheses)    │
│  • Identify market-specific needs and language                      │
│  • Map decision-making process in this market                       │
│  • Understand regulatory and compliance requirements                │
│  • Learn competitive dynamics from buyer perspective                │
│                                                                     │
│  Outputs:                                                           │
│  • Validated/refined ICP                                            │
│  • Market-specific needs and language                               │
│  • Buying process insights for this market                          │
│  • Competitive intelligence from buyer perspective                  │
│  • Go-to-market refinements                                         │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  QUALIFICATION AGENT                                                │
│                                                                     │
│  Inputs:                                                            │
│  • Discovery findings                                               │
│  • Market entry criteria (lighthouse potential)                     │
│  • Reference value assessment                                       │
│                                                                     │
│  Activities:                                                        │
│  • Evaluate opportunity against market entry goals                  │
│  • Assess lighthouse potential (will they be a reference?)          │
│  • Evaluate learning value even if deal doesn't close               │
│  • Balance revenue value vs. strategic value                        │
│                                                                     │
│  Outputs:                                                           │
│  • Go/No-go with strategic rationale                                │
│  • Lighthouse score (reference potential)                           │
│  • Deal structure recommendation (pilot vs. full)                   │
│  • Market learning capture                                          │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
```

**Example Output:**

"MedGroup Discovery Findings:

**ICP Validation:** ✓ Confirmed

* Digital transformation mandate is real (board-level priority)  
* Budget allocated for 2024-2025  
* Pain points match our hypothesis (integration, automation)

**Market Learning:**

* Compliance requirements: Need HIPAA-equivalent EU certification (we have it)  
* Buying process: Longer than expected (6-9 months), requires clinical sign-off  
* Language: 'Patient journey' not 'customer experience', 'care pathway' not 'workflow'  
* Incumbent weakness: Competitor A is slow to implement, taking 12-18 months

**Lighthouse Assessment:** HIGH VALUE

* CIO is well-connected in healthcare CIO community  
* They speak at conferences and publish articles  
* Explicit willingness to be reference if we deliver results

**Recommendation:** PURSUE as lighthouse

* Accept lower margin on first deal for reference value  
* Propose 90-day pilot with defined success criteria  
* Build case study into contract terms"

---

### **Phase 4: Value Development & Proposal**

```
┌─────────────────────────────────────────────────────────────────────┐
│  VALUE SELLING AGENT                                                │
│                                                                     │
│  Inputs:                                                            │
│  • Discovery findings with market-specific needs                    │
│  • Adjacent market proof points                                     │
│  • Pilot program structure                                          │
│                                                                     │
│  Activities:                                                        │
│  • Adapt ROI models for healthcare context                          │
│  • Translate adjacent proof points to healthcare metrics            │
│  • Build pilot success criteria with measurable outcomes            │
│  • Create healthcare-specific business case                         │
│                                                                     │
│  Outputs:                                                           │
│  • Healthcare-context ROI model                                     │
│  • Pilot success criteria and metrics                               │
│  • Business case with healthcare benchmarks                         │
│  • Risk mitigation through pilot structure                          │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  SALES ARGUMENTATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • Value Selling outputs                                            │
│  • Healthcare-specific language and concerns                        │
│  • DMU map (clinical + operational + IT stakeholders)               │
│                                                                     │
│  Activities:                                                        │
│  • Create stakeholder messaging in healthcare language              │
│  • Address "no healthcare references" objection                     │
│  • Develop clinical stakeholder arguments (patient outcomes)        │
│  • Build pilot as risk mitigation for unproven vendor               │
│                                                                     │
│  Outputs:                                                           │
│  • Healthcare-specific talk tracks                                  │
│  • "New to healthcare" objection handling                           │
│  • Clinical stakeholder value arguments                             │
│  • Pilot-as-proof positioning                                       │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
┌─────────────────────────────────────────────────────────────────────┐
│  PROPOSAL GENERATION AGENT                                          │
│                                                                     │
│  Inputs:                                                            │
│  • All value development outputs                                    │
│  • Pilot program structure and pricing                              │
│  • Reference commitment terms                                       │
│                                                                     │
│  Activities:                                                        │
│  • Create pilot-focused proposal                                    │
│  • Include clear success criteria and decision points               │
│  • Build in reference commitment terms                              │
│  • Structure path from pilot to full deployment                     │
│                                                                     │
│  Outputs:                                                           │
│  • Pilot proposal with success criteria                             │
│  • Full deployment roadmap and pricing                              │
│  • Reference agreement terms                                        │
│  • Risk mitigation summary                                          │
└─────────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
                           ┌──────────────┐
                           │  LIGHTHOUSE  │
                           │  CUSTOMER    │
                           │  WON         │
                           │              │
                           │  Opens new   │
                           │  market      │
                           └──────────────┘
                                    │
                                    ▼
                    ┌──────────────────────────┐
                    │  Feed learnings back to  │
                    │  Strategy Layer agents   │
                    │  for market scaling      │
                    └──────────────────────────┘
```

**Example Output (Healthcare Pilot Proposal):**

"MedGroup Pilot Proposal Summary:

**Pilot Scope:** Patient intake automation across 2 pilot hospitals (90 days)

**Success Criteria:**

* Reduce patient intake time by 40%  
* Achieve 95%+ patient satisfaction on intake process  
* Zero compliance incidents  
* Full integration with existing EMR within 30 days

**Investment:**

* Pilot: €45,000 (50% of standard pricing)  
* Includes full implementation support and dedicated CSM  
* No risk: If success criteria not met, no obligation to continue

**Path to Full Deployment:**

* If pilot successful: Full deployment proposal for all 12 hospitals  
* Estimated full value: €280,000 ARR  
* Implementation timeline: 6 months post-pilot

**Reference Commitment:**

* MedGroup agrees to participate in 1 case study and 2 reference calls in first year  
* Marketing rights to use MedGroup logo and results (with approval)

**Why This Makes Sense for MedGroup:**

* Test our solution with minimal risk  
* Validate results before major commitment  
* Get premium support at discounted pilot pricing  
* If it works, you're first mover in healthcare digital transformation"

---

## **Enter Workflow: Agent Summary**

| Agent | Role in Enter Workflow |
| ----- | ----- |
| Strategic Market Intelligence Agent | Analyzes new market opportunity and competitive landscape |
| Segment Strategy Agent | Defines beachhead segment and lighthouse targets |
| Value Proposition Optimization Agent | Adapts messaging for new market context |
| Offering Configuration Agent | Creates market entry pricing and pilot programs |
| Prospect Intelligence Agent | Researches lighthouse accounts and finds intro paths |
| Outreach Automation Agent | Executes thought leadership-led awareness building |
| Discovery Agent | Validates market hypotheses and learns market dynamics |
| Qualification Agent | Evaluates strategic value, not just revenue value |
| Value Selling Agent | Adapts ROI models and builds pilot success criteria |
| Sales Argumentation Agent | Creates market-specific messaging and objection handling |
| Proposal Generation Agent | Creates pilot-focused proposals with reference terms |
| Lead Nurturing Agent | Maintains engaged prospects for longer sales cycles |

**12 agents working together to systematically enter new markets.**

---

## **Business Impact of Enter Workflow**

| Metric | Without Agentic System | With Agentic System | Impact |
| ----- | ----- | ----- | ----- |
| Time to first lighthouse customer | 12-18 months | 6-9 months | 50% faster |
| Market research and analysis | Weeks of manual work | Days | 80% faster |
| Messaging iterations to find fit | Trial and error over months | Rapid A/B testing | Faster learning |
| Pilot-to-full conversion | 30-40% | 50-60% | \+50% improvement |
| Market learning capture | Informal, lost in emails | Systematic, fed back to strategy | Compounding intelligence |
| Lighthouse reference acquisition | Uncertain | Built into deal structure | Predictable |

---

## **Why Enter Is Harder (And Why Systems Matter More)**

1. **Unknown unknowns**: You don't know what you don't know about the new market. Systematic discovery and learning capture is essential.  
2. **No references**: You can't prove value with direct case studies. Agents help create compelling analogies and pilot-as-proof strategies.  
3. **Longer cycles**: New market deals take longer. Lead Nurturing Agent prevents opportunities from going cold.  
4. **Higher failure rate**: Not every beachhead attempt works. Systems help you fail fast, learn quickly, and adjust.  
5. **Learning must compound**: Each interaction should make you smarter about the market. Without systems, learning stays in salespeople's heads and leaves when they do.

---

## **When to Use Each Workflow**

| Workflow | Use When | Primary Goal | Time to Value |
| ----- | ----- | ----- | ----- |
| **Expand** | You have customers to grow | Maximize existing customer value | 30-90 days |
| **Acquire** | You need new customers in known markets | Predictable new customer acquisition | 90-180 days |
| **Enter** | You need to diversify into new markets | Establish beachhead in new market | 6-12 months |

**Recommended sequence:**

1. Start with **Expand** — prove the system, generate quick wins  
2. Add **Acquire** — build the growth engine  
3. Layer in **Enter** — when ready for strategic expansion

---

## **Why Start with Expand?**

1. **Existing relationships reduce risk** — you're not testing with prospects, you're testing with customers who already trust you  
2. **Data is available** — you have CRM data, usage data, and relationship history to work with  
3. **Quick wins build momentum** — closing an expansion deal in 30-60 days proves the system works  
4. **Learns your context** — the agents learn your offerings, customers, and winning patterns before you apply them to harder problems (new customer acquisition)  
5. **Funds further investment** — expansion revenue can fund the buildout of opportunity generation for new customers

# **SUMMARY: Three Ways to Communicate**

## **For Initial Conversations (Workflow-Led)**

"We help you systematically grow revenue from existing customers. Here's how our AI agents work together to identify, qualify, develop, and close expansion opportunities." → Use the Expand Workflow example

## **For Architecture Discussions (Systems-Led)**

"Every B2B sales organization needs two systems: one to generate qualified opportunities, one to convert them to closed deals. Here's how we build each." → Use the Two Systems illustrations

## **For Depth & Customization (Catalogue-Led)**

"We have 26 specialized AI agents across strategy, management, and execution layers. Based on your priorities, we select and configure the right agents for your situation." → Use the full Functional Requirements document

---

# **Value Proposition**

**Why our approach?**

| Benefit | How We Deliver It |
| ----- | ----- |
| **Faster time to market** | Pre-built agent architectures based on proven Lean Sales methodology — not starting from scratch |
| **Lower development cost** | Modular agents that can be configured, not custom-built for each client |
| **Lower implementation risk** | Battle-tested workflows based on real B2B sales patterns |
| **Flexibility** | Pick the agents you need, adapt to your sales process, CRM, and team structure |
| **Continuous improvement** | Management layer agents drive ongoing optimization based on your data |

**The foundation:** Our agentic sales system is built on the proven Lean Sales method, which focuses on making your sales funnel flow faster by eliminating waste and focusing on value — for both you and your customers.
