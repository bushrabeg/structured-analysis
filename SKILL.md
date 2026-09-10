---
name: structured-analysis
description: Analyze a topic's background and future using structured analytic techniques drawn from intelligence tradecraft — genealogy, actor mapping, red team, STEEP, key assumptions check, scenario 2x2, second-order effects, and ACH/pre-mortem/what-if. Load when the user asks to unpack how something came to be, why an actor is moving now, what structural forces drive a situation, what might happen next, what could go wrong, or which of several competing readings holds. Not for quick factual lookups, generic SWOT-style strategy templates, or opinion pieces.
---

# Structured Analysis

Eight analytic frames for reasoning about a topic's **background** (how it came to be) and **future** (where it might go). Each frame is a discipline, not a template. The skill's job is to pick the right frame for the question, run it to depth, and refuse to produce shallow bullet-list output.

## Core principle

Most analysis fails in one of three ways: it stays on the surface (bullets without causal chain), it hides its assumptions (confident forecast built on unexamined ground), or it treats one perspective as objective (blind to how the other side reads the same facts). The eight frames each attack one of those failure modes. Use them singly or in combination — never all at once.

## Decision flow — how to pick frames

Follow this order every time. Do not skip step 3.

**1. Explicit override.** If the user names a frame, a count, or a direction, obey it and skip to step 3.
- Frame named: *"run a red team on this"*, *"do a genealogy"*
- Count: *"one frame only"*, *"two angles"*, *"go deep with three"*
- Direction: *"just the background"* → backward-looking frames only (1–5) / *"just the future"* → forward-looking frames only (6–8)

**2. Trigger phrase in the user's message.** Check the trigger dictionary at the bottom of this file. If one or more phrases match, select those frames.

**3. No signal → default match.** Read the topic, match it to the topic-type table below, pick the paired frames.

**4. State the selection and invite additions. Then wait.**

Every run, before analysis begins, output exactly one line in this shape:

> *"For this topic I've selected: **[Frame A]** + **[Frame B]**. Add another or swap — otherwise I'm starting."*

Then stop. If the user replies with an addition or swap, apply it. If the user replies with anything else (including "go", "yes", "ok", or a follow-up question), start the analysis.

This is not permission-asking. It is a transparency beat. Do not ask "shall I proceed?" or "does this look right?" — the invitation is enough.

**5. Default depth is two frames.** Not one, not five. Two frames run to depth beats five frames run shallow. Expand only when the user says *"go deeper"*, *"three angles"*, *"more frames"* or similar.

## The eight frames

Frames 1–5 are backward-looking (how did we get here). Frames 6–8 are forward-looking (where might it go). The line between them is porous — genealogy sets up scenario work, second-order effects loops back into structural analysis.

---

### 1. Genealogy

**Asks:** How did we get here? Which critical junctures locked in today's configuration, and what alternatives were foreclosed?

**When it fits:** Systemic change, institutional inertia, path-dependent outcomes, "why is X still with us" questions, discourse/legitimacy analysis.

**How to run:**
1. Identify the phenomenon under analysis in its current form. State it in one sentence.
2. Walk backward through **at least three critical junctures** — moments where a different choice would have produced a materially different present. For each juncture: what was the choice, who made it, what was the alternative, why was that alternative foreclosed.
3. Name the **discursive / institutional / material inheritance** each juncture bequeathed. What must be true today because of what happened then.
4. End with the question: *what would need to change for this configuration to become contingent again?*

**Required output sections:**
- Present configuration (1 sentence)
- Critical junctures (minimum 3, chronological)
- Inheritance mapping (what is locked in and why)
- Contingency test (what would loosen it)

**Failure modes to avoid:**
- History-as-narration — telling the story instead of showing the junctures
- Presentism — treating today's outcome as inevitable
- Actor-blindness — critical junctures were choices, not weather

---

### 2. Actor Mapping

**Asks:** Who are the players, what do they want, who is aligned with whom, and who has recently gained or lost?

**When it fits:** Political moves, negotiations, coalition dynamics, "why now" questions about a specific actor's behavior.

**How to run:**
1. List the relevant actors. Include off-stage actors (bureaucracies, factions inside a state, non-state financiers) not just the visible ones.
2. For each actor: **stated interest** vs **revealed interest** (what their behavior implies, which may differ from what they say). Note the gap.
3. Map coalitions and antagonisms. Who benefits from whose success. Who has veto power.
4. Identify recent shifts — who moved up, who moved down, who was displaced.
5. Optional mini-position snapshot for a key actor: leverage / vulnerability / current opening / current constraint. (This replaces standalone SWOT.)

**Required output sections:**
- Actor list with stated vs revealed interest
- Coalition / antagonism map
- Recent shifts (last 6–24 months)
- Position snapshot for the pivotal actor(s)

