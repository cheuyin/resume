---
name: resume-tailor
description: Customize resume for specific job postings while maintaining truthfulness. Use when the user asks to tailor, customize, or target a resume for a job description or role.
---

# Resume Tailor

## When to Use This Skill

Use this skill when the user wants to:
- Customize their resume for a specific job posting
- Adjust their resume to match job requirements
- Create a targeted version of their resume
- Mentions: "tailor resume", "customize resume", "target role", "specific job", "match job description"

Use AFTER job-description-analyzer to know what to emphasize.

## Core Capabilities

- Reorder experience sections by relevance to target role
- Adjust professional summary for specific position
- Add missing keywords from job description
- Modify bullet points to match job requirements
- Maintain authenticity while optimizing match
- Create multiple targeted resume versions

## The Tailoring Philosophy

**Key Principle:** You're not lying or fabricating - you're HIGHLIGHTING the most relevant parts of your true experience.

Think of your full experience as a library of achievements. Tailoring means selecting the books that best fit what each employer is looking for.

## Tailoring Process

### Step 1: Analyze the Job (Use Job Description Analyzer First)
- Identify required skills and keywords
- Note the company's priorities
- Understand the role's primary responsibilities

### Step 2: Audit Your Resume
For each section, ask:
- Does this support my candidacy for THIS specific role?
- Is there a better way to phrase this for THIS job?
- Should this be higher or lower in priority?

### Step 3: Make Strategic Adjustments

**Professional Summary:** Rewrite to mirror the job's key requirements

**Skills Section:** Reorder to put most relevant skills first, add missing keywords

**Experience:** 
- Reorder jobs if a less recent role is more relevant
- Swap bullet points to lead with most relevant achievements
- Add keywords naturally into existing bullets

**Education:** Highlight relevant coursework, certifications

## Section-by-Section Tailoring Guide

### Professional Summary

This is your "elevator pitch" - customize for each application.

**Generic Summary (AVOID):**
```
Results-driven professional with 5 years of experience in business operations. Strong analytical and communication skills. Looking for a challenging opportunity to grow.
```

**Tailored for Operations Manager Role:**
```
Operations Manager with 5 years optimizing supply chain processes and reducing costs by 25%. Expertise in Lean Six Sigma, vendor management, and cross-functional team leadership. Track record of improving operational efficiency while maintaining quality standards.
```

**Tailored for Project Manager Role (Same Person):**
```
Project Manager with 5 years leading cross-functional initiatives from concept to delivery. PMP-certified with expertise in Agile methodology, stakeholder management, and budget oversight. Track record of on-time, under-budget project delivery across $10M+ portfolios.
```

### Skills Section Reordering

**Job Description Emphasizes:** Data analysis, SQL, Python, stakeholder communication

**Before (Generic Order):**
```
Skills: Microsoft Office, Communication, Project Management, Python, SQL, Data Visualization, Leadership
```

**After (Tailored Order):**
```
Skills: SQL, Python, Data Analysis, Data Visualization, Stakeholder Communication, Project Management, Microsoft Office
```

### Experience Section

**Strategy 1: Reorder Jobs**

If your most recent job is less relevant than a previous role:

**Before:**
1. Marketing Coordinator (current, but applying for data role)
2. Data Analyst (previous, highly relevant)

**After:**
1. Data Analyst (labeled with dates, moved up)
2. Marketing Coordinator (still included, but secondary)

**Strategy 2: Swap Bullet Order**

Lead with bullets most relevant to the target role.

**Applying for Management Role - Lead with:**
- "Led team of 12..."
- "Managed budget of $2M..."

**Applying for Technical Role - Lead with:**
- "Developed automated system..."
- "Analyzed 500K+ data points..."

**Strategy 3: Adjust Bullet Language**

Incorporate job description keywords while staying truthful.

**Job Description Says:** "stakeholder management"
**Your Bullet Says:** "Worked with various teams"
**Tailored Version:** "Managed stakeholder relationships across 5 departments, ensuring alignment on project priorities"

## Tailoring Templates

### For Each Job Application, Create:

```markdown
## RESUME TAILORING PLAN

**Target Position:** [Job Title]
**Company:** [Company Name]
**Match Score:** [From JD Analyzer]

### Summary Customization
**Current:** [Your current summary]
**Tailored:** [Rewritten for this role]

### Skills Reordering
**Current Order:** [List]
**New Order:** [Reordered list with added keywords]
**Keywords Added:** [New skills from JD]

### Experience Adjustments

**Job 1: [Title]**
- Bullet to emphasize: [Which bullet to lead with]
- Keyword to add: [What phrase to incorporate]
- Bullet to de-emphasize: [Move down or remove if space needed]

**Job 2: [Title]**
[Same structure]

### Other Adjustments
- Education: [Any relevant coursework to add]
- Certifications: [Any to highlight]
- Projects: [Relevant projects to include]
```

## Common Tailoring Scenarios

### Scenario 1: Technical Role at Non-Tech Company

**Challenge:** They want technical skills but also business acumen

**Strategy:**
- Lead with technical achievements
- Include business impact in every technical bullet
- Add "translated technical concepts for business stakeholders"

### Scenario 2: Management Role (But You've Done Both IC and Management)

**Challenge:** Show leadership without abandoning technical credibility

**Strategy:**
- Summary: Emphasize leadership
- Experience: Lead with team management bullets
- Keep some technical bullets to show you understand the work

