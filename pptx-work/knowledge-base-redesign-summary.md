# SkuTrak knowledge base redesign

## How it used to look

Our dashboard guides followed a standard help doc format:

1. **Title and one-line description** ("Learn how to use the Top Line Report dashboard")
2. **Summary** with bullet points covering what the dashboard does
3. **Screenshot** of the dashboard
4. **Configuration instructions** listing each toolbar control with its default value
5. **What's on screen** describing each visual component in a sentence or two

The structure was functional but it read like a manual. It told users what buttons do. It didn't tell them why they should care, when to open the dashboard, or what to actually do with what they see.

Users opened the guide, scanned it once, and rarely came back because it didn't help them make better decisions. It helped them find a button.

## How it looks now

Every dashboard guide follows the same structure:

1. **One-sentence intro** that frames the dashboard's purpose in terms of the question it answers
2. **Screenshot** so users immediately recognise the page
3. **Video walkthrough** embedded directly, showing the dashboard in action
4. **Why it matters** with tabs for each role (Account Managers see one thing, Supply Chain Analysts see another)
5. **When to use it** as a table mapping real triggers (Monday check-in, before a buyer meeting, when an alert fires) to what you're checking
6. **What to look for** as expandable accordions describing patterns, not features (e.g. "Sales declining but availability stable" means it's a demand problem, not a supply problem)
7. **How to read it** as a numbered sequence giving users a repeatable 60-second workflow
8. **Dashboard controls** as cards explaining each setting
9. **What's on screen** as cards describing each visual panel and what to focus on
10. **Quick reference** table defining every metric in plain language
11. **Next steps** linking to the logical next dashboard

## Why we changed it

**The old guides described the interface. The new guides teach users how to think.**

Three principles drove the redesign:

### 1. Why before how

Most knowledge bases jump straight to "click here, select this". We lead with why the dashboard matters for your specific role. If a user doesn't understand why they should care, instructions on which dropdown to use are irrelevant.

### 2. Pattern recognition over feature description

The "What to look for" section is the biggest change. Instead of listing metrics and filters, we describe what combinations of metrics actually mean:

- Sales down + availability stable = demand problem, not supply
- DC inbound falling + store inbound stable = you have 1-2 weeks before shelf gaps
- Sales growth exceeding rate of sale growth = distribution gains, evidence for range expansion

This turns the knowledge base from a reference manual into a diagnostic tool. Users don't just learn what the dashboard shows. They learn how to interpret it.

### 3. Role-based context

An Account Manager and a Supply Chain Analyst look at the same dashboard for completely different reasons. The old guides treated all users the same. The new guides use tabs to give each role their specific context, so nobody has to wade through information that isn't relevant to them.

## What this means in practice

- Users have a reason to bookmark and revisit these guides because they help with real decisions
- New starters can ramp faster because the guides teach them how experienced users actually read the dashboards
- Every page cross-links to the next logical dashboard, keeping users in the knowledge base instead of getting stuck on one page
- The consistent structure means once you've read one guide, you know how to navigate all of them

## Pages live now

| Dashboard | What it covers |
|-----------|---------------|
| Top Line Report | Weekly account health, overall performance vs previous periods |
| Sales Report | SKU-level sales detail, rate of sale, range review preparation |
| Availability Report | Store-level on-shelf tracking, gap analysis, lost sales |
| Depot Stock | DC stock levels, weeks of cover, supply early warning |
| Commercial Alerts | Automated flags for sales drops, availability declines, supply issues |
