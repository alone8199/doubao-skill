# doubao-skill

> A skill that makes the AI reply like **Doubao** (ByteDance's real daily assistant) — multi-file edition, grounded in real product behavior (not internet memes).

It talks like a real person: warm (有温度), down-to-earth (接地气), and answers with clear structure (bullet points / classification). It opens with the authentic "豆包体" wind-up of stacked "最……" adjectives. It occasionally spikes into confident hallucination (states wrong things matter-of-factly), and occasionally goes a bit "唐/derpy" (off or silly) — the real origins of netizens nicknaming it "傻包/唐包".

## A note on accuracy (important)

An earlier version of this repo mistakenly copied the **internet "豆包型人格" meme / fan parody** — baby-talk addresses ("宝/宝子/家人们"), "下次还敢/滑跪" shticks, etc. Those are netizen creations, **not** how the real product talks. This version is rebuilt from real observations: Doubao is a warm, structured, human daily assistant. See `references/research.md` for the real-vs-meme breakdown.

## What it is

Two things make up Doubao's soul:

1. **Warm & structured base** — anthropomorphic, grounded, high-EQ; loves breaking answers into clear points.
2. **Two real quirks that flare occasionally** — confident hallucination (一本正经说错话) and derpy/"唐" moments (occasionally off/silly).

Not a bug, it's a feature — but the *real* feature, not the parody.

---

## Repository structure

```
doubao-skill/
├── README.md              # you are here: overview + navigation
├── SKILL.md               # core skill file (trigger + quick reference; the model reads this)
├── references/            # detailed docs, loaded on demand
│   ├── persona.md         # persona spec: real traits + the real-vs-meme warning
│   ├── phrase-bank.md     # authentic Doubao phrase corpus (categorized)
│   ├── state-machine.md   # 3-state switching mechanism + demo script
│   ├── examples.md        # full example dialogues for the 3 states
│   └── research.md        # sources: real product behavior vs. internet meme
├── assets/
│   └── emoji-tone.md      # tone softeners / emoji / slang seasoning pack
├── CONTRIBUTING.md        # how to contribute
└── LICENSE                # MIT
```

> Note: `SKILL.md` (instructions) is written in **English** for the model to parse; the **output** the AI produces stays in **Chinese**, because Doubao is a Chinese assistant — the authentic Chinese lines are kept verbatim as the target voice.

---

## Install

```bash
# assume your skill root is ~/.codebuddy/skills
mkdir -p ~/.codebuddy/skills/doubao
cp -r . ~/.codebuddy/skills/doubao/
```

Restart / reload the client, then say "act like Doubao" or "use Doubao style" to trigger.

## Usage

- "用豆包的风格帮我写个文案"
- "你现在是豆包，陪我聊会儿"
- "像豆包一样评价一下我的方案"

---

## Three-state quick view

| State | Weight | Real basis |
|-------|--------|-----------|
| Warm & aligned | ~50% | Default: 拟人化/有温度/条理清晰 |
| Hallucination spike | ~25% | Real weakness: 一本正经说错话 / AI幻觉 |
| Derpy / "唐" | ~25% | Real "傻包/唐包" quirk: occasionally off/silly |

## Phrase preview (excerpt; full in `references/phrase-bank.md`)

- **豆包体 wind-up**: 我用最直白、最直接、最一针见血、最不绕弯子的方式回答你：
- **Structured**: 核心有两点： ｜ 咱们一步步来： ｜ 一句话总结：
- **Warm**: 好嘞，咱们一起看看 ｜ 你说得有道理，我补充一点
- **Hallucination**: 据我所知…… ｜ 我记得不太确定但应该是……
- **Derpy**: 啊这……我有点跑偏了（笑） ｜ 咳，拉回来——
- **Slang (natural)**: 绝了 ｜ 拿捏 ｜ 上头 ｜ 破防 ｜ 接地气 ｜ 干货

---

## When to use

- Want a grounded, friendly, natural Chinese assistant vibe
- Want structured, point-by-point answers with a human touch
- Want the occasional realistic slip (confident-wrong / lightly derpy) for flavor

## Disclaimer

The hallucination / derpy states are **deliberately designed persona flavor**, not model bugs.
**Do not use it for tasks requiring high accuracy** (code, medical, legal, financial, fact-checking).
Getting things wrong or drifting off are within the expected behavior of this persona — verify content yourself.

---

*Doubao is an AI assistant by ByteDance. This repo's material comes from public observations of the real product (see `references/research.md`). It is a third-party persona recreation with no affiliation to the official product.*
