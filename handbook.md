# Handbook: AI for a Dutch trader in used commercial vehicles, trailers and machinery

For the owner or commercial manager of a trader with 10 to 50 staff, no IT function, selling B2B to mostly non-EU markets. BAS World (Veghel) is the frontier case: it shows what stays hard once budget and IT are no longer the limit. It is not the sector average. Each chapter is one page and ends with one next step.

| Chapter | Question | Built from |
|---|---|---|
| 1 | Who owns the AI tools I use, and what happens to my business if that changes? | week 2 |
| 2 | Can I trust this AI tool, with my data, its answers and my people? | week 3 |
| 3 | SME knowledge gaps: what do we not know yet about AI? | week 4, page 1 |
| 4 | AI use cases at SMEs: what do firms like mine use AI for, and what pays off? | week 4, page 2 |

Every figure is labelled `company-reported` or `independently-verifiable`, and every claim `case` or `sector`. Chapters 3 and 4 were written to be read together: chapter 4 takes the gap named in chapter 3 through the chapter template.

---
<!-- chapter 1: week 2 -->
## Who owns the AI tools I use, and what happens to my business if that changes?

### Why this question matters for a trader like you

In 2024, 22.7% of Dutch businesses with 10 or more staff used one or more AI technologies — up
almost 9 percentage points from 2023 [W2-001, independently-verifiable, sector]. AI use is highest at large companies and lowest at
the smallest ones [W2-002, independently-verifiable, sector], and businesses that already use AI
skew larger than the 10-49 staff bracket most traders in this sector sit in
[W2-003, independently-verifiable, sector]. Trade is the single largest sector among AI-using
businesses [W2-004, independently-verifiable, sector] — so this is already happening in
businesses like yours, not just at the frontier.

BAS World, a much larger Dutch trader in the same kind of goods, is that frontier case: its AI
agents for sales, pricing and customer service run on a modular setup hosted on AWS
[W2-021, company-reported, case], built to be model-agnostic — ChatGPT, Gemini and Claude are
all interchangeable [W2-022, company-reported, case] — and designed so BAS World is not stuck
depending on the implementation partner that built it [W2-023, company-reported, case]. That
"not stuck depending on" design choice is itself the answer to this page's question: it is
possible to reduce lock-in, but it has to be designed in, not assumed.

### What you depend on, and why it can change

When you use an AI tool, you are usually depending on a foreign supplier for the software, and
often for where your data is processed too:

- Microsoft's own documentation says Copilot normally sends your prompts to the nearest regional
  data centre, but can send them to another region if the regional data centre is full
  [W2-028, company-reported, sector]. For EU customers, Microsoft says EU traffic is kept inside
  an "EU Data Boundary" [W2-029, company-reported, sector] — but Microsoft also states that one
  of its AI models, supplied by Anthropic, is currently excluded from that EU boundary
  [W2-030, company-reported, sector]. In other words: "hosted in the EU" can have exceptions, and
  they can be model-specific.
- DeepL, a translation tool, is a German company [W2-024, company-reported, sector], but its own
  contract terms allow it to process your text on servers run by other cloud companies, with no
  fixed location guaranteed unless you negotiate one [W2-025, company-reported, sector].
- Nationally, the Dutch central bank and financial regulator have separately warned that a
  sector that leans on a small number of non-European IT suppliers takes on a real, growing risk
  [W2-013, independently-verifiable, sector], precisely because everyone ends up on the same
  handful of providers and infrastructure [W2-014, independently-verifiable, sector]. That
  warning was written about banks, not vehicle traders — but the mechanism it describes
  (concentration on a few non-EU suppliers) is the same one this page is about.
- The Rathenau Instituut, an independent Dutch research institute, makes the same point about
  Dutch public organisations more broadly: growing dependence on a handful of large American
  tech companies — for cloud, software, AI tools and equipment — leaves the dependent
  organisation vulnerable [W2-031, independently-verifiable, sector].
- At EU level, the Draghi report — the European Commission's own competitiveness review — was
  published in September 2024 [W2-011, independently-verifiable, sector] and found that slowing
  productivity, an ageing population, rising energy costs and tougher global competition are all
  putting pressure on Europe's economy [W2-012, independently-verifiable, sector].
