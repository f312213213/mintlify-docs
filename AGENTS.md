# Documentation project instructions

This is the customer-facing documentation site for [JobBeacon](https://jobbeacon.app).

## About this project

- Built on [Mintlify](https://mintlify.com)
- Pages are MDX with YAML frontmatter
- Configuration in `docs.json`
- `mint dev` to preview, `mint broken-links` to verify

## Audience

End users — job seekers who want to be notified when companies post new roles. Not developers and not internal staff. Avoid implementation details, internal architecture, ATS-specific API quirks (unless they affect what the user sees).

## Terminology

- "Company" — what the user adds to their watchlist (not "site", "board", or "employer")
- "Job" or "role" — interchangeable
- "Filters" — the keyword and location rules per company
- "Notifications" — always means email (until other channels exist)
- "ATS" or "platform" — only when the user needs to know it (e.g., Workday quirks)
- Refer to ATS platforms by their brand name (Greenhouse, Workday, etc.) only when necessary

## Style

- Active voice, second person ("you")
- One idea per sentence
- Sentence case headings
- Bold for UI elements: Click **Add company**
- Code formatting for URLs, file paths, field names
- Avoid emoji in body copy
- Avoid marketing fluff ("powerful", "seamless", "world-class")

## Content boundaries

**Do document:**
- How to use any feature visible in the app
- What to expect (polling cadence, email format, limits)
- Troubleshooting common user-visible issues
- Plan differences and billing flow

**Don't document:**
- Internal architecture, database schema, deploy pipeline
- Specifics of how each ATS API works (it's an internal concern; only surface what affects the user)
- Future / roadmap features that aren't shipped
- Anything the user can't act on