**Failure modes to avoid:**
- Listing only the loudest actors
- Taking stated interests at face value
- Treating states as unitary — internal factions matter

---

### 3. Red Team

**Asks:** How does the situation look through the eyes of the actor being analyzed — using their categories, their fears, their read of you?

**When it fits:** Adversary behavior, negotiation preparation, breaking mirror-imaging, testing whether a policy will be read the way its designers intend.

**How to run:**
1. Choose the actor whose mind you are entering. Name them explicitly.
2. Reconstruct their **worldview inputs**: what information do they have, what history shapes their reflexes, what domestic constraints do they carry, what do they think you think.
3. Rewrite the situation from inside that worldview. Not "what they claim to think" but what the situation *looks like* when you have their categories.
4. Identify at least two **reading gaps** — points where their perception of the situation diverges from yours. Which side's reading is closer to reality is not the question; the divergence itself is the finding.
5. Name what they would consider a provocation, a concession, a victory, a humiliation.

**Required output sections:**
- Actor and worldview inputs
- Situation as they see it
- Reading gaps (minimum 2)
- Symbolic register (provocation / concession / victory / humiliation)

**Failure modes to avoid:**
- Caricature — projecting your assumptions onto them
- Rational-actor flattening — they are not maximizing utility, they are navigating internal politics
- Ignoring domestic constraints on the leader

---

### 4. Structural (STEEP)

**Asks:** What structural forces — beyond the choices of any single actor — are pressing on this situation?

**When it fits:** Big-frame questions ("what is happening in this region"), technology-driven change, longue durée shifts, questions where personalities distract from tectonics.

**How to run:**
Walk through five layers. For each, name the specific pressure operating on the topic, not a generic description of the layer.

- **Social** — demographic, cultural, generational shifts. Who is moving, aging, leaving, radicalizing, secularizing.
- **Technological** — capability shifts, cost curves, adoption thresholds. What is now possible that was not.
- **Economic** — debt, trade, resource, monetary dynamics. Who is being squeezed, who has slack.
- **Environmental** — resource stress, climate impacts, ecological carrying capacity. Physical constraints.
- **Political** — regime type shifts, legitimacy, coalition stability, sovereignty erosion or consolidation.

At the end, identify **which two layers are the load-bearing ones** for this specific topic. Not all five carry equal weight; naming the dominant ones is the analytic move.

**Required output sections:**
- Five-layer walk (specific pressure per layer)
- Load-bearing layers named
- Cross-layer interaction — where two pressures compound

**Failure modes to avoid:**
- Generic descriptions ("technology is changing") instead of specific pressures
- Treating layers as independent — they interact
- Skipping a layer because it seems obviously irrelevant; make the negative finding explicit

---

### 5. Key Assumptions Check

**Asks:** What must be true for our current reading to hold, and what would falsify it?

**When it fits:** Before committing to a forecast, when confidence feels too easy, when the analysis has been running unchallenged for a while, when the topic touches your priors.

**How to run:**
1. State the working analysis in one paragraph.
2. Extract every **implicit assumption** it rests on. Aim for at least six. Assumptions are usually invisible until named — this is the whole discipline.
3. Sort assumptions into three buckets:
   - **Solid** — well-supported, would take a major shift to break
   - **Supported but fragile** — currently true but structurally exposed
   - **Unexamined** — you don't actually know if this holds, you assumed
4. For each fragile or unexamined assumption, write the **falsification condition**: what specific observation would tell you it broke.

**Required output sections:**
- Working analysis (one paragraph restatement)
- Assumption inventory (minimum 6, bucketed)
- Falsification conditions for fragile/unexamined assumptions

**Failure modes to avoid:**
- Listing only assumptions you already know are safe
- Making assumptions too general to be falsifiable
- Treating this as a formality rather than the point

---

### 6. Scenario 2x2 (with Signposts)

**Asks:** Given deep uncertainty, what are the plausible futures — and what would tell us which one is arriving?

**When it fits:** Forecasting under uncertainty, strategic planning, "5 years from now" questions, situations where a single prediction would be dishonest.

**How to run:**
1. Identify the **two critical uncertainties** — the axes along which the future genuinely could go different ways. Not variables you already know how to bet on; variables where you would take even odds.
2. Cross them into a 2x2. Label each quadrant with a short name (a single word or short phrase evoking the world).
3. For each of the four quadrants, describe the world in one paragraph: what has happened, who has adapted, what is normal now.
4. **Signposts (required, do not skip):** For each quadrant, list **three concrete signals** that would indicate this scenario is the one arriving. Signposts must be observable and specific — a policy announcement, a threshold crossed, a defection, a market move. Not vibes.

**Required output sections:**
- Two critical uncertainties (named and defended)
- Four quadrants named + one paragraph each
- Three signposts per quadrant

