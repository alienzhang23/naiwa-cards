# 奶娃知识卡片（naiwa-cards）

输入一篇文章、一段话或一句话，输出一套 **3:4 竖版小红书知识卡片**，单张生图直出。

每张卡片只讲一件事：顶部一个抓人的问题，中部奶娃出镜讲解，接着 3–4 个要点，底部一句话结论。读者 3 秒看懂一张，整套看完带走一个完整认知。

## 主角：奶娃

圆润的黄色团子，黑色手绘墨线、扁平奶黄填充，大大的绿眼睛、一条平静的一字嘴、一双棕色小手。冷静、话少、爱思考——每张卡片里它都在"讲"点什么，绝不当装饰。

## 制作原理

- 每张卡片**一次生图调用直出**，卡片上的所有文字都由生图模型绘制；
- IP 参考图（`assets/character/naiwa/ref-front.png`）只用于锁定奶娃形象，不抄场景和姿势；
- 纯白背景、黑色手绘线稿、奶娃是全图唯一的彩色角色、少量红/蓝手写批注；
- 文字宁可少写、不可写错：提示词用"只能出现这些字 / EXACTLY these words"锁死。

## 用法

这是一个 Agent Skill，把本仓库放进你的 AI 助手 skill 目录即可使用（Claude Code / Codex / Cursor 等）：

```bash
# 示例：放到 Claude Code 的 skill 目录
cp -r naiwa-cards ~/.claude/skills/
```

然后对 AI 说：

> 把这篇文章做成奶娃知识卡片

AI 会先给出卡片组策略（每张的问题 + 要点 + 结论）请你过目，确认后逐张生成。每张一出就交付，不攒着。

## 换主角

默认主角是奶娃。想换成你自己的 IP/吉祥物：准备一张干净的正面定妆图存到 `assets/character/<slug>/ref-front.png`，按 `ips/naiwa.md` 的格式写一份 `ips/<slug>.md` 档案，再更新 `config/active-ip.md` 即可。

## 示例

`examples/sample/card-01.png` —— "Agent 和 Bot 有啥区别？"样卡。

## License

MIT
