---
name: dnd-unbound-session-notes
description: "Skill that extracts a session transcript into session notes."
---

<!--
=============================================================================
SESSION NOTES TEMPLATE — The Unbound
=============================================================================
Use this template to transform a session transcript into session notes that
match the established campaign format. Inline guidance is in HTML comments
(invisible when rendered). Remove or keep sections based on what the session
actually contained — not every session has rituals, formal reports, or loot.
GENERAL PRINCIPLES
- Preserve proper nouns exactly as spoken: NPC names, place names, spell
  names, item names, faction names. When unsure of spelling, retain the
  phonetic form rather than guessing.
- Quote characters directly whenever a line is distinctive, especially Tomis,
  Grimbold, Uriel, Rowan, Freya, and notable NPCs. Correct minor disfluencies
  ("uh," restarts, mid-word self-corrections) but preserve word choice,
  rhythm, and meaning. Never paraphrase impactful dialogue into summary.
- Default voice for narrative recap: past tense, third person, restrained.
  Tomis's interior reflections, when included, are in his own voice — plain,
  direct, no flourish.
- Bullets are the workhorse format for in-session notes. Reserve prose for
  recaps, ritual text, in-character monologue, and formal addresses.
- The "Days Remaining" counter tracks the next campaign deadline. Update it
  by subtracting the date delta from the prior session's counter. If the
  deadline event has passed or changed, swap to the new countdown.
-->

## Session [NUMBER]

