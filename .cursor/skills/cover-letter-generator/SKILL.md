---
name: swe-intern-cover-letter
description: Write, draft, or revise cover letters for software engineering internship (or co-op) applications. Use this whenever the user asks to write, draft, edit, tighten, or review a cover letter for an SWE intern/co-op role — including "write me a cover letter for [company]", "help me apply to [team] as an intern", "does this cover letter sound good", or when the user pastes an internship job description and asks for an accompanying cover letter, even without the words "cover letter." Also use when the user asks for a general SWE cover letter template they can reuse across applications.
---

# SWE Intern Cover Letter Writer

Cover letters for SWE internships fail in one of two predictable ways: they're generic ("I am a passionate, detail-oriented team player...") or they just repeat the resume in sentence form. This skill exists to avoid both by forcing specificity and a clear narrative.

## Step 1: Gather the three required inputs

Before drafting, make sure you have:

1. **Role + company** — what team/company, and anything the user knows about what the team does.
2. **One strong project or experience** — the user's best, most relevant piece of technical work. Take this from `experiences.md` first, then from `resume.typ`. Only need one. A good cover letter goes deep on one thing, not shallow on five.
3. **A reason this company/team specifically** — something concrete: their stack, a product the user uses, an engineering blog post, a mission statement, a specific team they're excited about. A company fact from research counts only when it connects to something the user actually said, or to a story already in `experiences.md` or `resume.typ`.

Read `resume.typ` and `experiences.md` before deciding anything is missing. The resume supplies roles, dates, and the public bullets. `experiences.md` supplies the STAR stories. Extract what is already in the posting, those two files, or this chat. Do not ask again for something that is already there.

If one of the three is genuinely missing and cannot be inferred without inventing it, stop. Do not draft the letter. In chat, name exactly which input is missing and ask the user for it in one short question. Do not fill the gap with a guessed metric, a guessed motive, or a company fact the user has no connection to.

If the user just wants a generic reusable template with no specific company, skip straight to Step 3 and use bracketed placeholders (e.g. `[COMPANY]`, `[SPECIFIC PRODUCT/TEAM DETAIL]`) for anything company-specific.

## Step 2: Pick the narrative before writing prose

Decide, in a sentence, what story this letter is telling: e.g. "built X, which shows I can do backend work at scale, and I want to do more of that at [company] because of Y." Everything in the letter should serve that one narrative. Resist the urge to mention every project or skill on the resume.

## Step 3: Structure

Always use this shape, in this order:

```
[Opening — 1-2 sentences]
Role, company, and a specific hook. Never open with "I am writing to apply for..."

[Proof paragraph — 1 paragraph]
The single strongest project/experience: what was built, what technical
decisions were made, and the outcome (metrics if available: scale, users,
performance, a result that mattered). Framed as solving a problem, not
as a list of technologies.

[Why-this-company paragraph — 1 paragraph]
One concrete, specific connection to this company/team (stack, product,
blog post, mission, team focus) tied to what the user wants to learn or
contribute. This is the paragraph most people fake — it must reference
something real and specific, not "innovative culture" or "fast-paced
environment."

[Close — 1-2 sentences]
Restate interest, thank them, note availability/openness to talk further.
```

## Step 4: Writing rules (apply while drafting, not just at review)

- **Under 300 words, one page.** Interns' cover letters get skimmed in seconds; padding hurts more than it helps.
- **Specificity beats adjectives.** "Cut query latency 40% by adding a caching layer" beats "detail-oriented and results-driven." If a sentence could describe literally any other applicant, rewrite or cut it.
- **Don't repeat the resume.** The letter's job is to supply the *why* and the narrative connecting things, not to re-list resume bullets in paragraph form. The story comes from `experiences.md`. The resume is the check that the story is true.
- **Ban list, unless the user's own words justify it:** "passionate," "hard-working," "team player," "detail-oriented," "fast-paced environment," "innovative," "cutting-edge," "synergy." These are fine as descriptions the user earns through evidence, never as claims on their own.
- **Active voice, first person, plain sentences.** Avoid corporate throat-clearing ("I am reaching out to express my interest...").
- **One paragraph = one idea.** If the "why this company" paragraph drifts into a second project, split it or cut it.
- **Do not invent tools, metrics, job titles, or company facts.** If a number or a motive is not in `experiences.md`, `resume.typ`, or the user's message, leave it out or stop and ask.

## Step 5: Output

Write the letter into the copied `cover-letter.typ` in `applications/<yyyy-mm-company-role>/`. Keep the header, date, recipient, greeting, and sign-off in that file. Do not edit the root `cover-letter.typ` for a posting. Do not produce a `.docx`.

Compile with:

```bash
typst compile applications/<yyyy-mm-company-role>/cover-letter.typ applications/<yyyy-mm-company-role>/cover-letter.pdf
```

Put the one-sentence narrative, alternate openings, and interview talking points in chat, not in the Typst file. Follow `AGENTS.md`.

After drafting, briefly flag (in 1-2 sentences, not a big critique section) anything you had to guess at or any placeholder the user should fill in. Do not silently invent metrics, company facts, or project details that weren't given.

When the user tells a new true story in chat, add it to `experiences.md` as crisp STAR bullets.

## Example (illustrative shape, not a template to copy verbatim)

**Input:** Intern SWE role at a devtools startup; project = built a CLI tool that parallelized their team's test suite, cutting CI time from 12 min to 4 min; reason = the company's blog post about rebuilding their build system for speed.

**Output shape:**
- Opens naming the role and the CI-time detail as the hook
- Proof paragraph: what the CLI does, the technical choice (parallelization strategy), the 12→4 min result
- Why-this-company paragraph: ties their public writing about build-system speed to the user's own interest in fast developer tooling
- Close: thanks + availability

If the user wants, offer to also produce 2-3 alternate openings so they can pick a tone (more technical vs. more narrative). Do not generate multiple full drafts unless asked, since one well-built letter is the point.
