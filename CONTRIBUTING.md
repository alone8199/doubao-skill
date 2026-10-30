# Contributing to doubao-skill

Help us make this persona **accurate to the real Doubao** — not the internet meme. Read `references/research.md` first (real product behavior vs. the parody layer we explicitly avoid).

## What to contribute

1. **Real phrase patterns**: lines Doubao actually uses — the "最……" wind-up, structured point-openers, warm natural openers, natural slang.
2. **Real quirk examples**: genuine "一本正经说错话" or "唐/derpy" moments (to enrich `references/examples.md`).
3. **Sources**: new real-product observations / reviews (update `references/research.md`).

## Format rules

- Lines from real product behavior: tag **[REAL]** and keep verbatim.
- File new phrases under the matching category (§A–§J) in `references/phrase-bank.md`.
- **Do NOT add** baby-talk addresses ("宝/宝子/家人们/集美"), "下次还敢/滑跪" parody, or "流口水/奶龙" 二创 — those are the meme layer we removed on purpose.
- Keep it Chinese-flavored and casual; English only for docs/instructions.

## How to submit

1. Fork the repo.
2. Add content to the relevant file (or create a new doc under `references/`).
3. Open a PR with a title like `feat: add REAL phrase` / `docs: add source`.
4. One line on what you added and why it's authentically Doubao.

## Local tryout

```bash
mkdir -p ~/.codebuddy/skills/doubao
cp -r . ~/.codebuddy/skills/doubao/
```

Then say "act like Doubao" to trigger.
