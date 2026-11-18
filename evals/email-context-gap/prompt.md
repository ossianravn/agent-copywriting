---
max_turns: 25
timeout_seconds: 900
allowed_tools: [Read, Glob, Grep, Skill, Agent]
---

We've been going back and forth on this all week. Here are my notes. Can you write the email to our customers?

- Decided Tuesday: we go with Option B. (Option A meant keeping the old PDF export, too costly. Lars pushed for B.)
- The "v2 flow": an invoice is sent automatically as soon as a job is marked complete in the app. Today the user has to press "Send invoice" on the Invoices tab.
- Goes live Monday 1 March 2027 for all accounts.
- Anyone who wants to keep sending by hand can turn auto-send off under Settings > Invoicing. It is on by default.
- The Hansen fix ships in the same release (the rounding bug Hansen & Søn reported). VAT is now rounded per line instead of per invoice, so totals can differ by a few øre from before.
- Phase 2 (payment reminders) is planned for Q3.
- The migration script ran fine on staging, 14k accounts.
- Support: support@fakturo.example

The product is Fakturo. The readers are small trades businesses that use it for invoicing.
