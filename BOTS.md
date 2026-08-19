# Bots of IT  (docx S5 candidate menu)

These are the **Major sub-functions** of IT from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 7.

- `infrastructure` — **Infrastructure**  ·  titles: CIO, VP IT, IT Director, IT Operations Manager, Systems Administrator, IT Support Manager, IT Governance Manager
- `enterprise-applications` — **Enterprise Applications**  ·  titles: CIO, VP IT, IT Director, IT Operations Manager, Systems Administrator, IT Support Manager, IT Governance Manager
- `internal-support` — **Internal Support**  ·  titles: CIO, VP IT, IT Director, IT Operations Manager, Systems Administrator, IT Support Manager, IT Governance Manager
- `identity-access` — **Identity & Access**  ·  titles: CIO, VP IT, IT Director, IT Operations Manager, Systems Administrator, IT Support Manager, IT Governance Manager
- `systems-administration` — **Systems Administration**  ·  titles: CIO, VP IT, IT Director, IT Operations Manager, Systems Administrator, IT Support Manager, IT Governance Manager
- `it-operations` — **IT Operations**  ·  titles: CIO, VP IT, IT Director, IT Operations Manager, Systems Administrator, IT Support Manager, IT Governance Manager
- `it-governance` — **IT Governance**  ·  titles: CIO, VP IT, IT Director, IT Operations Manager, Systems Administrator, IT Support Manager, IT Governance Manager
