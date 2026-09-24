# Agent instructions

This repo holds one public resume. `resume.typ` is the source of truth. `resume.pdf` is the compiled copy GitHub shows. `cover-letter.typ` is the cover letter template. Cover letters are always tailored, so do not commit a filled-in letter.

The master resume is the full library for every later copy. It can run longer than one page. Do not drop a job, project, or bullet from `resume.typ` to save space. One-page cuts happen only on tailored copies in `applications/`.

## Compile

Master files, from the repo root:

```bash
typst compile resume.typ resume.pdf
```

Do not compile a send PDF or a filled cover letter in the repo root.

## What belongs on GitHub

Commit `resume.typ` and `resume.pdf` only when the generic resume gets better for every application. Examples are a stronger bullet, a new project, or a skills line that stays true everywhere.

Commit `cover-letter.typ` only when the template or shared contact header changes. Do not commit a letter written for one company.

`experiences.md` is the master library of STAR stories for cover letters. Commit it when a new true story is added. Do not put company-specific letter text in it.

Do not commit a version of either document that exists only for one posting.

## Tailoring

Read `.cursor/skills/resume-tailor/SKILL.md` before editing. Never edit the root `resume.typ` or `cover-letter.typ` for a posting. Copy them into `applications/`, then tailor the copies.

1. Create a folder and copy the masters:

```bash
mkdir -p applications/<yyyy-mm-company-role>
cp resume.typ cover-letter.typ applications/<yyyy-mm-company-role>/
```

2. Analyze the posting in chat. Follow the resume-tailor skill on `applications/<yyyy-mm-company-role>/resume.typ`: reorder, drop a weak project, and add keywords that are actually true. Put the tailoring plan in chat. Commerce coursework is tailored-only (see that skill); do not add a course list to the master.
3. Bold matching keywords in Experience and Project bullets only. See Scannable keywords below.
4. If the user asked for a cover letter, or the posting requires one, write it using `.cursor/skills/cover-letter-generator/SKILL.md`. Fill `applications/<yyyy-mm-company-role>/cover-letter.typ`. Put the analysis, alternative openings, and interview talking points in chat, not in Typst.
5. Compile the send files in that folder:

```bash
typst compile applications/<yyyy-mm-company-role>/resume.typ applications/<yyyy-mm-company-role>/Yin_Cheung_Resume.pdf
typst compile applications/<yyyy-mm-company-role>/cover-letter.typ applications/<yyyy-mm-company-role>/cover-letter.pdf
```

The file to download and attach is `applications/<yyyy-mm-company-role>/Yin_Cheung_Resume.pdf`. Do not put company names, dates, or role tags in that filename.

If a tailored edit is simply a better sentence, fold it into the root `resume.typ` and commit that. That is the only tailoring that belongs in git.

This resume has no professional summary. Do not add one unless the user asks.

## Scannable keywords

A recruiter should be able to skim Experience and Projects and see the posting's stack.

Bold matching technologies and phrases only inside Experience and Project bullets. Do not bold them on tool lists: the company tech line, the project tech line, or the Skills section.

Bold only terms that are true of the work. Do not bold entire sentences. Do not stuff the same keyword into every line.

In Typst, write `*Python*`. Put a space around `/` so `*JWT* / Argon2` compiles.

Reorder the Skills list so matching skills come first. Leave the Skills names unbolded except for the category labels.

## Cover letters

Read `.cursor/skills/cover-letter-generator/SKILL.md` before writing. The letter pulls from `resume.typ` and from `experiences.md`. If role, one strong story, or a real reason for this company is missing, stop and ask. Do not draft until those are known. Fill the lets at the top of the copied `cover-letter.typ` (`letter-date`, `company`, `company-location`, `greeting`) and replace the placeholder paragraphs.

Keep the letter under 300 words and one page. Match tone to the company: more formal for banks, insurers, and other enterprise roles. Research the company before using a company-knowledge hook. Do not invent tools, metrics, job titles, or company facts.

If the posting wants resume, letter, and transcript in one PDF, say so after compiling. Do not merge a transcript unless the user asks.

## Local snapshots

`applications/` is gitignored. One folder per application:

```
applications/
  2026-08-google-swe-intern/
    resume.typ
    cover-letter.typ
    Yin_Cheung_Resume.pdf
    cover-letter.pdf
```

Do not create a tracker in this repo. Application logging lives in Google Sheets.

Do not create a git branch per company. Do not add reusable Backend / Full-stack / ML variants unless those are stable tracks sent often.

## Honesty

Do not invent tools, metrics, or job titles. Tailoring means emphasis and order, not fiction.