### Scenario 3: Startup (But You've Worked at Big Companies)

**Challenge:** Show you can thrive in ambiguity and wear many hats

**Strategy:**
- Highlight cross-functional work
- Emphasize initiative and self-starting
- Show scrappy, creative problem-solving
- De-emphasize rigid processes and large team structures

### Scenario 4: Big Company (But You've Worked at Startups)

**Challenge:** Show you can work within structure and at scale

**Strategy:**
- Emphasize process improvement
- Highlight work that scaled
- Show collaboration across teams
- Add metrics that show impact at scale

## Keyword Integration Rules

### DO:
- Add keywords that truthfully describe your work
- Use exact phrasing from job description when accurate
- Place keywords naturally in context
- Include keywords in multiple locations (summary, skills, experience)

### DON'T:
- Add skills you don't actually have
- Keyword stuff (repeating same term 10x)
- Create a different meaning than your actual experience
- Sacrifice readability for keyword density

## Truth vs. Tailoring Line

**Acceptable Tailoring:**
- Reordering true information
- Emphasizing relevant experience
- Using industry-standard terminology
- Adding context to vague statements
- Matching language style to job description

**Unacceptable (Lying):**
- Adding skills you don't have
- Changing numbers or metrics
- Creating fake experiences
- Claiming titles you didn't hold
- Stating certifications you don't have

## Version Management

### Maintain a Master Resume
- Keep ONE complete document with ALL experiences
- Include every bullet you've ever written
- This is your "source of truth"
- It may be longer than one page; do not cut it to fit a page

### Create Targeted Versions
- Name files clearly: "JohnSmith_Resume_ProductManager_TechCorp.pdf"
- Track which version went to which company
- Save tailoring notes for interview prep

### Version Naming Convention
```
[LastName]_Resume_[TargetRole]_[Company]_[Date].pdf

Examples:
- Smith_Resume_PM_Google_Jan2024.pdf
- Smith_Resume_DataAnalyst_Meta_Jan2024.pdf
- Smith_Resume_General_Master.docx (your master file)
```

## Quick Tailoring Checklist

Before submitting any resume:

1. ✅ Summary mentions the exact job title/function
2. ✅ Top 5 skills match job description's top 5 requirements
3. ✅ Most relevant experience is positioned first
4. ✅ Each job's top bullet addresses job's key requirement
5. ✅ Keywords from JD appear naturally throughout
6. ✅ Company/industry terminology is used correctly
7. ✅ All claims are truthful
8. ✅ File is named appropriately
9. ✅ ATS formatting maintained
10. ✅ Saved for interview prep reference

## Output Format

When tailoring a resume, provide:

```markdown
# TAILORED RESUME CHANGES

## Target: [Job Title] at [Company]

### Professional Summary
**Before:** [Original]
**After:** [Tailored version]
**Keywords Added:** [List]

### Skills Section
**New Order:** [Reordered list]
**Added:** [New keywords]
**Removed:** [If any, for space]

### Experience Changes

**[Company Name] - [Title]**
- Move bullet X to position 1
- Modify bullet Y: [Before → After]
- Add keyword "[phrase]" to bullet Z

[Repeat for each relevant job]

### Overall Changes Summary
- Keywords added: X
- Bullets modified: Y
- Sections reordered: Yes/No
- Estimated new match score: Z%
```

Put this change plan in chat. Then edit the copy of `resume.typ` in the application folder and compile. Do not leave the tailored resume only in markdown. Do not edit the root master.

## Implementation Notes

- Always start with the job description analyzer
- Keep tailoring changes documented for interview prep
- Maintain master resume as source of truth
- Never sacrifice ATS compatibility for tailoring
- Test keyword match after tailoring

## This repository

There is no separate job-description-analyzer skill. Do Step 1 in chat, then tailor.

This resume has no professional summary. Do not add one unless the user asks. Skip the summary section of the plan.

Copy the masters into `applications/<yyyy-mm-company-role>/` and edit only those copies. Keep the send copy to one page. The master may be longer than one page; do not cut `resume.typ` to fit a page. Follow `AGENTS.md`. Do not edit root `resume.typ` or `cover-letter.typ` for a posting.

**Bold keywords** only inside Experience and Project bullets so a recruiter can skim the stack. Do not bold keywords on tool lists: the company tech line (`VoltSafe Inc. | TypeScript, ...`), the project tech line, or the Skills section. Project names stay bold as titles.

Bold only terms that are actually in the work. Do not bold entire bullets. In Typst, write `*Python*`. Put a space around `/` so `*JWT* / Argon2` compiles; `*JWT*/Argon2` does not.

Compile the send file in that folder as `Yin_Cheung_Resume.pdf`. Do not put the company name in the filename you attach.

Master `resume.typ` is the source of truth for GitHub. Targeted versions live only under `applications/`. Do not invent tools, metrics, or titles.

### Commerce coursework (tailored copies only)

The master degree line already has `Minor in Commerce`. Do not add a course list to root `resume.typ`.

On a tailored copy, add this Education bullet when the posting is finance, markets, accounting, consulting, product, marketing, or otherwise wants a business background (investment firms, banks, PE/VC, asset management, insurers):

```
- Relevant coursework: Financial Accounting, Organizational Behaviour, Marketing
```

Put Financial Accounting first. Do not use course codes (`COMR 457`). Do not mark courses in progress.

Skip this bullet on generic SWE, backend, full-stack, and other software-only postings. The minor on the degree line is enough.