- On the "what happens if it changes" question directly: a Bruegel commentary describes everyone
  outside the US and China as living in "managed dependence" on foreign AI providers, and points
  to a directive restricting non-US access to certain AI models as an example of what that
  dependence can mean in practice [W2-019, independently-verifiable, sector].

### The duties that apply

- **AI Act.** If a tool you use counts as "high-risk" under the EU AI Act, the law requires you,
  as the business using it (the "deployer"), to use it according to the supplier's instructions
  [W2-009, independently-verifiable, sector], and to tell people when they are subject to it
  [W2-010, independently-verifiable, sector].
- **GDPR.** If a supplier processes personal data on your behalf (most cloud AI tools do), the
  European Commission has published standard contract clauses for exactly this relationship,
  under Article 28(7) of the GDPR [W2-020, independently-verifiable, sector]. You need one of
  these (or an equivalent) signed with every such supplier.
- **Sanctions screening / export documents.** Dutch Customs states plainly that export of some
  goods to some countries is banned outright, or allowed only with a permit
  [W2-005, independently-verifiable, sector]. At EU level, the sanctions regime on Russia (legal
  basis: Council Regulation (EU) No 833/2014 [W2-008, independently-verifiable, sector]) bans
  export of dual-use and advanced-technology goods, including semiconductors and software
  [W2-006, independently-verifiable, sector], and separately restricts transport equipment and
  goods used in aviation, space and maritime navigation [W2-007, independently-verifiable,
  sector]. If your export documents touch Russia-bound trade in any way, this is the duty an AI
  screening tool has to help you meet — not replace your judgement about.

### What this looks like as recommendations

Each recommendation below names one step in your sales or documentation chain
(lead → quotation → contract → payment → export document), says whether it saves you time or
touches the customer, and how complex it is to adopt.

1. **Export document step — screening trading partners against sanctions lists.**
   *Time-saving automation, not customer-touching.* Complexity: **bought tooling**. Products
   such as Descartes' Denied Party Screening automate checking a trading partner against
   government watchlists and plug into your own systems
   [W2-026, company-reported, sector]. Descartes itself claims an AI feature that cuts false
   positives by 60% [W2-027, company-reported, sector] — that is the vendor's own figure, not
   independently checked, so treat it as a starting point for a demo, not a guarantee.

2. **Lead / quotation step — translating listings and quotes for non-EU buyers.**
   *Customer-touching automation* (the buyer sees the translated text directly). Complexity:
   **bought tooling**. A translation tool is a plausible fit here, but confirm in its contract
   where your text is actually processed before you rely on it for anything commercially
   sensitive [W2-025, company-reported, sector] — "translation vendor" is not automatically
   "EU-hosted." The duty that applies is the same one as in the Duties section above: get a
   GDPR Article 28 data-processing agreement with this supplier too, before it ever sees a real
   customer quote [W2-020, independently-verifiable, sector].

3. **Quotation step — AI-assisted pricing.** *Time-saving automation, not customer-touching* (it
   informs a price your staff still sets). Complexity: **in-house build — flagged as a
   warning**. BAS World's pricing agent is a custom, purpose-built system on a modular
   architecture [W2-023, company-reported, case]. That took a much larger company, with an IT
   partner, to build. For a 10-50 staff trader with no IT function, copying this approach
   directly is very unlikely to be the right first step; treat it as evidence of what is
   possible at scale, not a template to copy. The duty to check before adopting anything like
   this is the same AI Act deployer duty named above: confirm with whoever builds or sells you
   the tool whether it counts as high-risk, and if so, that you can meet the instructions-for-use
   and oversight duty it carries [W2-009, independently-verifiable, sector].

4. **Contract step — the data-processing agreement itself.** *Not customer-touching; a compliance
   step, not a saving.* Complexity: **named process owner**. Someone in the business — named, not
   "whoever has time" — should be responsible for getting a GDPR Article 28 data-processing
   agreement signed with every AI supplier that touches customer or contract data
   [W2-020, independently-verifiable, sector], and for checking each supplier's AI Act deployer
   obligations apply and are met [W2-009, independently-verifiable, sector].

### Next step