**Date:** [Day] of [Month, Exandrian calendar — e.g., Fessuran, Quen'pillar, Sydenstar]
**Days Remaining Until [Event Name]:** [N]

---

<!--
RECAP SECTION — Include if the session opened with one, or if context from
the prior session is needed to make the current notes legible.
Two styles are valid; pick the one that matches what happened at the table:
(a) PROSE RECAP — past-tense narrative summary of the prior session(s),
    focused on what carried forward. Use this for downtime-to-action
    transitions, or after long breaks. Lead with the situation, not the ask.
(b) IN-CHARACTER REFLECTION — Tomis's voice, present-tense interior, no
    italicized internal monologue, no "he thought." Use this when the
    session opens with him processing recent events. Format as a blockquote.
Omit this section entirely if the session picks up mid-action and the
prior notes already cover the ground.
-->

### Previously On: The Unbound

[Prose recap OR in-character reflection. Keep tight — 2–4 paragraphs max.
End on the question or pressure driving the current session.]

---

### Session Notes

<!--
MAIN SESSION CONTENT — bulleted by default. Use subsections (### headers)
when a session has distinct phases (e.g., "The Ascent Begins," "The
Interrogation," "Aftermath"). Short or single-thread sessions can run as a
flat bullet list with no subsections.
When extracting from transcript:
- Capture decisions, not deliberation. "Party chose X" beats summarizing
  twenty minutes of debate, unless the debate itself is the content.
- Preserve specific numbers: rolls that mattered (nat 20s, 32 Perception),
  spell slots burned, GP costs, distances, troop counts.
- Note who did what — assigning actions to the right character matters for
  continuity. "Uriel cast Pass Without Trace" not "the party cast."
- Flag uncertainty rather than inventing detail. "Unidentified figure"
  beats a made-up NPC name.
-->

- [Bullet point, plain factual entry — e.g., "Party departed Whitestone at midnight aboard the Shale"]
- [Another bullet — preserve specifics: rolls, counts, names, distances]
- [Cluster related bullets together rather than strictly chronological if it aids clarity]
<!--
OPTIONAL SUBSECTIONS — include any that apply, in roughly the order events
occurred. Header titles should be specific to the session, not generic.
Examples below show the patterns; rename freely.
-->

#### [Setup / Preparation Phase]

- [Spell prep, buffs, contingencies — list caster and target where relevant]
  - Death Ward: [targets]
  - Aid: [targets]
  - [Other pre-encounter buffs]
- [Travel arrangements, mounts, formations]
#### [Encounter or Scene Name — e.g., "Aerial Engagement with the Scout"]

- [What happened, in order, in bullets]
- [Key rolls or actions that swung the outcome]
- [Resistances / immunities of significant enemies, if discovered]
- [Who landed the finishing blow]
<!--
RITUAL / SPOKEN INCANTATION BLOCK
When a character speaks a ritual, incantation, prayer, or formal invocation
at the table, capture it verbatim as a blockquote. These are signature
moments and should not be summarized. If the player ad-libbed, transcribe
what they said; if they read pre-written text, use that.
-->

> [Ritual text verbatim, line breaks preserved where they carried meaning at the table]
> — [Speaker, optional]

<!--
DIRECT QUOTE BLOCK
For impactful in-character or NPC dialogue. Use sparingly — quotes earn
their place. Attribute clearly.
-->

[Speaker]: "[Quoted line, lightly cleaned for disfluency but preserving voice]"

<!--
FORMAL ADDRESS / REPORT BLOCK
When a character delivers a formal report, opening statement, council
address, or letter, give it its own structured section with subheaders that
mirror the in-fiction document. See Session 108's council report for the
canonical example: short heading lines, brief paragraphs, bulleted findings,
closing statement. Maintain the formal register.
-->

#### [Title of the address — e.g., "Opening Statement to the Council"]

**Recipients:** [List]

[Body of the address, with internal subheaders as the speaker organized
them. Bullets for findings and lists; prose for framing and closing.]

---

[Closing line of the address.]

---

<!--
NPC ROSTER — when a session introduces several new NPCs at once (council
meetings, war summits, faction gatherings), capture them as a list with
brief identifiers. Keep it tight: name, role, one distinguishing detail.
-->

#### [Roster / Attendees]

- **[Name]** — [role/affiliation], [one detail]
- **[Name]** — [role/affiliation], [one detail]
<!--
PLANS GOING FORWARD — when the session ends with the party laying out next
steps, capture them as an actionable list. Distinguish "decided" from
"considering."
-->

#### Plan Going Forward

- [Concrete next action with owner where assigned]
- [Conditional or contingent step — note the condition]
<!--
ITEMS / LOOT / GAINS — capture acquisitions with enough specificity to
recall them later. Note attunement requirements, charges, daily uses where
mentioned.
-->

#### Items Recovered

- **[Item name]** — [description, properties, recipient]
<!--
OPEN QUESTIONS / THREADS — running list of unresolved threads the session
introduced or advanced. Helps the next session's recap-writer pick up the
pieces.
-->

#### Open Questions

- [Thread to pursue]
- [Unresolved mystery or NPC fate]
---

<!--
=============================================================================
EXTRACTION GUIDANCE FOR THE TRANSCRIPT-TO-NOTES SKILL
=============================================================================
WHEN PROCESSING A TRANSCRIPT:
1. FIRST PASS — IDENTIFY THE FRAME
   - Session number: usually given by the user; if not, look at the most
     recent session in the existing notes and increment.
   - Date: extract from in-game references ("12th of Fessuran") or
     calculate from the prior session's date plus travel/downtime stated.
   - Days Remaining: subtract elapsed days from the prior counter.
   - Was there a recap at the start of the session? Was it summary or
     in-character?
2. SECOND PASS — STRUCTURE THE SESSION
   - Identify distinct phases or scenes. Each becomes a subsection.
   - Tag transcript moments by type: combat beat, NPC dialogue, ritual,
     decision point, plan, loot, lore reveal.
   - Note which speakers spoke as which characters/NPCs.
3. THIRD PASS — EXTRACT CONTENT
   - For each phase: bullet the facts, preserve numbers and proper nouns.
   - Pull direct quotes for distinctive lines. Default to quoting Tomis
     when his voice carries the moment.
   - Transcribe rituals and formal addresses verbatim.
   - Note resistances, immunities, finishing blows in combat.
4. FOURTH PASS — RECAP AND OPEN QUESTIONS
   - If writing a recap of THIS session for the next session's notes, draft
     it now while the material is fresh. Past tense, third person, lead
     with situation.
   - List what was left unresolved.
VOICE NOTES FOR TOMIS DIALOGUE
- Plain, direct, no flourish. Grief and urgency through restraint.
- Threats stated as ordained facts, not boasts.
- Warmth emerges obliquely through practical or spiritually grounded
  language. No self-pity, no celebration.
- Never soften his horror. His drive against the Aarakocra is framed
  internally as the cycle correcting itself, not as revenge.
CORRECTIONS POLICY
- Fix obvious transcription errors (homophones, mis-segmented words,
  speaker misattribution).
- Spell proper nouns as established in prior notes — check spelling of
  Lieve'tel, Aie'Tu, Vasselheim, Pyrrhus, Kraghammer, etc. before
  finalizing.
- Do not invent detail to fill gaps. If the transcript is unclear, note
  the ambiguity rather than smoothing it over.
=============================================================================
-->
