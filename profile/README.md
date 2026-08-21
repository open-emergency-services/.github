# Open Emergency Services

**Free, open-source software for emergency services** — built to push back on the price-gouging that followed private-equity roll-ups of the software and systems that fire, EMS, and dispatch agencies depend on.

When the vendors got bought up and the cheaper options got killed off, the bill landed on small, mostly-volunteer departments least able to pay it. The response here is simple: build the core tools as open software, on open standards, under a rule that the code stays open, the data stays the agency's, and nobody can lock it up and resell it.

## The projects

| Repo | What it is | Scope |
|---|---|---|
| **open-fire-platform** | Fire records and federal incident reporting, built on NERIS — the U.S. federal *fire* incident standard (the EMS side is NEMSIS). The local database is the system of record, so the department always owns its data. | Fire-specific, on purpose |
| **open-p25-console** | An open dispatch console for P25 radio systems — so any agency can dispatch on its own radios without paying a recurring toll to a vendor for a core function on a published standard (CSSI). | All disciplines (fire, police, EMS) |

More pieces will split out under the same scheme as they mature — e.g. `open-mcptt` (push-to-talk over cellular), or the platform's reporting modules as `open-neris-reporting` / `open-nemsis-epcr`.

## The naming convention

Every repo is **`open-<what-it-is>`**: lowercase, hyphen-separated, descriptive, boring on purpose — so people find it by searching for exactly the thing. **Named by honest scope:** if a thing is discipline-specific, the name says so; if it's cross-discipline, the name doesn't pretend otherwise. Broaden at the umbrella level; keep each product honestly scoped.

## Shared rules across everything here

- **License: AGPLv3** — open, and specifically so no vendor can take it, close it, and resell it (the network-copyleft clause closes the "run it as a hosted service" loophole).
- **Public-service-first, anti-lock-in** — open standards, the agency owns its data, no paywalling core functions.
- **Honest, low-key** — solo/small maintainer for now; names and claims match what actually exists.
- **Independent repos, shared identity** — each piece stands alone technically but belongs to one family, and they're designed to integrate through clean interfaces (an event bus / gateway), not by living in one codebase.

## What this org is (and isn't)

A GitHub org is just a free namespace that holds repos. This one is **not** a legal entity, nonprofit, or foundation — no admin overhead, no fundraising, no board. Just a home for the code and a shared set of rules. If a formal structure is ever needed, that's a later decision made deliberately; it isn't one now.

---

*Early days, built in the open. If one of these tools would help your agency — or you want to help build it — the individual repos have the details.*