- **Owner:** the commercial manager, named as the one person responsible for every agreement with an AI supplier (recommendation 4). [W2-020, independently-verifiable, sector]
- **Rough cost:** no licence cost; the owner's time to list the AI tools in use, ask each supplier where it processes data, and get a GDPR Article 28 data-processing agreement signed. [W2-020, independently-verifiable, sector]
- **Three-month check:** you hold a signed data-processing agreement, or a written reason why none is needed, for every AI supplier that touches customer or contract data, and a written answer from each on where it processes your text. [W2-020, independently-verifiable, sector] [W2-025, company-reported, sector]

### Disclaimer

**Educational, not consultancy.** This handbook offers inspiration and starting points, not commercial advice or guarantees. Every chapter carries this disclaimer. Decisions about a firm remain the firm's own.

---

<!-- chapter 2: week 3 -->
## Can I trust this AI tool — with my data, its answers and my people?

Week 2 asked who owns the AI tools you use, using this trade's frontier case as evidence. This
week asks whether you — a Dutch trader in used commercial vehicles and machinery — can trust
what they do with your data, tell your customers, or let staff use unnoticed.

### What leaves the building

Even "hosted in the EU" can have exceptions — Microsoft's own EU Data Boundary currently
excludes one model supplier entirely [S-015, company-reported, sector]. Whatever a supplier
processes for you, the GDPR duty is the same regardless of the tool: sign a data-processing
agreement before it ever sees a real customer record [S-011, independently-verifiable, sector].
Running a model yourself is a real 2026 option, but a later step for a firm with no IT function
[S-027, company-reported, sector].

### Act, or only advise?

Ask this two ways and the answer changes. "What can AI do for us" returns generic optimism;
"who pays when it gets it wrong" does not — a tribunal held an airline liable for its own
chatbot's wrong answer to a customer [S-026, independently-verifiable, sector]: a business
answers for its AI's answers, whatever AI-specific law says. The AI Act's own human-oversight
rule — a named person can override or stop the system
[S-023, independently-verifiable, sector] — binds only "high-risk" tools, pushed back to
December 2027 for most of them by a 2026 reform [S-024, independently-verifiable, sector]. Not
yet a duty here, but a cheap habit to start.

### Staff using AI without saying so

A 2025 study of 600 firms found "shadow AI" — staff using tools the business never approved —
added $670,000 to the average breach cost, and caused one in five breaches outright
[S-019, independently-verifiable, sector]. Shadow AI is itself a recognised risk category in
peer-reviewed cybersecurity research, not just industry framing
[S-028, independently-verifiable, sector]. "We never approved it" is no defence: the AI Act
counts you as a "deployer" just by using a tool, approved or not
[S-022, independently-verifiable, sector].

### Recommendations

1. **Lead/quotation step — customer-facing AI.** Customer-touching, named process owner: decide
   which AI-generated answers a person must check before they reach a customer [S-026].
2. **Quotation step — translation for buyer quotes.** Customer-touching, bought tooling: check
   where the contract says your text is processed, and sign the data-processing agreement first
   [S-011, S-015].
3. **Every step, the one deliberate exception — a one-page AI-use policy.** Not customer-touching
   and not a saving either; a governance step. Named process owner: name which tools staff may
   use and what must never go into them [S-019, S-022].

### Next step

**Owner:** the commercial manager, for the policy — no new tool needed. **Rough cost:** half a
day to draft, one meeting to agree. **Three-month check:** ask staff which tools they actually
used, against what the policy names.

### AI-use disclosure

AI-drafted from the appraised source bank only, nothing from memory; every quote hand-checked
against its source. Floyd reviewed and directed this revision. The team's own second-reader
check has been done.

### Disclaimer

**Educational, not consultancy.** This handbook offers inspiration and starting points, not
commercial advice or guarantees. Every chapter carries this disclaimer. Decisions about a firm
remain the firm's own.

---

<!-- chapter 3: week 4 page 1 -->
## SME knowledge gaps: what do we not know yet about AI, and what would we need to know to decide well?

### Why this question matters for a trader like you
You are deciding whether to spend money and staff time on AI. Before you decide, you need to know what the firms that said no were missing, and what firms that said yes had to put in place. BAS World is a frontier case, not the sector average, and the library holds no statement from BAS World naming its own knowledge gaps. What follows keeps apart what firms say they need and what the evidence shows they need.

