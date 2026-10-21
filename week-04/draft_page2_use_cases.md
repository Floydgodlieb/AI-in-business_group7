# AI use cases at SMEs: what do firms like mine use AI for, and what pays off?

## Why this question matters for a trader like you
Page 1 found that the gap that matters most is not knowing whether AI pays back for your own staff. This page names the uses found in the library, says what each one has been shown to pay, and takes one through the chapter template. No source in the library covers a trader of used vehicles, trailers or machinery, and BAS World is a frontier case, not the sector average.
- Most businesses use ready-made AI products; some try tailored applications, including AI agents. [W4-011, independently-verifiable, sector]

## The uses we found, and what pays off
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

## The one we take through the template: draft replies to standard buyer questions
We pick it because it closes the page 1 gap. Its result can be measured in a unit a trader already has (questions answered per hour), and BAS World names it as a low-risk place to start. [W4-I11, expert-opinion, general]

### Illustrative use case (CRISP-DM)
Honest about the data: no source in the library says which records a 10 to 50 person trader keeps of past buyer questions. Each phase below says what to look for, not what you have. We found no source on which question records a trader holds.

1. **Business understanding.** Goal: more standard buyer questions answered per salesperson-hour, with a salesperson still responsible for what the buyer receives. In the support study the assistant was built to support the agents, who stayed responsible for the conversation and could ignore its suggestions. [W4-026, independently-verifiable, sector] The measure that matters is time to answer, not revenue, since time saved does not directly lead to more revenue. [W4-034, company-reported, case]
2. **Data understanding.** Collect two weeks of real buyer questions with how long each took to answer. Check whether they carry personal data: BAS World's policy does not allow using personal data with AI. [W4-I09, company-reported, case] Check which questions repeat. We found no source on how much question history a trader has, so check this yourself before you plan.
3. **Data preparation.** Group the repeated questions into a short list of standard questions, and strip personal data from any example you give a tool. Nothing here needs a developer.
4. **Modelling.** You do not build or train a model. Buy a ready-made tool rather than building one. [W4-I12, expert-opinion, general] Many ready-made AI tools cost roughly €20 to €30 per user per month. [W4-I12, expert-opinion, general]
5. **Evaluation.** Compare against the two-week baseline: questions answered per salesperson-hour, and the share of drafts sent with only small edits. Watch each person separately. The gain was largest for novices and minimal for experienced staff [W4-025, independently-verifiable, sector], and weaker performers did worse in another setting. [W4-031, independently-verifiable, sector] The people checking the output must stay aware that they may rely on it too much (automation bias). [W4-013, independently-verifiable, sector]
6. **Deployment.** Start with drafts that a salesperson checks and sends. Move to a chat advisor that answers on its own only after three months of that. BAS World added guardrails before its own advisor went live [W4-I06, company-reported, case], and at HelloPrint satisfaction with the AI was lower than with staff. [W4-035, company-reported, case]

## The duties that apply
- **AI Act:** Companies that use AI must take steps to build AI know-how among their staff and others who work with the AI on their behalf. [W4-001, independently-verifiable, sector] An AI system that talks directly with people must be built so that people are told they are dealing with AI, unless that is obvious. [W4-003, independently-verifiable, sector]
- **GDPR (incl. who processes your data, and where):** The European data protection board says a legitimate interest can include building a conversational agent that helps users. [W4-004, independently-verifiable, sector] A customer of Anthropic can object to a new subprocessor in writing within 15 days of notice; otherwise the customer is treated as agreeing. [W4-014, independently-verifiable, sector]
- **Sanctions screening / Regulation 833/2014 (export documents):** Dutch exporters are legally required to follow the sanctions and to do careful checks to do so. [W4-006, independently-verifiable, sector] An AI that answers buyer questions does not take this check over; a person still screens the buyer before any quotation.

## What this looks like as recommendations
Each recommendation names one step in the chain (lead → quotation → contract → payment → export document).

1. **Lead — draft replies to standard buyer questions, which a salesperson checks and sends.**
   *Time-saving* automation: the AI writes, a person stays responsible for what the buyer receives. Complexity: **bought tooling**.
   Evidence: [W4-025, independently-verifiable, sector]; the assistant in that study supported agents who could ignore its suggestions. [W4-026, independently-verifiable, sector] Duty: AI Act AI literacy for the staff who use it [W4-001, independently-verifiable, sector]; GDPR basis for a conversational agent [W4-004, independently-verifiable, sector]. Supplier hosting: not known — ask before signing. For comparison, Microsoft 365 data stays inside an EU boundary [W4-015, independently-verifiable, sector], with limited exceptions [W4-016, independently-verifiable, sector].

2. **Lead — let a website chat advisor answer standard buyer questions on its own, only after recommendation 1 has run for three months.**
   *Customer-touching* automation: the buyer talks to the AI directly. Complexity: **named process owner**.
   Evidence: at BAS World, AI may currently act on its own in the AI advisor on the website. [W4-I04, company-reported, case] At HelloPrint satisfaction with the AI application is slightly lower (3.45 on a scale of 5) than with human service staff (3.75). [W4-035, company-reported, case] Duty: AI Act transparency, tell buyers they are talking to AI [W4-003, independently-verifiable, sector]; GDPR basis [W4-004, independently-verifiable, sector]. Supplier hosting: not known — ask before signing.

## Next step
- **Owner:** the commercial manager, as the one person responsible for this one process; buy a ready-made tool rather than building one. [W4-I12, expert-opinion, general]
- **Rough cost:** many ready-made AI tools cost roughly €20 to €30 per user per month [W4-I12, expert-opinion, general], plus the owner's time to run the two-week baseline and give the sales staff a short AI-literacy briefing [W4-001, independently-verifiable, sector].
- **Three-month check:** compare standard buyer questions answered per salesperson-hour, and the share of AI drafts sent with only small edits, against the two weeks measured before the start; then check whether the freed hours went into quotations, because time saved does not by itself raise revenue. [W4-034, company-reported, case]

## Disclaimer
**Educational, not consultancy.** This handbook offers inspiration and starting points, not commercial advice or guarantees. Every chapter carries this disclaimer. Decisions about a firm remain the firm's own.
