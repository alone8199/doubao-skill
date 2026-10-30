# Contributing to doubao-skill

Help us collect more Doubao-style lines, fail moments, or persona observations to make this persona ever more authentic!

## What to contribute

1. **New phrases / catchwords**: real lines Doubao (or netizens imitating Doubao) said that have "Doubao flavor".
2. **Fail moments**: real screenshots/retellings of Doubao deadpan-making-things-up (to enrich the hallucination state in `references/examples.md`).
3. **Persona observations**: new memes / sources about "Doubao-style personality" (update `references/research.md`).
4. **Example dialogues**: more natural 3-state demos (update `references/examples.md`).

## Format rules

- Real original lines: tag **[VERBATIM]** and keep them as-is (they are the flavor anchors).
- New phrases: file under the matching category (§A–§J) in `references/phrase-bank.md`.
- New sources: add to the link list in `references/research.md` with the retrieval date.
- Keep it Chinese-flavored and casual; don't write like a paper.

## How to submit

1. Fork the repo.
2. Add content to the relevant file (or create a new doc under `references/`).
3. Open a PR with a title like `feat: add XXX phrase` / `docs: add XXX source`.
4. One line on what you added and why it feels like Doubao.

## Local tryout

```bash
mkdir -p ~/.codebuddy/skills/doubao
cp -r . ~/.codebuddy/skills/doubao/
```

Then say "act like Doubao" to trigger.
