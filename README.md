# Blockchain Developer Roadmap — Cyfrin Updraft, 1hr/day

**Start date:** _fill in today's date_
**Cadence:** 1 hour/day, no zero days
**Goal track:** Solidity Smart Contract Developer (Cyfrin Updraft)

> Course names/order can shift on Updraft — check `updraft.cyfrin.io/courses` before each phase and adjust the checklist below if a module's been renamed or reordered. Treat the hour estimates as rough pacing, not a hard contract.

---

## Phase 0 — Setup (Day 1, ~1 hr)
- [ ] Create GitHub repo `blockchain-dev-log` (structure below)
- [ ] Install: Git, Node.js, VS Code (+ Solidity extension), MetaMask browser extension
- [ ] Create an Updraft account, bookmark the course dashboard
- [ ] Skim the "Career Tracks" page and confirm **Solidity Smart Contract Developer** is still the right track for you

## Phase 1 — Blockchain Basics (~Week 1)
Covers wallets, gas, consensus, how chains actually work. Ends in a proficiency exam.
- [ ] Complete Blockchain Basics course
- [ ] Pass the proficiency exam
- [ ] Commit: notes on the 5 concepts you understood least well going in

## Phase 2 — Solidity Fundamentals (~Weeks 2–5)
Core language + Remix IDE. This is where daily coding-along starts.
- [ ] Solidity syntax, types, functions, storage vs. memory
- [ ] Write & deploy your first contracts in Remix (simple storage, a "fund me" style contract)
- [ ] Intro to testing contracts
- [ ] Mini-project: a small contract of your own design (not from the tutorial) — e.g. a tip jar, a simple voting contract

## Phase 3 — Foundry & Tooling (~Weeks 6–8)
Move off Remix into a real dev workflow — this is what production Solidity devs actually use.
- [ ] Foundry setup (forge, cast, anvil)
- [ ] Rewrite one of your Phase 2 contracts in Foundry with proper tests
- [ ] Scripting deployments, environment config, testnets (Sepolia)
- [ ] Mini-project: deploy a contract to Sepolia testnet, verify it on Etherscan

## Phase 4 — Intermediate Solidity / DeFi primitives (~Weeks 9–12)
- [ ] ERC-20 tokens — build your own
- [ ] Oracles (Chainlink price feeds) — common real-world pattern
- [ ] Intro to an existing protocol's mechanics (Updraft's Uniswap/DeFi modules)
- [ ] Mini-project: a small DeFi-flavored contract (staking, simple lending, or a token with a price-feed-based feature)

## Phase 5 — Security basics (ongoing, light touch)
Even as a developer, auditing literacy is a strong differentiator.
- [ ] Common vulnerability classes (reentrancy, overflow, access control bugs)
- [ ] Review 2–3 known historical exploit writeups
- [ ] Optional: dip into Updraft's smart contract auditing intro material

## Phase 6 — Portfolio project (open-ended, after Phase 4)
- [ ] Design and ship one original project end-to-end: contracts + tests + testnet deploy + README with architecture notes
- [ ] This becomes your primary "look what I built" artifact for interviews

---

## GitHub Tracking System

### Repo structure
```
blockchain-dev-log/
├── README.md              # progress table + current streak, links to daily logs
├── daily-log/
│   ├── 2026-09-11.md       # one file per day: what you did, what confused you
│   └── ...
├── contracts/
│   ├── phase2-simple-storage/
│   ├── phase2-fund-me/
│   ├── phase3-foundry-fundme/
│   └── ...
└── notes/
    ├── solidity-syntax.md
    ├── foundry-cheatsheet.md
    └── ...
```

### Daily habit (keeps the graph green *and* actually teaches you something)
1. Watch/read the day's lesson segment (~40 min)
2. Type the code yourself — don't copy-paste (~15 min)
3. Commit: either new contract code, or a `daily-log/YYYY-MM-DD.md` entry summarizing what you learned in 2–3 sentences (~5 min)

A daily-log entry template:
```markdown
## 2026-09-11
**Phase:** 1 — Blockchain Basics
**Covered:** consensus mechanisms, gas mechanics
**Confusing bit:** EIP-1559 base fee vs priority fee
**Next:** finish wallets module
```

### README progress table (update weekly)
```markdown
| Phase | Status | Started | Finished |
|---|---|---|---|
| 0 — Setup | ✅ | 2026-09-11 | 2026-09-11 |
| 1 — Blockchain Basics | 🔄 | 2026-09-11 | — |
| 2 — Solidity Fundamentals | ⬜ | — | — |
| 3 — Foundry & Tooling | ⬜ | — | — |
| 4 — DeFi Primitives | ⬜ | — | — |
| 5 — Security Basics | ⬜ | — | — |
| 6 — Portfolio Project | ⬜ | — | — |
```

### Optional: GitHub Issues as a task board
Create one Issue per phase, checklist items as task-list items in the issue body, close it when the phase is done. Gives you a visible "Closed: 3" count and a changelog of when each phase actually wrapped.

---

## Effective-learning notes (the part that actually matters)

- **Type every line yourself.** Watching without typing is the single biggest reason tutorial-followers can't build anything afterward.
- **Explain it back in your own words** in the daily log — if you can't summarize a concept in 2 sentences, you didn't actually get it yet.
- **Don't skip the mini-projects.** Following a tutorial builds recognition, not recall. Building something *not* in the tutorial (even tiny) is what makes it stick.
- **5-minute warm-up:** before each session, skim yesterday's commit/code for a minute. Cheap spaced repetition.
- **Deploy to testnets early and often.** A contract that only exists in Remix's sandbox feels theoretical; one live on Sepolia with a real Etherscan link feels real — and it's a better portfolio artifact.
- **Use the Cyfrin Updraft Discord/community** when stuck rather than burning your 1 hour debugging alone — the hour budget is for learning, not for solo-stuck time.
- **Take the proficiency exams.** They're a real forcing function to check retention before you move on.
