# structured-analysis

A Claude skill for analyzing a topic's **background** (how it came to be) and **future** (where it might go), using eight structured analytic frames drawn from intelligence tradecraft.

Built for people who need analysis with actual depth — researchers, analysts, journalists, strategists — and who are tired of watching AI produce five-bullet summaries in place of thinking.

---

## What this does

You bring a topic. The skill picks the right frames for the question, states its selection out loud so you can override, then runs the frames to depth with required structural output — not free-form bullets.

The default is **two frames, deep**, not five frames, shallow.

Each frame comes with a built-in steel man (the strongest counter-reading to what was just produced) and a source quality note (weak-source claims, unverified assumptions, currency risk).

---

## The eight frames

**Backward-looking — how did we get here**
1. **Genealogy** — critical junctures that locked in today's configuration
2. **Actor Mapping** — who wants what, stated vs revealed interests, coalitions
3. **Red Team** — the situation through the analyzed actor's eyes
4. **Structural (STEEP)** — social / technological / economic / environmental / political pressures
5. **Key Assumptions Check** — what must be true for the current reading to hold

**Forward-looking — where might it go**

6. **Scenario 2x2** — plausible futures with observable signposts
7. **Second-Order Effects** — consequences of consequences, out to third order
8. **ACH / Pre-Mortem / What-If** — competing-hypothesis test, failure walkback, or shock scenario

Frames combine. The skill picks pairs by question type — an actor's move gets Actor Mapping + Red Team; a systemic shift gets Genealogy + Scenario 2x2; a contested reading gets ACH + Key Assumptions Check.

---

## When it fits

- *"Why is X moving now?"*
- *"How did we get to this configuration?"*
- *"What might happen if Y decides Z?"*
- *"Whose reading of this holds up?"*
- *"What's the analysis missing?"*

## When it doesn't

- Quick factual lookups
- Generic SWOT-style strategy templates
- Opinion pieces / hot takes
- Anything you already know the answer to

---

## Install

### claude.ai (web / desktop app)

1. Download the latest release ZIP from the [Releases](../../releases) page.
2. In claude.ai, go to **Settings → Capabilities → Skills** (or **Customize → Skills**, depending on your client version).
3. Click **Upload skill** and select the ZIP.

Requires a paid Claude plan.

### Claude Code

Clone the repo and symlink the skill folder:

```bash
git clone https://github.com/bushrabeg/structured-analysis.git ~/skills/structured-analysis
ln -s ~/skills/structured-analysis ~/.claude/skills/structured-analysis
```

To update: `git pull` inside the cloned repo. The symlink picks up changes.

---

## Usage

The skill triggers automatically when your message signals background or future analysis of a topic. You don't need to invoke it by name.

**Explicit frame:**
> "Run a red team on Ankara's Syria policy shift."

**Trigger phrase:**
> "What's behind the recent uranium enrichment push in Iran?"
> → Skill picks Genealogy (triggered by "what's behind"), states its selection, invites additions, proceeds.

**No signal — default match:**
> "Analyze the semiconductor decoupling."
> → Skill reads the topic as a systemic shift, picks Genealogy + Scenario 2x2, states its selection, proceeds.

**Override count or direction:**
> "Just the background — three angles."
> → Skill runs three backward-looking frames.

**Override the reflex:**
> "Skip the steel man on this one."
> → Steel man omitted; source note stays.

### What every run looks like

Before analysis begins, the skill outputs one line:

> *For this topic I've selected: **Genealogy** + **Scenario 2x2**. Add another or swap — otherwise I'm starting.*

This is a transparency beat, not a permission request. Silence or "go" means proceed. An addition or swap redirects.

---

## Extending to other languages

The bilingual trigger dictionary in `SKILL.md` has two columns — English and Turkish. Add your own by appending a column with the same rows. The skill will match user phrases in your language to the right frame.

Pull requests welcome for additional languages.

---

## Origins

The eight frames draw from **Structured Analytic Techniques (SATs)** developed in the U.S. intelligence community and codified in the Kent School tradition — particularly Richards Heuer's *Psychology of Intelligence Analysis* and *Structured Analytic Techniques for Intelligence Analysis* (Heuer & Pherson).

Analysis of Competing Hypotheses, Key Assumptions Check, Red Team, and Pre-Mortem come directly from that tradition. Genealogy borrows from Foucauldian historical method. STEEP is standard futures-studies scaffolding. Scenario 2x2 is Shell / Global Business Network. Second-order effects and What-If are from strategic foresight practice.

This skill's contribution is not the frames themselves — it's the packaging: enforcing depth via required output sections, defaulting to a paired-frame minimum, and making frame selection transparent so the user stays in control.

---

## Contributing

Issues and pull requests welcome, especially:

- Additional language trigger dictionaries
- Topic types the default-match table doesn't cover
- Failure modes worth adding to the anti-patterns list
- Sharper phrasing anywhere the current text feels bureaucratic

Please keep the two-frame default and the transparency beat — those are load-bearing design choices, not decoration.

---

## License

MIT. Use it, fork it, adapt it, ship your own version.