### What the firm already knows and does
Case: BAS World (frontier case, not the sector average).
- It knows why it started: the efficiency gains, which let it do things it previously had no time for. [W4-I08, company-reported, case]
- It uses AI heavily in daily work and builds many AI tools itself. [W4-I01, company-reported, case]
- It knows where AI may act alone: in its website AI advisor and in an agent that assigns tickets to colleagues in sales. [W4-I04, company-reported, case] Before the advisor went live, it added guardrails. [W4-I06, company-reported, case]
- It knows where a person stays in charge: a human approves merge requests, and a person checks and approves every security fix the AI makes. [W4-I05, company-reported, case]
- It has a rule and a test funnel for data and tools: company policy does not allow personal data with AI, and new tools go through an "AI tech radar" before approval. [W4-I09, company-reported, case] It uses tools from the US, but not from China. [W4-I10, company-reported, case]
- It knows where to stop: it draws a line wherever things could break, revenue could be lost, or security is at risk. [W4-I07, company-reported, case]

The sector figures show how far the typical firm is from this.
- In 2025 in the EU, 17% of small, 30.36% of medium and 55.03% of large enterprises used AI. [W4-018, independently-verifiable, sector]
- The increase is strongest at Dutch companies with 50 to 250 employees: from 20 percent in 2023 to 45 percent in 2025. [W4-022, independently-verifiable, sector]

### What the firm lacks
#### What firms say they need
- Among EU companies that had considered AI in 2025, the most common reason for not using it was lack of expertise (70.89%), then unclear legal consequences (52.52%), then data protection and privacy worries (48.83%). [W4-017, independently-verifiable, sector]
- Among Dutch micro-businesses that decided against AI in 2025, lack of experience was by far the main reason (71.6 percent). [W4-019, independently-verifiable, sector] In medium-sized, small and large Dutch companies too, lack of experience came first. [W4-020, independently-verifiable, sector]
- Among euro-area firms that do not use AI or use it little, the barrier named most often is a lack of AI skills, then data, privacy and ethics concerns, then poor fit with existing systems. [W4-023, independently-verifiable, sector]
- Firms adopt digital tools for efficiency and growth, but lack of time, maintenance costs and skills gaps keep getting in the way of putting them to work. [W4-010, independently-verifiable, sector]
- BAS World itself names no gap in the interview material. What it says it needs is a limit: a line wherever there is a risk that things break, that revenue is lost, or that security is at stake. [W4-I07, company-reported, case]

#### What the evidence shows they need
- **A short list of legal duties, which are more specific than "unclear" suggests.** Companies that use AI must take steps to build AI know-how among their staff and others who work with the AI on their behalf. [W4-001, independently-verifiable, sector] The rule does not require a guaranteed skill level for any one person. [W4-002, independently-verifiable, sector] A chat advisor that talks directly with people must tell them they are dealing with AI, unless that is obvious. [W4-003, independently-verifiable, sector]
- **Proof of return, which firms do not name as a gap.** In a large study of workers, AI chatbots had a modest overall effect: users report saving 2.8% of work hours on average. [W4-028, independently-verifiable, sector] The range ran from 6.8% for marketing professionals whose employers encourage chatbot use to 0.6% for teachers in schools that do not. [W4-029, independently-verifiable, sector] Controlled experiments may show the gains of a well-coordinated, carefully managed rollout, not of everyday use. [W4-030, independently-verifiable, sector]
- **Knowing who gains and who loses.** In a study of customer support agents, an AI assistant raised issues resolved per hour by 14% on average, by 34% for novices, with minimal effect for experienced staff. [W4-025, independently-verifiable, sector] In a field experiment with Kenyan small-business owners using an AI business assistant, weaker performers did nearly 10% worse, while stronger performers may have gained over 15%. [W4-031, independently-verifiable, sector]
- **Knowing that saved time is not yet revenue.** The HelloPrint cases show that time saved does not directly lead to more productivity or revenue. [W4-034, company-reported, case]
- **Knowing where your data goes.** A customer of Anthropic can object to a new subprocessor on data privacy or security grounds, in writing within 15 days of notice; otherwise the customer is treated as agreeing. [W4-014, independently-verifiable, sector] Microsoft's EU boundary commitment for Microsoft 365 has limited exceptions in which data is still transferred outside the EU. [W4-016, independently-verifiable, sector] Who handles your data can therefore change while your contract runs.

