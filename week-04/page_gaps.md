version: 1.0 · date: 2026-10-21 · context: 1.5

# SME knowledge gaps: what do we not know yet about AI, and what would we need to know to decide well?

*How much checking was done: 20 of 22 statements auto-verified against the live source; 2 sources checked by a person (review_queue.md); all numbers checked; second reader: Aaron.*

## Why this question matters for a trader like you
You are deciding whether to spend money and staff time on AI. Before you decide, you need to know what the firms that said no were missing, and what firms that said yes had to put in place. BAS World is a frontier case, not the sector average, and the library holds no statement from BAS World naming its own knowledge gaps. What follows keeps apart what firms say they need and what the evidence shows they need.

## What the firm already knows and does
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

## What the firm lacks
### What firms say they need
- Among EU companies that had considered AI in 2025, the most common reason for not using it was lack of expertise (70.89%), then unclear legal consequences (52.52%), then data protection and privacy worries (48.83%). [W4-017, independently-verifiable, sector]
- Among Dutch micro-businesses that decided against AI in 2025, lack of experience was by far the main reason (71.6 percent). [W4-019, independently-verifiable, sector] In medium-sized, small and large Dutch companies too, lack of experience came first. [W4-020, independently-verifiable, sector]
- Among euro-area firms that do not use AI or use it little, the barrier named most often is a lack of AI skills, then data, privacy and ethics concerns, then poor fit with existing systems. [W4-023, independently-verifiable, sector]
- Firms adopt digital tools for efficiency and growth, but lack of time, maintenance costs and skills gaps keep getting in the way of putting them to work. [W4-010, independently-verifiable, sector]
- BAS World itself names no gap in the interview material. What it says it needs is a limit: a line wherever there is a risk that things break, that revenue is lost, or that security is at stake. [W4-I07, company-reported, case]

### What the evidence shows they need
- **A short list of legal duties, which are more specific than "unclear" suggests.** Companies that use AI must take steps to build AI know-how among their staff and others who work with the AI on their behalf. [W4-001, independently-verifiable, sector] The rule does not require a guaranteed skill level for any one person. [W4-002, independently-verifiable, sector] A chat advisor that talks directly with people must tell them they are dealing with AI, unless that is obvious. [W4-003, independently-verifiable, sector]
- **Proof of return, which firms do not name as a gap.** In a large study of workers, AI chatbots had a modest overall effect: users report saving 2.8% of work hours on average. [W4-028, independently-verifiable, sector] The range ran from 6.8% for marketing professionals whose employers encourage chatbot use to 0.6% for teachers in schools that do not. [W4-029, independently-verifiable, sector] Controlled experiments may show the gains of a well-coordinated, carefully managed rollout, not of everyday use. [W4-030, independently-verifiable, sector]
- **Knowing who gains and who loses.** In a study of customer support agents, an AI assistant raised issues resolved per hour by 14% on average, by 34% for novices, with minimal effect for experienced staff. [W4-025, independently-verifiable, sector] In a field experiment with Kenyan small-business owners using an AI business assistant, weaker performers did nearly 10% worse, while stronger performers may have gained over 15%. [W4-031, independently-verifiable, sector]
- **Knowing that saved time is not yet revenue.** The HelloPrint cases show that time saved does not directly lead to more productivity or revenue. [W4-034, company-reported, case]
- **Knowing where your data goes.** A customer of Anthropic can object to a new subprocessor on data privacy or security grounds, in writing within 15 days of notice; otherwise the customer is treated as agreeing. [W4-014, independently-verifiable, sector] Microsoft's EU boundary commitment for Microsoft 365 has limited exceptions in which data is still transferred outside the EU. [W4-016, independently-verifiable, sector] Who handles your data can therefore change while your contract runs.

### Where the two differ
Firms say they lack expertise. The evidence agrees, and then adds what the survey does not ask about. Expertise is a legal duty, not only a wish. [W4-001, independently-verifiable, sector] The legal rules for a chat advisor are short and findable. [W4-003, independently-verifiable, sector] The larger gap is knowing whether it pays back for your own staff, because the same tool gave large gains to novices [W4-025, independently-verifiable, sector] and made weaker performers worse in another setting. [W4-031, independently-verifiable, sector] No source in the library says how a trader of used vehicles would measure this. That difference is the finding.

## The gap that matters most for a decision you face now
The decision: whether to put one ready-made AI tool on one recurring task. Of the gaps above, the return gap decides it, because without a baseline you cannot tell a 14% gain from a 0.6% one. [W4-025, independently-verifiable, sector] [W4-029, independently-verifiable, sector] BAS World's own advice to others is to start with one recurring task that takes a lot of time and carries little risk. [W4-I11, expert-opinion, general] Page 2 takes one such task through the chapter template.

## The duties that apply
- **AI Act:** staff who use AI need AI literacy [W4-001, independently-verifiable, sector], and a chat advisor must tell people it is AI. [W4-003, independently-verifiable, sector]
- **GDPR (incl. who processes your data, and where):** the European data protection board says a legitimate interest can include building a conversational agent that helps users. [W4-004, independently-verifiable, sector] Where your supplier processes the data, and who it may add as a subprocessor, is set in its contract. [W4-014, independently-verifiable, sector]
- **Sanctions screening / Regulation 833/2014 (export documents):** Dutch exporters are legally required to follow the sanctions and to do careful checks to do so. [W4-006, independently-verifiable, sector] Dual-use products may never be exported without a licence, whatever the destination outside the EU. [W4-007, independently-verifiable, sector] An AI that answers buyer questions does not take this check over; a person still screens the buyer before any quotation.

## What this looks like as recommendations
Each recommendation closes one gap and names one step in the chain (lead → quotation → contract → payment → export document).

1. **Lead — time how long standard buyer questions take today, before any tool.**
   *Time-saving* groundwork: nothing is automated yet; this only creates the baseline that closes the return gap. Complexity: **named process owner**.
   Evidence: the studies above measure issues resolved per hour [W4-025, independently-verifiable, sector], and time saved does not by itself raise revenue [W4-034, company-reported, case]. Duty: AI Act AI literacy for the staff who will use a tool later [W4-001, independently-verifiable, sector]. Supplier hosting: not known — no supplier chosen yet.

2. **Lead — before signing with any AI supplier, ask where it processes buyer data and who it may add as a subprocessor.**
   *Time-saving* groundwork: it costs one email and closes the data-location gap. Complexity: **named process owner**.
   Evidence: subprocessor changes run on a 15-day objection window [W4-014, independently-verifiable, sector]. Duty: GDPR basis and processor terms [W4-004, independently-verifiable, sector]. Supplier hosting: not known — ask before signing. For comparison, Microsoft 365 data stays inside an EU boundary [W4-015, independently-verifiable, sector], with limited exceptions [W4-016, independently-verifiable, sector].

## Next step
- **Owner:** the commercial manager, as the one person responsible for this one process. [W4-I12, expert-opinion, general]
- **Rough cost:** no licence cost yet; the owner's time, the sales staff's time to note durations for two weeks, and a short AI-literacy briefing. [W4-001, independently-verifiable, sector]
- **Three-month check:** you can state, in numbers, how many standard buyer questions a salesperson answers per hour today, and you hold a written answer from each candidate supplier on where it processes data.

## Disclaimer
**Educational, not consultancy.** This handbook offers inspiration and starting points, not commercial advice or guarantees. Every chapter carries this disclaimer. Decisions about a firm remain the firm's own.
