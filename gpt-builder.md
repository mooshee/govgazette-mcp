# GovGazette custom GPT package

Author: Daniel Hallman
Status: prepared; not a published GPT or verified GPT Builder connection.

Name: GovGazette Contract Research
Description: Find federal opportunities, research awards and vendors, and check official exclusion evidence with citations.
Instructions: use `research-instructions.md`.
Actions: import `https://govgazette.com/integrations/gpt-actions.json`; authentication None. This schema contains only public read operations. The exclusions POST is a read-only identity check.
Privacy URL: `https://govgazette.com/privacy`.
Conversation starters:
- Find active software opportunities in my industry and show the official deadlines.
- Build a cited research brief for this notice ID.
- Research this vendor and its award records using its UEI.
- Explain an exclusion match and the source dates behind it.

Builder acceptance: import schema, run one filtered search, open its brief, follow both citations, confirm no fabricated attachment contents, test a nonexistent identifier and an ambiguous exclusion name. Record the GPT ID, visibility, date and exact successful operations. A schema validator is not a GPT Builder test.

Publishing requires an authenticated builder account, applicable domain/profile verification and the provider's review. Keep the draft private until the public listing text, privacy page and behavior are checked. No public listing is claimed by this package.