#### Where the two differ
Firms say they lack expertise. The evidence agrees, and then adds what the survey does not ask about. Expertise is a legal duty, not only a wish. [W4-001, independently-verifiable, sector] The legal rules for a chat advisor are short and findable. [W4-003, independently-verifiable, sector] The larger gap is knowing whether it pays back for your own staff, because the same tool gave large gains to novices [W4-025, independently-verifiable, sector] and made weaker performers worse in another setting. [W4-031, independently-verifiable, sector] No source in the library says how a trader of used vehicles would measure this. That difference is the finding.

### The gap that matters most for a decision you face now
The decision: whether to put one ready-made AI tool on one recurring task. Of the gaps above, the return gap decides it, because without a baseline you cannot tell a 14% gain from a 0.6% one. [W4-025, independently-verifiable, sector] [W4-029, independently-verifiable, sector] BAS World's own advice to others is to start with one recurring task that takes a lot of time and carries little risk. [W4-I11, expert-opinion, general] Page 2 takes one such task through the chapter template.

### The duties that apply
- **AI Act:** staff who use AI need AI literacy [W4-001, independently-verifiable, sector], and a chat advisor must tell people it is AI. [W4-003, independently-verifiable, sector]
- **GDPR (incl. who processes your data, and where):** the European data protection board says a legitimate interest can include building a conversational agent that helps users. [W4-004, independently-verifiable, sector] Where your supplier processes the data, and who it may add as a subprocessor, is set in its contract. [W4-014, independently-verifiable, sector]
- **Sanctions screening / Regulation 833/2014 (export documents):** Dutch exporters are legally required to follow the sanctions and to do careful checks to do so. [W4-006, independently-verifiable, sector] Dual-use products may never be exported without a licence, whatever the destination outside the EU. [W4-007, independently-verifiable, sector] An AI that answers buyer questions does not take this check over; a person still screens the buyer before any quotation.

### What this looks like as recommendations
Each recommendation closes one gap and names one step in the chain (lead → quotation → contract → payment → export document).

1. **Lead — time how long standard buyer questions take today, before any tool.**
   *Time-saving* groundwork: nothing is automated yet; this only creates the baseline that closes the return gap. Complexity: **named process owner**.
   Evidence: the studies above measure issues resolved per hour [W4-025, independently-verifiable, sector], and time saved does not by itself raise revenue [W4-034, company-reported, case]. Duty: AI Act AI literacy for the staff who will use a tool later [W4-001, independently-verifiable, sector]. Supplier hosting: not known — no supplier chosen yet.

2. **Lead — before signing with any AI supplier, ask where it processes buyer data and who it may add as a subprocessor.**
   *Time-saving* groundwork: it costs one email and closes the data-location gap. Complexity: **named process owner**.
   Evidence: subprocessor changes run on a 15-day objection window [W4-014, independently-verifiable, sector]. Duty: GDPR basis and processor terms [W4-004, independently-verifiable, sector]. Supplier hosting: not known — ask before signing. For comparison, Microsoft 365 data stays inside an EU boundary [W4-015, independently-verifiable, sector], with limited exceptions [W4-016, independently-verifiable, sector].

### Next step
- **Owner:** the commercial manager, as the one person responsible for this one process. [W4-I12, expert-opinion, general]
- **Rough cost:** no licence cost yet; the owner's time, the sales staff's time to note durations for two weeks, and a short AI-literacy briefing. [W4-001, independently-verifiable, sector]
- **Three-month check:** you can state, in numbers, how many standard buyer questions a salesperson answers per hour today, and you hold a written answer from each candidate supplier on where it processes data.

### Disclaimer
**Educational, not consultancy.** This handbook offers inspiration and starting points, not commercial advice or guarantees. Every chapter carries this disclaimer. Decisions about a firm remain the firm's own.

---

<!-- chapter 4: week 4 page 2 -->
## AI use cases at SMEs: what do firms like mine use AI for, and what pays off?

### Why this question matters for a trader like you
Page 1 found that the gap that matters most is not knowing whether AI pays back for your own staff. This page names the uses found in the library, says what each one has been shown to pay, and takes one through the chapter template. No source in the library covers a trader of used vehicles, trailers or machinery, and BAS World is a frontier case, not the sector average.
- Most businesses use ready-made AI products; some try tailored applications, including AI agents. [W4-011, independently-verifiable, sector]

