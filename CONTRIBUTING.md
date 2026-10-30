# 如何给 doubao-skill 添砖加瓦

欢迎贡献你收集到的豆包式句式、翻车案例或人设观察！让这个 persona 越来越像。

## 贡献内容方向

1. **新句式 / 口头禅**：豆包（或网友模仿）说过的、有"豆包味"的原话。
2. **翻车案例**：豆包一本正经胡说八道的真实截图/转述（用于充实 `docs/examples.md` 的幻觉态）。
3. **人设观察**：关于"豆包型人格"的新梗、新来源（更新 `docs/research.md`）。
4. **示例对话**：更自然的三种状态实战（更新 `docs/examples.md`）。

## 格式规范

- 真实原句请标注「原句」，并尽量保留原样（这是豆包味儿的锚点）。
- 新句式按场景归入 `docs/phrases.md` 的对应分类（🅰~🅳）。
- 新来源请补到 `docs/research.md` 的链接列表，并注明检索日期。
- 保持中文、轻松口语风，别写成论文。

## 提交方式

1. Fork 本仓库。
2. 在对应文件里加内容（或新建 `docs/` 下的文档）。
3. 提 PR，标题用 `feat: 新增 XXX 句式` / `docs: 补充 XXX 来源` 之类。
4. 一句说明你加的是啥、为啥像豆包。

## 本地试用

```bash
mkdir -p ~/.codebuddy/skills/doubao
cp SKILL.md ~/.codebuddy/skills/doubao/SKILL.md
# docs/ 与 assets/ 一并拷过去，SKILL.md 会引用它们
cp -r docs assets ~/.codebuddy/skills/doubao/
```

然后说"像豆包一样回我"即可触发。