**Failure modes to avoid:**
- Uncertainties that aren't actually uncertain (you know which way they'll break)
- Four scenarios that are actually variations of one scenario
- Vague signposts ("tensions rise") that can't be checked against reality

---

### 7. Second-Order Effects

**Asks:** What are the consequences of the consequences? Whose adaptations to the first-order change reshape the situation?

**When it fits:** New technology, policy change, market shock, any question where the obvious effect is not the interesting one.

**How to run:**
1. State the first-order effect. What directly changes.
2. Identify the actors who must adapt to that change. For each, ask: what is their response and what does that response do to the system?
3. Walk to at least **third-order**: the response to the response. This is where most analysis stops too early.
4. Name **counter-adaptations** — the moves that neutralize or invert the initial change.
5. End with the **unexpected outcome** that emerges from the chain — the finding that would not be visible from the first-order effect alone.

**Required output sections:**
- First-order effect
- Second-order (adaptations)
- Third-order (adaptations to adaptations)
- Counter-adaptations
- Emergent unexpected outcome

**Failure modes to avoid:**
- Stopping at second-order and calling it done
- Linear chain thinking — the effects loop and interact
- Treating adaptation as passive; actors will move to protect their positions

---

### 8. ACH / Pre-Mortem / What-If

Three sub-frames. Pick one — they attack different questions.

#### 8a. ACH — Analysis of Competing Hypotheses

**Asks:** Given the evidence, which hypothesis survives falsification best?

**When it fits:** Contested readings, ambiguous evidence, situations where several explanations are floating and you need to discipline the choice.

**How to run:**
1. List **at least three competing hypotheses**. Not straw versions — the strongest form of each.
2. List the key pieces of evidence. Aim for at least six.
3. For each evidence item, mark whether it is **consistent (C), inconsistent (I), or ambiguous (A)** with each hypothesis. Diagnostic evidence — evidence that is C with one and I with another — is worth more than consistent-with-everything evidence.
4. The winning hypothesis is not the one with the most consistent evidence. It is the one with the **fewest inconsistent** items. This inversion is the whole point of ACH.
5. State the **conditions under which the leading hypothesis would fall**.

**Required output:**
- Hypotheses (min 3)
- Evidence inventory (min 6)
- Matrix (C/I/A per cell)
- Leading hypothesis + falsification condition

#### 8b. Pre-Mortem

**Asks:** Assume this failed. What did we miss?

**When it fits:** Strategy stress-testing, plans that feel too tidy, decisions in progress, identifying blind spots.

**How to run:**
1. Fast-forward to the point of failure. State the failure in concrete terms (not "it didn't work" — *what specifically broke*).
2. Walk backward through the causes. Aim for at least four distinct causes.
3. For each cause, name the **early warning sign** that would have been visible in the present if you were looking.
4. End with the **detection gap** — why weren't these signs being looked for now.

**Required output:**
- Concrete failure state
- Cause chain (min 4)
- Early warning signs
- Detection gap

#### 8c. What-If

**Asks:** What if a low-probability, high-impact shock hits — what breaks, what emerges?

**When it fits:** Black-swan disciplining, resilience testing, breaking the tyranny of expected outcomes.

**How to run:**
1. Name the shock. It must be **low-probability by consensus but not impossible**. State the trigger event.
2. Trace immediate breaks — what depends on the pre-shock state and no longer works.
3. Trace adaptations — who improvises, who freezes, who profits.
4. Identify the **new equilibrium** that emerges, if any. Sometimes there isn't one; naming that is a valid finding.

**Required output:**
- Shock event (specific)
- Immediate breaks
- Adaptations
- New equilibrium (or absence)

---

## Reflexes (append to every frame's output)

Both of these run automatically at the end of every frame's output, no matter which frame ran. The user can suppress either with an explicit command (see trigger dictionary), but the default is on.

### Steel Man

A one-paragraph statement of the **strongest counter-reading** to the analysis just produced. Not "on the other hand"-style hedging — an actual best-case version of the opposite view. If the analysis argued X, this paragraph argues not-X in its most defensible form.

### Source Quality Note

A short block flagging:
- **Weak-source claims** — assertions in the analysis that rest on thin, single-source, or motivated evidence
- **Unverified assumptions** — factual premises taken for granted that should be checked
- **Currency risk** — points where the analysis depends on facts that may have changed

Format: three short bullet lines or "none flagged" if truly clean.

---

## Bilingual trigger dictionary

Matches user phrasing to frame selection. Users of other languages can add their own column by cloning the pattern.

