# Web App Security Journey

Personal learning log for mastering web application security — organized by
vulnerability class, not chronologically, so this repo doubles as a
reference library over time.

**Focus areas:** HTTP fundamentals → Access Control/IDOR → XSS → SQL
Injection → SSRF/Auth → independent methodology practice, with an eye
toward bug bounty work.

## ⚠️ Documentation policy

- No full flags, no complete step-by-step "solve this exact room" walkthroughs
  for paid/premium platform content (e.g. TryHackMe premium rooms). Flags are
  redacted (`THM{redacted}`); focus is on **methodology and reasoning**, not
  answers.
- PortSwigger Web Security Academy labs are public learning material and can
  be documented more openly, but the same "explain the why" discipline
  applies — this is a portfolio of thinking, not a copy of instructions.
- This repo is private for now. Will reassess going public once there's a
  consistent quality bar across writeups.

## Progress tracker

### Week 1 — HTTP & Web Fundamentals
**Status:** ⬜ Not started
**Goal:** Explain what's in a request/response without looking it up. Comfortable
intercepting/modifying traffic in Burp.
- [ ] PortSwigger: HTTP basics / sessions / cookies / same-origin policy
- [ ] Burp Suite Community installed & configured as browser proxy
- [ ] Practice: inspect real request/response pairs, cookies, headers
- Notes:

### Week 2 — Access Control & IDOR
**Status:** ⬜ Not started
**Goal:** Instinctively test ID/role/parameter boundaries in any app.
- [ ] PortSwigger: Access control vulnerabilities (all labs)
- [ ] THM: 1–2 rooms on broken access control
- Notes:

### Week 3 — Cross-Site Scripting (XSS)
**Status:** ⬜ Not started
**Goal:** Understand *why* a payload executes — reflected, stored, DOM-based.
- [ ] PortSwigger: full XSS topic
- [ ] Practice reading JS source for DOM sinks
- Notes:

### Week 4 — SQL Injection
**Status:** ⬜ Not started
**Goal:** Manually test for SQLi (incl. blind/time-based) before reaching for sqlmap.
- [ ] PortSwigger: SQLi topic, all labs
- Notes:

### Week 5 — SSRF + Authentication Flaws
**Status:** ⬜ Not started
**Goal:** Understand how internal trust assumptions get abused.
- [ ] PortSwigger: SSRF topic
- [ ] PortSwigger: Authentication topic
- Notes:

### Week 6 — Consolidation
**Status:** ⬜ Not started
**Goal:** Cold methodology pass on an unguided box/room + one polished writeup.
- [ ] Pick unguided THM/HTB target
- [ ] Apply recon checklist from `methodology/`
- [ ] Produce one full writeup start to finish
- Notes:

## Repo structure

```
websec-journey/
├── README.md
├── 01-http-fundamentals/
├── 02-access-control-idor/
├── 03-xss/
├── 04-sql-injection/
├── 05-ssrf-auth/
├── 06-consolidation/
└── methodology/
    └── recon-checklist.md
```

Each numbered folder holds writeups (one file per target/lab) using the
template in `methodology/writeup-template.md`.
