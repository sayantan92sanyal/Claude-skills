# human-written

A Claude skill that rewrites an article so it does not read as AI-generated.

It enforces writing rules drawn from published research on AI-writing tells, including Wikipedia's "Signs of AI writing" guide, Pangram's frequency analysis of AI text, and the PubMed "excess vocabulary" study (Kobak et al.):

- Natural sentence and paragraph rhythm, without forced "human" tricks
- A banned word and phrase list you can edit
- No contractions (I am, not I'm)
- Minimal em dashes, no random bold, no bold-label bullets, no emojis or decorative Unicode
- No negative parallelism ("not just X, but Y"), reflexive triplets, trailing "-ing" commentary, synonym cycling, or vague attribution
- No inflated significance, manufactured suspense, or unearned calls to action
- Facts, names, and numbers kept exactly as in the source, with nothing invented
- A final self-audit checklist before the text is returned

## Repo layout

```
human-written/                  <- repo root
├── README.md
└── human-written/              <- the skill folder
    ├── SKILL.md                <- instructions Claude reads
    └── references/
        ├── banned-phrases.md   <- edit this list over time
        └── before-after.md     <- calibration example
```

## Install

**Claude.ai (web or desktop):** zip the inner `human-written/` folder so the folder itself is at the top level of the zip, then upload it under Settings, in the skills section. Menu names change, so check Anthropic's current docs if you cannot find it.

**Claude Code:** copy the inner `human-written/` folder to `~/.claude/skills/` (personal) or `.claude/skills/` inside a project.

## Use

Ask Claude to use the skill, or just say what you want:

> Use the human-written skill to rewrite the article below.

Paste the article after it. For a closer match to your own voice, paste a short sample of your writing too.

## Customize

- Add or remove entries in `human-written/references/banned-phrases.md`.
- Adjust the rules in `human-written/SKILL.md`. Keep the frontmatter `name` equal to the folder name.

## Notes

No rule list can guarantee that detectors or readers will not flag a text. Treat the output as a strong first draft and read it once yourself.