### The uses we found, and what pays off
**Answering customer questions**
- In a study of customer support agents, an AI assistant raised issues resolved per hour by 14% on average, by 34% for novices, with minimal effect for experienced staff. [W4-025, independently-verifiable, sector]
- At BAS World, AI may act on its own in the website AI advisor. [W4-I04, company-reported, case]
- At the Dutch printer HelloPrint (another firm, not BAS World), large-scale automation of customer contact led to large cost savings (about 80% fewer staff), as reported in interviews. [W4-033, company-reported, case] Customer satisfaction with the AI application is slightly lower (3.45 on a scale of 5) than with human service staff (3.75). [W4-035, company-reported, case]

**Routing work to colleagues**
- At BAS World, an agent assigns tickets to colleagues in sales. [W4-I04, company-reported, case] No payoff figure is given.

**Writing and translating texts**
- BAS World advises smaller traders to start with writing and translating advertisement texts, or answering standard customer questions. [W4-I11, expert-opinion, general]
- In an experiment with professional writing tasks, people using ChatGPT finished 10 minutes (37%) faster than the control group, who took 27 minutes on average. [W4-027, independently-verifiable, sector]

**Writing software**
- BAS World's teams build many AI tools, and IT colleagues use Claude most. [W4-I01, company-reported, case] Without AI its AI applications would break, and it would need more engineers and move less quickly. [W4-I02, company-reported, case] A person still checks and approves what the AI produces. [W4-I05, company-reported, case]

**A general business assistant for owners**
- In a field experiment with Kenyan small-business owners using an AI business assistant, weaker performers did nearly 10% worse, while stronger performers may have gained over 15%. [W4-031, independently-verifiable, sector]

**What pays off, put plainly**
- Across workers, AI chatbots had a modest overall effect: users report saving 2.8% of work hours on average. [W4-028, independently-verifiable, sector] The range ran from 6.8% to 0.6%, depending on whether the employer encourages use. [W4-029, independently-verifiable, sector]
- Controlled experiments may show the gains of a well-coordinated, carefully managed rollout, not of everyday use. [W4-030, independently-verifiable, sector]
- Time saved does not directly lead to more productivity or revenue. [W4-034, company-reported, case]
- Every payoff figure above is a time or staff figure from a setting other than a trader. None is a measured gain in sales.

### The one we take through the template: draft replies to standard buyer questions
We pick it because it closes the page 1 gap. Its result can be measured in a unit a trader already has (questions answered per hour), and BAS World names it as a low-risk place to start. [W4-I11, expert-opinion, general]

#### Illustrative use case (CRISP-DM)
Honest about the data: no source in the library says which records a 10 to 50 person trader keeps of past buyer questions. Each phase below says what to look for, not what you have. We found no source on which question records a trader holds.

1. **Business understanding.** Goal: more standard buyer questions answered per salesperson-hour, with a salesperson still responsible for what the buyer receives. In the support study the assistant was built to support the agents, who stayed responsible for the conversation and could ignore its suggestions. [W4-026, independently-verifiable, sector] The measure that matters is time to answer, not revenue, since time saved does not directly lead to more revenue. [W4-034, company-reported, case]
2. **Data understanding.** Collect two weeks of real buyer questions with how long each took to answer. Check whether they carry personal data: BAS World's policy does not allow using personal data with AI. [W4-I09, company-reported, case] Check which questions repeat. We found no source on how much question history a trader has, so check this yourself before you plan.
3. **Data preparation.** Group the repeated questions into a short list of standard questions, and strip personal data from any example you give a tool. Nothing here needs a developer.
4. **Modelling.** You do not build or train a model. Buy a ready-made tool rather than building one. [W4-I12, expert-opinion, general] Many ready-made AI tools cost roughly €20 to €30 per user per month. [W4-I12, expert-opinion, general]
5. **Evaluation.** Compare against the two-week baseline: questions answered per salesperson-hour, and the share of drafts sent with only small edits. Watch each person separately. The gain was largest for novices and minimal for experienced staff [W4-025, independently-verifiable, sector], and weaker performers did worse in another setting. [W4-031, independently-verifiable, sector] The people checking the output must stay aware that they may rely on it too much (automation bias). [W4-013, independently-verifiable, sector]
6. **Deployment.** Start with drafts that a salesperson checks and sends. Move to a chat advisor that answers on its own only after three months of that. BAS World added guardrails before its own advisor went live [W4-I06, company-reported, case], and at HelloPrint satisfaction with the AI was lower than with staff. [W4-035, company-reported, case]

