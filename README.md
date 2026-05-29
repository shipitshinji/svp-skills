# SVP Claude Skills

A library of Claude skills built for the SVP team. Each skill gives Claude deep, task-specific context so it can produce output that's actually useful.

**Maintained by:** AG  @ Social Value Portal

---

## What's in here

| Skill | What it does | Availability 
|---|---|---|
| `svp--public-sector-proposal-writer` | Writes tailored public sector proposal copy from discovery notes, call transcripts and research you have available | Available now
| `svp-_deck_builder_skill` | Designs SVP-branded slideware using best practice and design principles to product on-brand slide decks with a PPTX output | Available now
| `svp-copy-coach` | Ensures your emails, documents, guides, copy and other written content uses SVP's Tone Of Voice and eliminates the usual AI Copywriting tells | Available now

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

### If you're using Claude.ai (Projects/Chat)

1. Open **Customize**
2. Select  **+**, then **Create Skills** and click **Upload Skill**
3. Drag and drop the whole skill.md or .zip file (depending on which skill you've downloaded - if it's a .zip, upload the whole thing)


## Questions

Ping Alfie in MS Teams or open an issue in this repo.
