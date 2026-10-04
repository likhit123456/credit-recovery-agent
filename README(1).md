# KhataVaani — AI Credit-Recovery Agent for Kirana Shops

> Speak the credit. KhataVaani brings the money home — politely, in every customer's language.

**Hack Sprint 2026 · MIT Bengaluru · Track T.04 Applied AI · PS 41 (Sarvam API)**

## The problem
India's 14 million+ kirana stores run on trust. Customers buy on credit ("udhaar"), but recovering it is manual (paper khata), awkward (asking a neighbour for money hurts the relationship) and stuck in one language. Cash that should run the shop stays locked up.

## The solution
KhataVaani is a voice-first AI agent that:

1. **Records** credit from a voice note in Kannada or Hindi ("Ramesh, 2 kg rice and oil, ₹180, Friday")
2. **Understands** it with Sarvam speech-to-text + LLM: customer, items, amount, due date
3. **Reminds** customers on the due date with a polite text + voice note in *their own* language
4. **Collects** through a one-tap UPI link, and updates the ledger automatically on payment
5. **Scores** each customer's repayment reliability and gives the owner a spoken daily summary

## Tech stack
| Layer | Tech |
|---|---|
| Frontend | Mobile-first PWA · HTML / CSS / JS |
| Backend | Python · FastAPI · APScheduler |
| Language AI | Sarvam AI: speech-to-text, translation, text-to-speech, LLM |
| Data | PostgreSQL |
| Payments | UPI intent links · Paytm webhook |
| Messaging | WhatsApp Business API / SMS |

All AI calls run server-side; API keys never reach the client.

## Status
Idea stage. The working build happens live during the 24-hour Hack Sprint (Oct 17–18, 2026).

## Team
Likhit
Taneev
Saiyam
Shashank