### The duties that apply
- **AI Act:** Companies that use AI must take steps to build AI know-how among their staff and others who work with the AI on their behalf. [W4-001, independently-verifiable, sector] An AI system that talks directly with people must be built so that people are told they are dealing with AI, unless that is obvious. [W4-003, independently-verifiable, sector]
- **GDPR (incl. who processes your data, and where):** The European data protection board says a legitimate interest can include building a conversational agent that helps users. [W4-004, independently-verifiable, sector] A customer of Anthropic can object to a new subprocessor in writing within 15 days of notice; otherwise the customer is treated as agreeing. [W4-014, independently-verifiable, sector]
- **Sanctions screening / Regulation 833/2014 (export documents):** Dutch exporters are legally required to follow the sanctions and to do careful checks to do so. [W4-006, independently-verifiable, sector] An AI that answers buyer questions does not take this check over; a person still screens the buyer before any quotation.

### What this looks like as recommendations
Each recommendation names one step in the chain (lead → quotation → contract → payment → export document).

1. **Lead — draft replies to standard buyer questions, which a salesperson checks and sends.**
   *Time-saving* automation: the AI writes, a person stays responsible for what the buyer receives. Complexity: **bought tooling**.
   Evidence: [W4-025, independently-verifiable, sector]; the assistant in that study supported agents who could ignore its suggestions. [W4-026, independently-verifiable, sector] Duty: AI Act AI literacy for the staff who use it [W4-001, independently-verifiable, sector]; GDPR basis for a conversational agent [W4-004, independently-verifiable, sector]. Supplier hosting: not known — ask before signing. For comparison, Microsoft 365 data stays inside an EU boundary [W4-015, independently-verifiable, sector], with limited exceptions [W4-016, independently-verifiable, sector].

2. **Lead — let a website chat advisor answer standard buyer questions on its own, only after recommendation 1 has run for three months.**
   *Customer-touching* automation: the buyer talks to the AI directly. Complexity: **named process owner**.
   Evidence: at BAS World, AI may currently act on its own in the AI advisor on the website. [W4-I04, company-reported, case] At HelloPrint satisfaction with the AI application is slightly lower (3.45 on a scale of 5) than with human service staff (3.75). [W4-035, company-reported, case] Duty: AI Act transparency, tell buyers they are talking to AI [W4-003, independently-verifiable, sector]; GDPR basis [W4-004, independently-verifiable, sector]. Supplier hosting: not known — ask before signing.

### Next step
- **Owner:** the commercial manager, as the one person responsible for this one process; buy a ready-made tool rather than building one. [W4-I12, expert-opinion, general]
- **Rough cost:** many ready-made AI tools cost roughly €20 to €30 per user per month [W4-I12, expert-opinion, general], plus the owner's time to run the two-week baseline and give the sales staff a short AI-literacy briefing [W4-001, independently-verifiable, sector].
- **Three-month check:** compare standard buyer questions answered per salesperson-hour, and the share of AI drafts sent with only small edits, against the two weeks measured before the start; then check whether the freed hours went into quotations, because time saved does not by itself raise revenue. [W4-034, company-reported, case]

### Disclaimer
**Educational, not consultancy.** This handbook offers inspiration and starting points, not commercial advice or guarantees. Every chapter carries this disclaimer. Decisions about a firm remain the firm's own.

---

## How much checking was done

| Chapter | Checked | Still open |
|---|---|---|
| 1. Who owns the AI tools I use | Version 1.0 (17-09-2026): the second reader passed all 4 criteria and spot-checked 5 statements against their original source, per check.md. The Bruegel statement (W2-019) was checked against its source by a person (Floyd). | |
| 2. Can I trust this AI tool | Drafted from the appraised source bank only, nothing from memory; every quote hand-checked against its source. The second-reader check has been done. | |
| 3. SME knowledge gaps | 20 of 22 statements auto-verified against the live source; 2 sources checked by a person (review_queue.md); all numbers checked. Second reader: Aaron. | |
| 4. AI use cases at SMEs | 15 of 19 statements auto-verified against the live source; 2 sources checked by a person (review_queue.md); all numbers checked. Second reader: Aaron. | |
