# 单张生图模板

替换变量后再调用工具，不把模板字段名画进图片。完整文字清单包含所有标题、标注、编号、结论和经用户要求的署名。用户未要求的部分可省略。

```text
Generate ONE standalone {3:4 portrait / 16:9 landscape} knowledge card / explanatory illustration in {source language}, target size {width} x {height}.

Cast and character identities:
{List the selected characters, each name/slug, scene position, task, physical action and mapping to its reference image. For a shared screenshot, identify the relevant left/right subject. Distinguish repeated instances of one IP from different IPs.}
{Paste EACH selected IP profile's English identity lock verbatim. Attach all required reference images, deduplicating shared files.}
The reference locks identity, anatomy, proportions and character colors only. Render it as flat 2D hand-drawn ink. Do not inherit 3D lighting, materials, background, pose, text or watermark. Preserve the active character's specific body shape and features; do not substitute another IP such as Xiaohei.

Visual language:
Pure white background, fine slightly wobbly black pen lines, sparse composition, generous quiet white space. Each selected character retains its own profile palette; do not transfer colors or anatomy between characters. Props are unfilled black outlines, no gray fill. Tiny red notes for emphasis, blue for secondary notes, optional orange line for movement only. No gradients, shadows, paper texture, commercial vector polish, realistic UI, dense course-slide layout or cute decorative treatment.

Core idea:
{One accurate idea from the source.}

Scene and conceptual action:
{What each character physically does, which 1–2 objects are involved, what changes and why this represents the idea. Respect each character's anatomy. Naidan is limbless: use rolling, leaning, supporting, pressing or blocking, not grasping tools.}

Composition:
{Arrange for the selected ratio. Identify the core scene, any short heading, nearby labels, optional conclusion and a quiet white area. For a list, specify why it is needed and what action the character demonstrates.}
{For scene mode: main scene about 40–60% of canvas, aim for at least 35% white space.}

Visible text whitelist:
EXACTLY these words, no other text:
{Each approved visible text string on its own line, including any numbering.}
{If no text is needed, replace the whitelist instruction with: No visible text, letters, numbers or signatures.}

Constraints:
Explain one core idea through the scene. The character must cause or sustain the key action, not merely stand beside labels. Keep the character identity stable; do not transform its body into a device or add limbs. Do not write internal structure-type names, invent captions, watermarks or signatures. Invent a fresh visual metaphor for this content; do not copy reference scenes or prior case compositions. Question headings are allowed when requested or useful; no mandatory title box, bullet list or bottom slogan.
```

## 局部修改

明确要改的区域和文字，要求保留其余角色、场景、笔触与比例。文字严重出错时先减字再重生成；双比例输出分别使用构图描述，不能让模型机械拉伸旧图。
