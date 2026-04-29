# SVP Claude Skills

A library of Claude skills built for the SVP Sales and Marketing teams. Each skill gives Claude deep, task-specific context so it can produce output that's actually useful.

**Maintained by:** Alfie, Product Marketing @ Social Value Portal

---

## What's in here

| Skill | What it does |
|---|---|---|
| `svp--public-sector-proposal-writer` | Writes tailored proposal copy from discovery notes, call transcripts and research you have available |
| `svp-brand-guidelines` | Enforces SVP's visual identity in any designed output | COMING SOON
| `qbr-deck-preparation` | Structures and drafts QBR presentation content | COMING SOON
| `social-value-research` | Synthesises customer and sector research for social value context | COMING SOON
| `social-value-case-studies` | Synthesises customer Social Value data to turn raw project data into a case study slide | COMING SOON

---

## How to download a skill

1. Navigate to the skill folder you want (e.g. `/skills/svp-proposal-writer/`)
2. Open the `SKILL.md` file
3. Click the **Raw** button in the top-right of the file view
4. Right-click the page and select **Save As**, saving it as `SKILL.md` — or copy the raw URL and run:

```bash
curl -O https://raw.githubusercontent.com/your-org/your-repo/main/skills/svp-proposal-writer/SKILL.md
```

---

## How to install a skill into Claude

Skills work by being made available to Claude at runtime via a mounted file path. The exact setup depends on your Claude environment, but the general flow is:

### If you're using Claude.ai (Projects)

1. Open the relevant **Project** in Claude.ai
2. Go to **Project Settings → Instructions** (or equivalent in your plan)
3. Paste the contents of `SKILL.md` into the custom instructions field, or attach the file if your plan supports file uploads to Projects
4. Claude will now have access to the skill in that Project context

### If you're using the Claude API / a local Claude environment

1. Place the downloaded `SKILL.md` file in your skills directory (e.g. `/mnt/skills/user/`)
2. Ensure your system prompt or environment configuration references that directory
3. Claude will detect and load the skill when relevant tasks are triggered

> **Note:** If you're unsure which setup applies to you, ask Alfie or check with whoever manages your Claude environment.

---

## Adding or updating a skill

Raise a PR against `main` with your changes. Tag `@alfie` for review. Keep skill descriptions accurate — they control when Claude decides to use the skill, so vague descriptions lead to it being ignored or misapplied.

---

## Questions

Ping Alfie in Slack or open an issue in this repo.
