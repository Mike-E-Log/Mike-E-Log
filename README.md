<h2 align="center">Mike Ilog · AI Engineer</h2>

<p align="center">
  <em>I build and evaluate AI to make products work.</em>
</p>

---

### Selected work

**[GG Tank Watch](https://github.com/Mike-E-Log/gg-tank-watch)** is a civic emergency archive I built during a real May 2026 chemical-tank evacuation (~50,000 residents; [Wikipedia](https://en.wikipedia.org/wiki/Garden_Grove_chemical_leak), [NPR](https://www.npr.org/2026/05/24/nx-s1-5833165/california-chemical-tank-malfunction-leak-explode-emergency-evacuate)). While it ran, an LLM (Claude, with web search) summarized official and news updates every 30 minutes. A consumer-facing AI system held inside its authority by code and tests, not prompting:

- **What if the AI got something wrong?** The design assumed it would. The AI only wrote drafts — a separate, tested program checked every one and controlled what reached the page. And the page never told people what to do: at most, it pointed readers to official sources.
- **The asymmetry that matters.** A false all-clear is catastrophic; a false alarm is survivable. So danger *downgrades* need ≥2 sources (including an official agency), while *upgrades* fire on one. Enforced in code, never asked of a model.
- **A [behavioral harness of 200+ tests](https://github.com/Mike-E-Log/gg-tank-watch/actions/workflows/eval.yml)** — green in CI — catches drift from the safety contract (fabricated sources, authored directives, stale data) before it ships, not after.

> **Live archive** → [ggtankwatch.org](https://ggtankwatch.org)
>
> **Code** → [gg-tank-watch](https://github.com/Mike-E-Log/gg-tank-watch)
>
> **Safety method & red-team evidence** → [gg-tank-watch-method](https://github.com/Mike-E-Log/gg-tank-watch-method)

**[Business Scenario Judge](https://github.com/Mike-E-Log/business-scenario-judge)** — a method study: can you trust an AI judge to grade another AI? I blind-graded 60 real service chats in a labeling tool I built, calibrated an AI judge on my rulings, and measured it against an uncalibrated judge on held-out chats — every ruling committed, all the math re-runnable by anyone, the honest result up front.

---

### Writing

Three essays on AI evaluation, from practice — [mikeilog.com/writing](https://www.mikeilog.com/writing):

- **[What building an emergency dashboard taught me about trustworthy AI](https://www.mikeilog.com/writing/emergency-dashboard-trustworthy-ai/)** — the GG Tank Watch story: five lessons about AI you can trust.
- **[What AAA QA teaches about AI evaluation](https://www.mikeilog.com/writing/aaa-qa-teaches-ai-evaluation/)** — Square Enix QA as a multi-agent evaluation system before anyone called it that.
- **[Human-in-the-loop eval and the part you can't ask about](https://www.mikeilog.com/writing/human-in-the-loop-subjective-eval/)** — what a real human-in-the-loop looks like, and when the honest move is to cut the feature.

---

### Contributions

**Open**

- **[gstack](https://github.com/garrytan/gstack)** security fix [#1822](https://github.com/garrytan/gstack/pull/1822): withholds the localhost auth token from content-script `getPort` callers
- **[Claude Code](https://github.com/anthropics/claude-code)**
  - Reported and diagnosed [session-bloat bug #61613](https://github.com/anthropics/claude-code/issues/61613) in the Read tool's binary-file serialization path (root cause + fix sketch)
  - Added a reproduction, render-only proof, and fix direction to [scrollback-duplication #51828](https://github.com/anthropics/claude-code/issues/51828#issuecomment-4567557135)

**Merged**

- **[gstack](https://github.com/garrytan/gstack)** PR [#1554](https://github.com/garrytan/gstack/pull/1554): fix shipped in squash commit [7ca04d8](https://github.com/garrytan/gstack/commit/7ca04d8ef03db07764bef66c4252bf7a1699ffec), credited in the v1.42.0.0 release wave ([#1594](https://github.com/garrytan/gstack/pull/1594))

---

### Tools & methods

- **Building AI agents:** Claude Agent SDK, MCP, Anthropic SDK
- **Languages:** Python, TypeScript

<sub>I pick up new domains fast; everything is language.</sub>

---

### Contact

- **LinkedIn** → [https://www.linkedin.com/in/mikeilog](https://www.linkedin.com/in/mikeilog)
- **Email** → [mike@mikeilog.com](mailto:mike@mikeilog.com)

<sub>cooperation FTW · US (Pacific time) · remote</sub>