| Frame | English triggers | Türkçe tetikleyiciler |
|---|---|---|
| **Genealogy** | how did we get here, what's behind this, where does this come from, historical development, path to today | bunun arkasında ne var, nasıl buraya geldik, kökeni ne, tarihsel olarak nasıl gelişti, hangi kavşakta bugüne kilitlendi |
| **Actor Mapping** | who wants what, whose interests, players, coalitions, who won/lost | kim ne kazandı / kim ne kaybetti, kimin çıkarı ne, aktörleri çıkar, koalisyonlar, sahnede kim var arkada kim var |
| **Red Team** | through their eyes, from their side, how do they read this, put yourself in X's shoes | X'in gözünden bak, X yerinde olsan, onlar bunu nasıl okuyor, karşı taraftan nasıl görünüyor |
| **Structural (STEEP)** | structural forces, macro dynamics, what's shifting underneath, systemic pressures | yapısal olarak ne oluyor, hangi zemin kayıyor, arka plandaki basınçlar, makro dinamikler, kişilerden bağımsız ne var |
| **Key Assumptions Check** | what are we assuming, what's the analysis resting on, what would break this reading | hangi varsayımlara dayanıyoruz, neyi sorgulamadan geçtik, ne olursa bu okuma çöker, temel kabuller ne |
| **Scenario 2x2** | possible futures, what might happen, scenarios, 5 years out | olası dünyalar, olası gelecekler, senaryoları çıkar, belirsizlik ekseni ne, 5 yıl sonra ne olur |
| **Second-Order** | then what, downstream effects, consequences of consequences, ripple | sonra ne olur, zincirleme etki, asıl sonuç ilk sonuç değil, bunun sonucunun sonucu |
| **ACH** | which hypothesis holds, competing readings, test the interpretations | hangi hipotez daha güçlü, kanıtları hipotezlere karşı test et, rakip yorumlar |
| **Pre-Mortem** | what could go wrong, blind spots, imagine it failed, how does this break | ya çuvallarsa, bu iş nasıl patlar, kör noktalar, 5 yıl sonra çöktü diye baksak sebep ne |
| **What-If** | what if X happens, black swan, low-probability shock | ya X ölürse, beklenmedik ama etkili, black swan, düşük olasılıklı yüksek etkili |
| **Depth override** | go deeper, three angles, more frames | derinleş, üç açıdan, daha fazla çerçeve |
| **Speed override** | quick take, one frame, short | hızlı bak, kısa bak, tek çerçeveyle |
| **Direction override** | just background / just future | sadece arka plan / sadece gelecek |
| **Reflex suppression** | skip steel man / skip source note | steel man'e gerek yok / kaynak notu koyma |

---

## Topic-type → default frame map

Used only when no override and no trigger phrase apply. Pick the paired frames; then apply step 4 of the decision flow (state selection, invite additions, wait one beat, proceed).

| Topic type | Default frames |
|---|---|
| Systemic shift / hegemonic change | Genealogy + Scenario 2x2 |
| Actor move ("why is X doing this now") | Actor Mapping + Red Team |
| New technology / disruptive capability | Second-Order + STEEP |
| Uncertain future / decision under uncertainty | Scenario 2x2 + What-If |
| Institutional or strategic failure | Pre-Mortem + Actor Mapping |
| Contested reading / evidence dispute | ACH + Key Assumptions Check |
| Policy / strategy design | Red Team + Second-Order |
| Discourse / legitimacy analysis | Genealogy + Actor Mapping |

If the topic straddles two rows, pick the row that matches the *question the user is actually asking*, not the topic in the abstract.

---

## Output structure (every run)

```
[One-line selection statement — Frame A + Frame B, invite additions]

[USER RESPONDS — proceed if any signal to start, apply if addition/swap]

## [Frame A name]
[Full frame output following that frame's required sections]

**Steel man:** [one paragraph]

**Source quality note:**
- [bullet]
- [bullet]
- [bullet]

## [Frame B name]
[Full frame output following that frame's required sections]

**Steel man:** [one paragraph]

**Source quality note:**
- [bullet]
- [bullet]
- [bullet]

## Cross-frame synthesis
[Only if the two frames produced findings that interact. One paragraph. If they don't interact, skip this section — do not manufacture synthesis.]
```

---

## Anti-patterns — what this skill refuses to produce

- **Bullet-list surface analysis.** Every frame has required sections with structural demands. Producing five bullets under a frame heading is not running the frame.
- **Actor-less structural analysis.** Structural pressures are exercised by actors making choices. A STEEP walk that describes "forces" with no agents in them is incomplete.
- **Overconfident forecasts.** Every forward-looking frame carries uncertainty; if the output reads like prophecy, Key Assumptions Check was skipped.
- **Consensus-flattering conclusions.** If the steel man reads weaker than the main argument, the steel man is not doing its job — rewrite it.
- **Frame theater.** Running five frames badly is worse than running one well. Two frames, deep, is the default for a reason.
- **Fake synthesis.** Do not paper over the seams between frames with a "putting it all together" section unless the frames genuinely produced findings that talk to each other.
