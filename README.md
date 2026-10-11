# awesome-photo-skills

> 将照片变成插画、海报、Zine、旅行卡片与更多艺术作品的 AI Agent Skills 精选目录。

A curated collection of AI agent skills that transform photos into illustrations, posters, zines, postcards, and more.

按视觉风格整理可复用的照片创作技能，附原仓库、实际 Skill 入口、效果介绍和许可证说明。优先收录包含 `SKILL.md` 的项目，并将多风格合集、内部预设、工作流和辅助工具分开标注。

**收录快照：2026-10-11 · 79 个相关仓库 · 108 个已核验的相关 `SKILL.md` · 98 个已整理的内部风格／构图预设。**

这些数字不代表 108 或 206 种独立照片风格：Skill 明细包含路由与审核功能，预设属于现有 Skill 的内部选项。仓库数量也包含少量索引、生成后端及需要适配照片输入的插画工具。

本目录核对了 README、相关 `SKILL.md` 和可取得的许可证文件，尚未逐项运行或评测生成效果。链接指向上游当前版本；功能、路径及授权可能随版本变化。

## 快速开始

| 想做什么 | 推荐入口 |
| --- | --- |
| 找独立的照片风格 Skill | [GZ-L/photo-to-poster-skills](https://github.com/GZ-L/photo-to-poster-skills)：14 项，覆盖水彩、厚涂、纸雕、像素等 |
| 按照片内容自动选择海报风格 | [PosterLoom](https://github.com/liuweispace/posterloom-sklls)：29 个直接风格契约与 1 个混合契约 |
| 做撕纸拼贴或照片语义提炼 | [Gathered Scenes](https://github.com/Zeejay0/gathered-scenes-zine-skill)：两条主线，注意当前个人非商业许可 |
| 浏览样图并发现更多仓库 | [skill-zine-summary](https://github.com/tluy/skill-zine-summary)：附样图与原仓库链接的索引 |
| 只想使用本地代码处理 | [halftone-riso-pop](https://github.com/Zhang-ym92/halftone-riso-pop)：Python/Pillow 网点印刷；另见[代码绘画](#code) |

安装方式、宿主兼容性与模型配置请以各上游仓库为准。多数风格 Skill 提供艺术指导和提示词规则，实际出图仍需要宿主的图像生成／编辑能力；部分项目只返回提示词，或使用单独的 API 与本地渲染工具。

## 目录

- [多风格合集](#collections)
- [纸艺、拼贴与 Zine](#zine)
- [极简与抽象](#minimal)
- [照片与插画双联](#diptych)
- [旅行卡片、明信片与贴纸](#travel)
- [水彩、钢笔与手绘](#painting)
- [东方水墨](#ink)
- [版画、Riso 与网点印刷](#print)
- [印章与记忆档案](#archive)
- [扁平与几何插画](#flat)
- [超现实与波普拼贴](#surreal)
- [真实照片加涂鸦](#doodle)
- [人像、宠物与 IP](#portrait)
- [像素与 CRT](#pixel)
- [摄影、胶片与电影](#cinema)
- [文化、建筑与物件设计](#objects)
- [艺术指导与系列工作流](#workflow)
- [扩展插画预设](#illustration-library)
- [代码绘画与本地渲染](#code)
- [生成后端、提示词与索引](#resources)
- [许可证与整合说明](#licensing)
- [收录与贡献](#contributing)

<a id="collections"></a>

## 多风格合集

一个仓库覆盖多种视觉方向。独立 Skill 与内部风格预设分别列出。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [GZ-L/photo-to-poster-skills](https://github.com/GZ-L/photo-to-poster-skills) | 已核验 14 个相关 Skill，见下方明细 | 14 个独立 Skill；水彩、厚涂、纸雕、像素、水粉、木刻等 | [MIT](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/LICENSE) |
| [haorantang97/antibes-holiday](https://github.com/haorantang97/antibes-holiday) | 已核验 3 个相关 Skill，见下方明细 | 当前 README 称 LabArt：松散钢笔画、颗粒像素重构、冷幽默涂鸦 | [PolyForm Noncommercial](https://github.com/haorantang97/antibes-holiday/blob/HEAD/LICENSE) |
| [lincotalk/linco-skills](https://github.com/lincotalk/linco-skills) | 已核验 3 个相关 Skill，见下方明细 | 照片意义海报、旅行贴纸卡、Gathered Zine 三项相关 Skill | [MIT](https://github.com/lincotalk/linco-skills/blob/HEAD/LICENSE) |
| [liuweispace/posterloom-sklls](https://github.com/liuweispace/posterloom-sklls) | [`posterloom`](https://github.com/liuweispace/posterloom-sklls/blob/HEAD/posterloom/SKILL.md)；30 个内部预设／模式 | 1 个 posterloom Skill；29 个直接风格契约与 1 个混合契约 | [MIT](https://github.com/liuweispace/posterloom-sklls/blob/HEAD/LICENSE) |

<details>
<summary>GZ-L/photo-to-poster-skills：已核验 Skill 明细</summary>

| Skill 源文件 | 效果或职责 |
| --- | --- |
| [`charcoal-fading-travel-study`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/charcoal-fading-travel-study/SKILL.md) | 炭笔旅行研究稿与消散留白 |
| [`clean-ink-zen-memory`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/clean-ink-zen-memory/SKILL.md) | 黑墨块、点描与象牙纸禅意记忆 |
| [`folk-ink-landmark-portrait`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/folk-ink-landmark-portrait/SKILL.md) | 民俗墨彩式地标肖像 |
| [`gouache-travel-still-life`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/gouache-travel-still-life/SKILL.md) | 不透明水粉旅行静物或场景 |
| [`impasto-miniature-landscape`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/impasto-miniature-landscape/SKILL.md) | 雕塑感厚涂油画微缩风景 |
| [`isometric-healing-blocks`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/isometric-healing-blocks/SKILL.md) | 圆润等轴积木式治愈场景 |
| [`kraft-stencil-landmark`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/kraft-stencil-landmark/SKILL.md) | 牛皮纸上的双色镂空模板地标 |
| [`memory-diary-duet`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/memory-diary-duet/SKILL.md) | 真实照片与水彩彩铅日记双联 |
| [`nostalgic-travel-duet`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/nostalgic-travel-duet/SKILL.md) | 怀旧旅行极简双联 |
| [`observational-pen-wash`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/observational-pen-wash/SKILL.md) | 观察式钢笔淡彩速写 |
| [`paper-cutout-travel-figures`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/paper-cutout-travel-figures/SKILL.md) | 真实背景中的白色剪纸人物 |
| [`papercraft-travel-diorama`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/papercraft-travel-diorama/SKILL.md) | 有纸张触感的旅行纸雕微缩景观 |
| [`pixel-dissolve-landscape`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/pixel-dissolve-landscape/SKILL.md) | 有限色像素景观向纸白消散 |
| [`watercolor-travel-card`](https://github.com/GZ-L/photo-to-poster-skills/blob/HEAD/skills/watercolor-travel-card/SKILL.md) | 整张水彩旅行卡，邮票齿孔式边缘 |

</details>

<details>
<summary>haorantang97/antibes-holiday：已核验 Skill 明细</summary>

| Skill 源文件 | 效果或职责 |
| --- | --- |
| [`antibes-holiday`](https://github.com/haorantang97/antibes-holiday/blob/HEAD/plugins/antibes-holiday/skills/antibes-holiday/SKILL.md) | 松散黑色钢笔线与假日插画 |
| [`deadpan-doodles`](https://github.com/haorantang97/antibes-holiday/blob/HEAD/plugins/deadpan-doodles/skills/deadpan-doodles/SKILL.md) | 冷幽默人物或宠物钢笔淡彩 |
| [`tephra`](https://github.com/haorantang97/antibes-holiday/blob/HEAD/plugins/tephra/skills/tephra/SKILL.md) | 颗粒、抖动像素式图像重构及动画 |

</details>

> **haorantang97/antibes-holiday 说明：** 仓库 README 已使用 LabArt 名称；此处保留检索到的仓库地址。

<details>
<summary>lincotalk/linco-skills：已核验 Skill 明细</summary>

| Skill 源文件 | 效果或职责 |
| --- | --- |
| [`journey-sticker-card`](https://github.com/lincotalk/linco-skills/blob/HEAD/journey-sticker-card/SKILL.md) | 3:2 大场景插画与六枚贴纸、三组关键词 |
| [`meaning-led-photo-poster`](https://github.com/lincotalk/linco-skills/blob/HEAD/meaning-led-photo-poster/SKILL.md) | 上半真实照片、下半意义提炼的 3:4 海报 |
| [`photo-gathered-zine`](https://github.com/lincotalk/linco-skills/blob/HEAD/photo-gathered-zine/SKILL.md) | 3:5 真实照片锚点与撕纸拼贴 |

</details>

> **lincotalk/linco-skills 说明：** 含其他 Zine 方案的来源关联；核验上游版本和授权链。

<details>
<summary>liuweispace/posterloom-sklls：30 个内部风格／构图预设</summary>

这些是同一 Skill 或风格家族内部的选项，不另计为独立 Skill。

| 所属 Skill／家族 | 预设 |
| --- | --- |
| `posterloom` / Photography | `Cinematic Editorial`、`Moody Night Editorial`、`Travel Cover Poster`、`Luxury Still-Life Editorial`、`Documentary Poster` |
| `posterloom` / Painterly | `Transparent Watercolor`、`Soft Gouache`、`Expressive Painting`、`Ink Wash Minimal`、`Pastel Atmosphere` |
| `posterloom` / Print | `Pop Screenprint`、`Riso Poster`、`Relief Print`、`Retro Lithograph`、`Paper-Cut Graphic` |
| `posterloom` / Oriental | `Neo Ink Poster`、`Tea-House Minimal`、`Classical Parchment`、`Seal & Calligraphy Poster`、`Folk Narrative Color` |
| `posterloom` / Abstract | `Editorial Surrealism`、`Abstract Editorial`、`Minimal Symbolic Poster`、`Collage-Lite Narrative` |
| `posterloom` / Modern | `Swiss Grid Poster`、`Brutalist Poster`、`Neo-Futurist Layout`、`Geometric Color-Block`、`Elegant Serif Poster` |
| `posterloom` / Meta | `Controlled Hybrid` |

</details>

<a id="zine"></a>

## 纸艺、拼贴与 Zine

撕纸边缘、纸张肌理、照片锚点、剪纸与杂志式编排。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [MuziGeek/mz-minimal-zine-reconstruction](https://github.com/MuziGeek/mz-minimal-zine-reconstruction) | [`mz-minimal-zine-reconstruction`](https://github.com/MuziGeek/mz-minimal-zine-reconstruction/blob/HEAD/mz-minimal-zine-reconstruction/SKILL.md)；4 个内部预设／模式 | 4 个模式：视觉岛、撕纸揭示、照片档案叠层、剪贴档案 | [MIT](https://github.com/MuziGeek/mz-minimal-zine-reconstruction/blob/HEAD/LICENSE) |
| [Zeejay0/gathered-scenes-zine-skill](https://github.com/Zeejay0/gathered-scenes-zine-skill) | 已核验 2 个相关 Skill，见下方明细 | 保留照片的撕纸拼贴，以及彻底重绘的语义提炼插画，两条主线 | [个人非商业许可](https://github.com/Zeejay0/gathered-scenes-zine-skill/blob/HEAD/LICENSE) |
| [jas0nh/zine-poster-skill](https://github.com/jas0nh/zine-poster-skill) | [`zine`](https://github.com/jas0nh/zine-poster-skill/blob/HEAD/SKILL.md) | 1 个 zine Skill，minimal/scenes/editorial 三路；scenes 可保留或提炼照片 | [MIT](https://github.com/jas0nh/zine-poster-skill/blob/HEAD/LICENSE) |
| [liuzihe849-png/silhouette-group-collage](https://github.com/liuzihe849-png/silhouette-group-collage) | [`silhouette-group-collage`](https://github.com/liuzihe849-png/silhouette-group-collage/blob/HEAD/silhouette-group-collage/SKILL.md) | 真实人物群像与上下正负纸剪影拼贴 | [MIT](https://github.com/liuzihe849-png/silhouette-group-collage/blob/HEAD/LICENSE) |
| [sherlyryn/make-tape-collage](https://github.com/sherlyryn/make-tape-collage) | [`make-tape-collage`](https://github.com/sherlyryn/make-tape-collage/blob/HEAD/SKILL.md) | 和纸胶带拼贴，可结合原图；含本地合成流程 | [MIT](https://github.com/sherlyryn/make-tape-collage/blob/HEAD/LICENSE) |
| [wnby/paper-spirit-zine](https://github.com/wnby/paper-spirit-zine) | [`paper-spirit-zine`](https://github.com/wnby/paper-spirit-zine/blob/HEAD/skills/paper-spirit-zine/SKILL.md) | 真实照片与具生命感的纸面余像、地景或动物形态 | 未确认 |
| [yanghaoraneve/torn-photo-window-sketch-zine-skill](https://github.com/yanghaoraneve/torn-photo-window-sketch-zine-skill) | [`torn-photo-window-sketch-zine`](https://github.com/yanghaoraneve/torn-photo-window-sketch-zine-skill/blob/HEAD/SKILL.md) | 撕开的照片窗口与同透视石墨素描连续连接 | 未确认 |

<details>
<summary>MuziGeek/mz-minimal-zine-reconstruction：4 个内部风格／构图预设</summary>

这些是同一 Skill 或风格家族内部的选项，不另计为独立 Skill。

| 所属 Skill／家族 | 预设 |
| --- | --- |
| `mz-minimal-zine-reconstruction` / 构图模式 | `visual-islands`、`torn-reveal`、`archive-over-photo`、`scrapbook-archive` |

</details>

<details>
<summary>Zeejay0/gathered-scenes-zine-skill：已核验 Skill 明细</summary>

| Skill 源文件 | 效果或职责 |
| --- | --- |
| [`scene-distillation-zine-v1-3`](https://github.com/Zeejay0/gathered-scenes-zine-skill/blob/HEAD/skills/scene-distillation-zine-v1-3/SKILL.md) | 不保留原照片像素；将语义完整提炼成极简插画 |
| [`scenes-gathered-zine-v1-3`](https://github.com/Zeejay0/gathered-scenes-zine-skill/blob/HEAD/skills/scenes-gathered-zine-v1-3/SKILL.md) | 保留真实摄影锚点、撕纸边与同源抽象插画 |

</details>

> **jas0nh/zine-poster-skill 说明：** 含其他 Zine 方案的来源关联；核验上游版本和授权链。

<a id="minimal"></a>

## 极简与抽象

将照片提炼成少量形状、视觉隐喻、留白与编辑排版。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [121dyy/dyy_photo_deconstruct](https://github.com/121dyy/dyy_photo_deconstruct) | [`dyy_photo_deconstruct`](https://github.com/121dyy/dyy_photo_deconstruct/blob/HEAD/SKILL.md) | 旧纸、剪影、墨色水彩；无文字场景解构 | 未确认 |
| [LiamGvchi/gc-minimal-zine-poster](https://github.com/LiamGvchi/gc-minimal-zine-poster) | [`gc-minimal-zine-poster-v0-3`](https://github.com/LiamGvchi/gc-minimal-zine-poster/blob/HEAD/SKILL.md) | 纸纹、大片留白、小型拼贴、实验字体与单一强调色 | [MIT](https://github.com/LiamGvchi/gc-minimal-zine-poster/blob/HEAD/LICENSE) |
| [dacnay816y62-hub/FANTASY-Minimal-Magazine](https://github.com/dacnay816y62-hub/FANTASY-Minimal-Magazine) | [`fantasy-minimal-magazine`](https://github.com/dacnay816y62-hub/FANTASY-Minimal-Magazine/blob/HEAD/SKILL.md) | 极简杂志、抽象图形与编辑排版 | 未确认 |
| [iamkong/photo-to-minimal-illustration](https://github.com/iamkong/photo-to-minimal-illustration) | [`gc-universal-field-study`](https://github.com/iamkong/photo-to-minimal-illustration/blob/HEAD/SKILL.md) | 奶油色留白、照片主体重绘为极简田野研究插画 | [MIT](https://github.com/iamkong/photo-to-minimal-illustration/blob/HEAD/LICENSE) |
| [wnby/photo-relic-editorial](https://github.com/wnby/photo-relic-editorial) | [`photo-relic-editorial`](https://github.com/wnby/photo-relic-editorial/blob/HEAD/SKILL.md) | 照片和极简抽象印刷遗物组成编辑画面 | [MIT](https://github.com/wnby/photo-relic-editorial/blob/HEAD/LICENSE) |

<a id="diptych"></a>

## 照片与插画双联

同一来源的真实照片与插画、抽象画或纸面研究稿并置。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [Evianis/travel-photo-abstraction](https://github.com/Evianis/travel-photo-abstraction) | [`travel-photo-abstraction`](https://github.com/Evianis/travel-photo-abstraction/blob/HEAD/travel-photo-abstraction/SKILL.md) | 真实照片与同源抽象插画并置 | [自定义：禁止修改与再分发](https://github.com/Evianis/travel-photo-abstraction/blob/HEAD/LICENSE) |
| [Yu-0312/paper-echo-photo-cards](https://github.com/Yu-0312/paper-echo-photo-cards) | [`photo-to-art-card`](https://github.com/Yu-0312/paper-echo-photo-cards/blob/HEAD/skill/photo-to-art-card/SKILL.md) | 纸面印刷研究稿或照片与轻盈插画双联 | [MIT](https://github.com/Yu-0312/paper-echo-photo-cards/blob/HEAD/LICENSE) |
| [ZzzLc0405/photo-abstract-editorial](https://github.com/ZzzLc0405/photo-abstract-editorial) | [`photo-abstract-editorial`](https://github.com/ZzzLc0405/photo-abstract-editorial/blob/HEAD/SKILL.md) | 忠实照片与抽象记忆画面并置 | 未确认 |
| [wnby/travel-photo-soft-abstraction](https://github.com/wnby/travel-photo-soft-abstraction) | [`travel-photo-soft-abstraction`](https://github.com/wnby/travel-photo-soft-abstraction/blob/HEAD/skills/travel-photo-soft-abstraction/SKILL.md) | 保留照片并配柔和、可辨认的来源抽象画 | 未确认 |
| [zhouaria28-cloud/photo-ink-echo](https://github.com/zhouaria28-cloud/photo-ink-echo) | [`photo-ink-echo`](https://github.com/zhouaria28-cloud/photo-ink-echo/blob/HEAD/SKILL.md) | 上部照片、下部小幅淡水彩与大留白 | [MIT](https://github.com/zhouaria28-cloud/photo-ink-echo/blob/HEAD/LICENSE) |

> **Yu-0312/paper-echo-photo-cards 说明：** 代码或说明的许可证不代表示例图片和第三方素材许可。

<a id="travel"></a>

## 旅行卡片、明信片与贴纸

适合旅行记录、月度回忆、明信片与贴纸套装。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [Whiplashzeb/photo-to-zine-postcard](https://github.com/Whiplashzeb/photo-to-zine-postcard) | [`photo-to-zine-postcard`](https://github.com/Whiplashzeb/photo-to-zine-postcard/blob/HEAD/SKILL.md) | 照片与来源元素组成双面 Zine 明信片 | [MIT](https://github.com/Whiplashzeb/photo-to-zine-postcard/blob/HEAD/LICENSE) |
| [carolinaaafy/travel-memory-card-duo](https://github.com/carolinaaafy/travel-memory-card-duo) | [`travel-memory-card-duo`](https://github.com/carolinaaafy/travel-memory-card-duo/blob/HEAD/SKILL.md) | 旅行插画卡与相同 6 枚贴纸的透明 PNG，双文件输出 | 未确认 |
| [carolinaaafy/travel-memory-sticker-card](https://github.com/carolinaaafy/travel-memory-sticker-card) | [`travel-memory-sticker-card`](https://github.com/carolinaaafy/travel-memory-sticker-card/blob/HEAD/SKILL.md) | 旅行插画主场景、6 枚模切贴纸与关键词 | [个人使用；禁止未经许可打包再分发](https://github.com/carolinaaafy/travel-memory-sticker-card/blob/HEAD/LICENSE) |
| [kaijie-czyh/pocket-postcard-skill](https://github.com/kaijie-czyh/pocket-postcard-skill) | [`pocket-postcard-v0-1`](https://github.com/kaijie-czyh/pocket-postcard-skill/blob/HEAD/SKILL.md) | 旧明信片、手写文字、邮戳与旅行记忆 | [MIT](https://github.com/kaijie-czyh/pocket-postcard-skill/blob/HEAD/LICENSE) |
| [maikeliu86-coder/handdrawn-postcard-skill](https://github.com/maikeliu86-coder/handdrawn-postcard-skill) | [`handdrawn-postcard`](https://github.com/maikeliu86-coder/handdrawn-postcard-skill/blob/HEAD/handdrawn-postcard/SKILL.md) | 水彩、Riso、丝网、凸版、蓝晒、复印拼贴等手绘明信片 | [MIT](https://github.com/maikeliu86-coder/handdrawn-postcard-skill/blob/HEAD/LICENSE) |
| [shenchangyi/photo-to-monthly-zine-postcard](https://github.com/shenchangyi/photo-to-monthly-zine-postcard) | [`photo-to-monthly-zine-postcard`](https://github.com/shenchangyi/photo-to-monthly-zine-postcard/blob/HEAD/skills/photo-to-monthly-zine-postcard/SKILL.md) | 照片、水彩、月份与书影音内容组成月度 Zine 明信片 | [MIT](https://github.com/shenchangyi/photo-to-monthly-zine-postcard/blob/HEAD/LICENSE) |

> **maikeliu86-coder/handdrawn-postcard-skill 说明：** 代码或说明的许可证不代表示例图片和第三方素材许可。

<a id="painting"></a>

## 水彩、钢笔与手绘

松散速写、铅笔、水彩、钢笔和选择性细节。更多水彩、水粉、厚涂油画见多风格合集中的 GZ-L 与 PosterLoom。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [dacnay816y62-hub/photo-revival](https://github.com/dacnay816y62-hub/photo-revival) | [`photo-revival`](https://github.com/dacnay816y62-hub/photo-revival/blob/HEAD/SKILL.md) | 照片转大留白中的小幅铅笔水彩记忆画 | [MIT](https://github.com/dacnay816y62-hub/photo-revival/blob/HEAD/LICENSE) |
| [joeyhu1108-maker/selective-ink-sketch](https://github.com/joeyhu1108-maker/selective-ink-sketch) | [`selective-ink-sketch`](https://github.com/joeyhu1108-maker/selective-ink-sketch/blob/HEAD/SKILL.md) | 选择性细节钢笔素描，主体精画、其余留白 | 未确认 |
| [liigoQi/photo-to-travel-sketch](https://github.com/liigoQi/photo-to-travel-sketch) | [`photo-to-travel-sketch`](https://github.com/liigoQi/photo-to-travel-sketch/blob/HEAD/SKILL.md) | 松散针管笔与干性灰马克笔，旅行现场速写 | [MIT](https://github.com/liigoQi/photo-to-travel-sketch/blob/HEAD/LICENSE) |

<a id="ink"></a>

## 东方水墨

东方留白、水墨笔触与照片双联。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [Hiseaa/eastern-ink-photo-diptych](https://github.com/Hiseaa/eastern-ink-photo-diptych) | [`eastern-ink-photo-diptych`](https://github.com/Hiseaa/eastern-ink-photo-diptych/blob/HEAD/eastern-ink-photo-diptych.zip) | 上方照片、下方东方水墨双联；Skill 以仓库 ZIP 发布 | 未确认 |
| [TwentyfiveBTea/ink-wash-poster](https://github.com/TwentyfiveBTea/ink-wash-poster) | [`ink-wash-poster`](https://github.com/TwentyfiveBTea/ink-wash-poster/blob/HEAD/SKILL.md) | 现代极简水墨海报 | [AGPL-3.0](https://github.com/TwentyfiveBTea/ink-wash-poster/blob/HEAD/LICENSE) |

> **Hiseaa/eastern-ink-photo-diptych 说明：** 已读取 ZIP 内实际 SKILL.md；不是仅根据 README 推断。

<a id="print"></a>

## 版画、Riso 与网点印刷

少色印刷、套色偏移、网点、复古制版与印刷肌理。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [Zhang-ym92/halftone-riso-pop](https://github.com/Zhang-ym92/halftone-riso-pop) | [`halftone-riso-pop`](https://github.com/Zhang-ym92/halftone-riso-pop/blob/HEAD/SKILL.md) | 本地 Python/Pillow 双色网点、错版和边缘线处理 | [MIT](https://github.com/Zhang-ym92/halftone-riso-pop/blob/HEAD/LICENSE) |
| [liuzihe849-png/ai-editorial-print-studio](https://github.com/liuzihe849-png/ai-editorial-print-studio) | [`editorial-illustration-generator`](https://github.com/liuzihe849-png/ai-editorial-print-studio/blob/HEAD/SKILL.md) | editorial-illustration-generator：复古印刷编辑插画 | [MIT](https://github.com/liuzihe849-png/ai-editorial-print-studio/blob/HEAD/LICENSE) |
| [luckdvr/photo-riso-poster](https://github.com/luckdvr/photo-riso-poster) | [`photo-riso-poster`](https://github.com/luckdvr/photo-riso-poster/blob/HEAD/SKILL.md) | 分析照片后用文字重新生成 2–3 色 Riso 档案海报；不直接发送参考图 | [MIT](https://github.com/luckdvr/photo-riso-poster/blob/HEAD/LICENSE) |
| [v92388375-gif/pixel-style-poster-skill](https://github.com/v92388375-gif/pixel-style-poster-skill) | [`pixel-style-poster-skill`](https://github.com/v92388375-gif/pixel-style-poster-skill/blob/HEAD/SKILL.md) | 点阵与网点编辑海报；不是游戏像素风 | [MIT](https://github.com/v92388375-gif/pixel-style-poster-skill/blob/HEAD/LICENSE) |
| [yanliudesign/mono-color-skill](https://github.com/yanliudesign/mono-color-skill) | [`mono-color`](https://github.com/yanliudesign/mono-color-skill/blob/HEAD/SKILL.md) | 单色或双色编辑印刷风格；资源另有授权说明 | [MIT](https://github.com/yanliudesign/mono-color-skill/blob/HEAD/LICENSE) |

> **yanliudesign/mono-color-skill 说明：** 代码或说明的许可证不代表示例图片和第三方素材许可。

<a id="archive"></a>

## 印章与记忆档案

照片、橡皮章、手账、色卡与档案式版面。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [Dlcccc71913/skill-make-photo-stamp-archive](https://github.com/Dlcccc71913/skill-make-photo-stamp-archive) | [`make-photo-stamp-archive`](https://github.com/Dlcccc71913/skill-make-photo-stamp-archive/blob/HEAD/SKILL.md) | 真实照片与小型印章、档案式白色版面 | [MIT](https://github.com/Dlcccc71913/skill-make-photo-stamp-archive/blob/HEAD/LICENSE) |
| [Mr-funny/hbg-rubber-stamp-field-note](https://github.com/Mr-funny/hbg-rubber-stamp-field-note) | [`hbg-rubber-stamp-field-note`](https://github.com/Mr-funny/hbg-rubber-stamp-field-note/blob/HEAD/skill/hbg-rubber-stamp-field-note/SKILL.md) | 左侧照片、右侧少色橡皮章或木刻式图案 | [MIT](https://github.com/Mr-funny/hbg-rubber-stamp-field-note/blob/HEAD/LICENSE) |
| [sbj61188-lab/compose-photo-memory-archive](https://github.com/sbj61188-lab/compose-photo-memory-archive) | [`compose-photo-memory-archive`](https://github.com/sbj61188-lab/compose-photo-memory-archive/blob/HEAD/SKILL.md) | 保留原照片，配水彩小稿、三色色卡与空白手账行 | [MIT](https://github.com/sbj61188-lab/compose-photo-memory-archive/blob/HEAD/LICENSE) |

<a id="flat"></a>

## 扁平与几何插画

大色块、简化轮廓、几何构成与稚拙插画。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [CreateLafont/dnr-flat-pic](https://github.com/CreateLafont/dnr-flat-pic) | [`dnr-flat-pic`](https://github.com/CreateLafont/dnr-flat-pic/blob/HEAD/SKILL.md) | 高饱和、大留白、扁平插画；PNG，可另行描摹 SVG | [MIT](https://github.com/CreateLafont/dnr-flat-pic/blob/HEAD/LICENSE) |
| [nevertoday/xxd-panel-017](https://github.com/nevertoday/xxd-panel-017) | [`xxd-panel-017`](https://github.com/nevertoday/xxd-panel-017/blob/HEAD/SKILL.md) | 韩系稚拙扁平插画；上下、左右、纯设计、壁纸四种输出 | [PolyForm Noncommercial](https://github.com/nevertoday/xxd-panel-017/blob/HEAD/LICENSE) |
| [wen3140/sunwoven-reverie](https://github.com/wen3140/sunwoven-reverie) | [`sunwoven-reverie`](https://github.com/wen3140/sunwoven-reverie/blob/HEAD/sunwoven-reverie/SKILL.md) | 现代扁平几何、宽阔色块与约 10–14 色调色板 | [PolyForm Noncommercial](https://github.com/wen3140/sunwoven-reverie/blob/HEAD/LICENSE) |

<a id="surreal"></a>

## 超现实与波普拼贴

尺度错置、戏剧布景、趣味物件与高饱和色彩。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [2998980-hue/surreal-pop-collage](https://github.com/2998980-hue/surreal-pop-collage) | [`surreal-pop-collage`](https://github.com/2998980-hue/surreal-pop-collage/blob/HEAD/SKILL.md) | 黑白摄影主体、饱和色块、超大不可能物体 | [MIT](https://github.com/2998980-hue/surreal-pop-collage/blob/HEAD/LICENSE) |
| [dacnay816y62-hub/fantasy-qiqiguaiguai-skill](https://github.com/dacnay816y62-hub/fantasy-qiqiguaiguai-skill) | [`fantasy-qiqiguaiguai`](https://github.com/dacnay816y62-hub/fantasy-qiqiguaiguai-skill/blob/HEAD/SKILL.md) | 人物编辑、物件拼贴、照片叠加三条趣味路线 | [MIT](https://github.com/dacnay816y62-hub/fantasy-qiqiguaiguai-skill/blob/HEAD/LICENSE) |
| [luji12/daily-photo-playground](https://github.com/luji12/daily-photo-playground) | [`daily-photo-playground`](https://github.com/luji12/daily-photo-playground/blob/HEAD/SKILL.md) | 高饱和情绪几何重构，加小型照片窗口 | 未确认 |
| [traveler0621/reality-restaged](https://github.com/traveler0621/reality-restaged) | [`reality-restaged`](https://github.com/traveler0621/reality-restaged/blob/HEAD/SKILL.md) | 照片改为高饱和超现实剧场布景，保留人物识别线索 | 未确认 |

<a id="doodle"></a>

## 真实照片加涂鸦

保留真实摄影环境，叠加手绘角色、线条或局部重绘。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [Hchen1218/heytea-style](https://github.com/Hchen1218/heytea-style) | [`heytea-doodle-poster`](https://github.com/Hchen1218/heytea-style/blob/HEAD/SKILL.md) | 真实食物、饮料照片叠加黑色手绘与趣味角色 | [MIT](https://github.com/Hchen1218/heytea-style/blob/HEAD/LICENSE) |
| [dacnay816y62-hub/street-photo-illustration-skill](https://github.com/dacnay816y62-hub/street-photo-illustration-skill) | [`street-photo-illustration`](https://github.com/dacnay816y62-hub/street-photo-illustration-skill/blob/HEAD/SKILL.md) | 保留真实街景，将人物重绘为黑墨或彩色 Q 版 | 未确认 |
| [luji12/handdrawn-photo-poster](https://github.com/luji12/handdrawn-photo-poster) | [`handdrawn-photo-poster`](https://github.com/luji12/handdrawn-photo-poster/blob/HEAD/SKILL.md) | 压暗照片与鲜亮手绘邮票块，或书页式编排 | 未确认 |
| [shouna12358-png/heytea-creative-style](https://github.com/shouna12358-png/heytea-creative-style) | [`heytea-style`](https://github.com/shouna12358-png/heytea-creative-style/blob/HEAD/skills/heytea-style/SKILL.md) | 真实食物加趣味手绘，提供两版文字排版 | [MIT](https://github.com/shouna12358-png/heytea-creative-style/blob/HEAD/LICENSE) |
| [zhu930824/poetic-line-zine-poster](https://github.com/zhu930824/poetic-line-zine-poster) | [`poetic-line-zine-poster`](https://github.com/zhu930824/poetic-line-zine-poster/blob/HEAD/SKILL.md) | 照片、炭笔粗线与单一彩色随手线条组合 | 未确认 |

> **Hchen1218/heytea-style 说明：** 代码或说明的许可证不代表示例图片和第三方素材许可。

<a id="portrait"></a>

## 人像、宠物与 IP

头像、动漫化、Q 版角色、宠物画像与角色衍生物。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [EverettFish/ip_illustration_for_yourself](https://github.com/EverettFish/ip_illustration_for_yourself) | [`ip-illustration-character-system`](https://github.com/EverettFish/ip_illustration_for_yourself/blob/HEAD/SKILL.md) | 人物或宠物转统一 Q 版 IP，衍生贴纸、头像、表情与照片融合 | 未确认 |
| [Lcxiv/portrait-skill](https://github.com/Lcxiv/portrait-skill) | [`portrait`](https://github.com/Lcxiv/portrait-skill/blob/HEAD/SKILL.md)；32 个内部预设／模式 | 32 个预设：5 摄影增强、7 卡通、20 动漫；依赖 Gemini API | 未确认 |
| [adrianpunk/Punk-Skill](https://github.com/adrianpunk/Punk-Skill) | 已核验 2 个相关 Skill，见下方明细 | 本表核验 punk-avatar 与 punk-ip-video-cover；头像 Skill 含 7 种预设 | [当前版本个人非商业许可](https://github.com/adrianpunk/Punk-Skill/blob/HEAD/LICENSE) |

<details>
<summary>Lcxiv/portrait-skill：32 个内部风格／构图预设</summary>

这些是同一 Skill 或风格家族内部的选项，不另计为独立 Skill。

| 所属 Skill／家族 | 预设 |
| --- | --- |
| `portrait` / 摄影增强 | `studio-classic`、`studio-warm`、`editorial`、`outdoor-natural`、`startup-ceo` |
| `portrait` / 卡通 | `pixar`、`comic-pop`、`watercolor`、`oil-painting`、`flat-vector`、`caricature`、`chibi` |
| `portrait` / 动漫 | `ghibli`、`shinkai`、`jjk`、`demon-slayer`、`chainsaw-man`、`spy-x-family`、`aot`、`jojo`、`edgerunners`、`promare`、`dbz`、`sailor-moon`、`akira`、`redline`、`mob-psycho`、`ping-pong`、`mononoke-tv`、`tatami-galaxy`、`violet-evergarden`、`satoshi-kon` |

</details>

> **Lcxiv/portrait-skill 说明：** 需要 Gemini API 配置及可能的调用费用；未实测效果。

<details>
<summary>adrianpunk/Punk-Skill：已核验 Skill 明细</summary>

| Skill 源文件 | 效果或职责 |
| --- | --- |
| [`punk-avatar`](https://github.com/adrianpunk/Punk-Skill/blob/HEAD/skills/punk-avatar/SKILL.md) | 人物或宠物头像，7 种风格预设 |
| [`punk-ip-video-cover`](https://github.com/adrianpunk/Punk-Skill/blob/HEAD/skills/punk-ip-video-cover/SKILL.md) | 人物 IP 与视频封面 |

</details>

<details>
<summary>adrianpunk/Punk-Skill：7 个内部风格／构图预设</summary>

这些是同一 Skill 或风格家族内部的选项，不另计为独立 Skill。

| 所属 Skill／家族 | 预设 |
| --- | --- |
| `punk-avatar` / 头像与插画 | `pixel-avatar`、`grotesque-soul-sketch`、`messy-crayon-pet-portrait`、`fashion-sketch-observation`、`polaroid-keepsake`、`minimal-paper-acrylic-block-illustration`、`surreal-pop-up-paper-landscape` |

</details>

<a id="pixel"></a>

## 像素与 CRT

8-bit、复古显示器、荧光栅格、余辉与翻拍质感。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [TaiT-tt/tait-crt-interface-skill](https://github.com/TaiT-tt/tait-crt-interface-skill) | [`tait-crt-interface-skill`](https://github.com/TaiT-tt/tait-crt-interface-skill/blob/HEAD/SKILL.md) | 复古 CRT、Mac、Minitel 界面与像素肖像 | 未确认 |
| [TwentyfiveBTea/8bit-pixel-art](https://github.com/TwentyfiveBTea/8bit-pixel-art) | [`8bit-pixel-art`](https://github.com/TwentyfiveBTea/8bit-pixel-art/blob/HEAD/SKILL.md) | 照片语义重绘为疏朗的 8-bit 像素编辑插画 | [AGPL-3.0](https://github.com/TwentyfiveBTea/8bit-pixel-art/blob/HEAD/LICENSE) |
| [fihaaade/skills](https://github.com/fihaaade/skills) | [`phosphor-relay-style`](https://github.com/fihaaade/skills/blob/HEAD/phosphor-relay-style/SKILL.md) | phosphor-relay-style：CRT 荧光屏、像素栅格、余辉与翻拍感 | 未确认 |

<a id="cinema"></a>

## 摄影、胶片与电影

胶片色调、夜景氛围、慢快门、电影静帧与电影海报。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [N1kO724/kodak-2383-film-look](https://github.com/N1kO724/kodak-2383-film-look) | [`kodak-2383-film-look`](https://github.com/N1kO724/kodak-2383-film-look/blob/HEAD/skills/kodak-2383-film-look/SKILL.md) | Kodak 2383 灵感胶片色调及前后对照；非官方校准 LUT | [MIT](https://github.com/N1kO724/kodak-2383-film-look/blob/HEAD/LICENSE) |
| [Nealsun1993/neil-night-skill](https://github.com/Nealsun1993/neil-night-skill) | [`neil-monochrome-night-v0-1`](https://github.com/Nealsun1993/neil-night-skill/blob/HEAD/SKILL.md) | 青蓝单色夜景、雾气、暖色实景灯与电影氛围 | [MIT](https://github.com/Nealsun1993/neil-night-skill/blob/HEAD/LICENSE) |
| [Nealsun1993/neil-quentin](https://github.com/Nealsun1993/neil-quentin) | [`neil-quentin`](https://github.com/Nealsun1993/neil-quentin/blob/HEAD/SKILL.md) | 90 年代通俗电影印刷海报，强对比与少色印刷 | [MIT](https://github.com/Nealsun1993/neil-quentin/blob/HEAD/LICENSE) |
| [dacnay816y62-hub/cinema-dna-21x9x3](https://github.com/dacnay816y62-hub/cinema-dna-21x9x3) | [`cinema-dna-21x9x3`](https://github.com/dacnay816y62-hub/cinema-dna-21x9x3/blob/HEAD/SKILL.md) | 参考照片或素材转电影静帧、三联图和故事板 | 未确认 |
| [dacnay816y62-hub/fantasy-movie-poster-skill](https://github.com/dacnay816y62-hub/fantasy-movie-poster-skill) | [`fantasy-movie-poster`](https://github.com/dacnay816y62-hub/fantasy-movie-poster-skill/blob/HEAD/SKILL.md) | 故事与参考素材生成原创中文电影海报；需适配照片入口 | 未确认 |
| [lzs0594/dreamy-motion-editorial](https://github.com/lzs0594/dreamy-motion-editorial) | [`dreamy-motion-editorial`](https://github.com/lzs0594/dreamy-motion-editorial/blob/HEAD/SKILL.md) | 梦幻雾化、慢快门、运动模糊编辑摄影；诊断与提示词，可继续生成 | [MIT](https://github.com/lzs0594/dreamy-motion-editorial/blob/HEAD/LICENSE) |

<a id="objects"></a>

## 文化、建筑与物件设计

建筑与工艺海报、材质艺术、色板及黑胶唱片包装。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [dacnay816y62-hub/culture-fragment-poster-engine](https://github.com/dacnay816y62-hub/culture-fragment-poster-engine) | [`culture-fragment-poster-engine`](https://github.com/dacnay816y62-hub/culture-fragment-poster-engine/blob/HEAD/SKILL.md) | 文化、建筑、器物碎片转主视觉与文化海报 | 未确认 |
| [joeyhu1108-maker/ZONE-Material-art](https://github.com/joeyhu1108-maker/ZONE-Material-art) | [`zone-material-art`](https://github.com/joeyhu1108-maker/ZONE-Material-art/blob/HEAD/SKILL.md) | 参考图转材质拼贴、浮雕、装置式艺术方向；提示词导向 | 未确认 |
| [laurent-7bk/Aigc-Skills](https://github.com/laurent-7bk/Aigc-Skills) | [`create-pantone-photo-posters`](https://github.com/laurent-7bk/Aigc-Skills/blob/HEAD/create-pantone-photo-posters/SKILL.md) | create-pantone-photo-posters：照片越框、提取色板和近似色号标签 | 未确认 |
| [liigoQi/vinyl-image-generator](https://github.com/liigoQi/vinyl-image-generator) | [`vinyl-image-generator`](https://github.com/liigoQi/vinyl-image-generator/blob/HEAD/SKILL.md) | 照片或记忆转虚构黑胶唱片四件套包装 | [MIT](https://github.com/liigoQi/vinyl-image-generator/blob/HEAD/LICENSE) |
| [op7418/guizang-yingzao-skill](https://github.com/op7418/guizang-yingzao-skill) | [`yingzao`](https://github.com/op7418/guizang-yingzao-skill/blob/HEAD/yingzao/SKILL.md) | yingzao：中式建筑、地点、工艺照片转文化艺术海报 | 未确认 |

<a id="workflow"></a>

## 艺术指导与系列工作流

选片、风格路由、系列一致性与质量审核；这些是工作流能力，并非都对应独立视觉风格。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [N1kO724/scene-to-art-lab](https://github.com/N1kO724/scene-to-art-lab) | [`scene-to-art-lab`](https://github.com/N1kO724/scene-to-art-lab/blob/HEAD/scene-to-art-lab/SKILL.md) | 从照片主体与情绪出发，自适应选择海报艺术方向 | [个人非商业许可](https://github.com/N1kO724/scene-to-art-lab/blob/HEAD/LICENSE) |
| [jiahuiqu17/paper-signal](https://github.com/jiahuiqu17/paper-signal) | 已核验 4 个相关 Skill，见下方明细 | 路由、单张艺术指导、2–10 张系列、质量审核四个工作流 Skill | [MIT](https://github.com/jiahuiqu17/paper-signal/blob/HEAD/LICENSE) |
| [karenlamb6082-ctrl/travel-photo-art-director-skill](https://github.com/karenlamb6082-ctrl/travel-photo-art-director-skill) | [`travel-photo-art-director`](https://github.com/karenlamb6082-ctrl/travel-photo-art-director-skill/blob/HEAD/skills/travel-photo-art-director/SKILL.md) | 旅行照片目录选片、预编辑、系列化混合媒介艺术指导 | [MIT](https://github.com/karenlamb6082-ctrl/travel-photo-art-director-skill/blob/HEAD/LICENSE) |

<details>
<summary>jiahuiqu17/paper-signal：已核验 Skill 明细</summary>

| Skill 源文件 | 效果或职责 |
| --- | --- |
| [`paper-signal-art-director`](https://github.com/jiahuiqu17/paper-signal/blob/HEAD/skills/paper-signal-art-director/SKILL.md) | 单张照片艺术指导 |
| [`paper-signal-audit`](https://github.com/jiahuiqu17/paper-signal/blob/HEAD/skills/paper-signal-audit/SKILL.md) | 系列和单张的质量审核 |
| [`paper-signal-series`](https://github.com/jiahuiqu17/paper-signal/blob/HEAD/skills/paper-signal-series/SKILL.md) | 2–10 张照片的统一系列设计 |
| [`paper-signal`](https://github.com/jiahuiqu17/paper-signal/blob/HEAD/skills/paper-signal/SKILL.md) | 照片艺术工作流路由 |

</details>

<a id="illustration-library"></a>

## 扩展插画预设

以主题生图为主的插画风格库，纳入照片工作流时需要补充照片分析与主体保留规则。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [yokel1121/muyang-illustration-skills](https://github.com/yokel1121/muyang-illustration-skills) | 已核验 9 个相关 Skill，见下方明细 | 9 个 Skill：1 路由与 8 风格家族，25 预设；偏主题生图，照片需适配 | [MIT](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/LICENSE) |

<details>
<summary>yokel1121/muyang-illustration-skills：已核验 Skill 明细</summary>

| Skill 源文件 | 效果或职责 |
| --- | --- |
| [`muyang-cinematic-narrative`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-cinematic-narrative/SKILL.md) | 清冷夏日、童话巨宠 |
| [`muyang-dark-fashion`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-dark-fashion/SKILL.md) | 暗调黑红、暗黑韩系、暗黑冷光 |
| [`muyang-editorial-minimal`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-editorial-minimal/SKILL.md) | 精致极简、极简现代、极简冰蓝 |
| [`muyang-fashion-colorblock`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-fashion-colorblock/SKILL.md) | 蓝白时尚、韩系蓝白、黄黑撞色、粉蓝撞色 |
| [`muyang-illustration`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-illustration/SKILL.md) | 主路由：选择八个家族中的风格 |
| [`muyang-oriental-poetry`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-oriental-poetry/SKILL.md) | 庭院手绘、东方青绿、极简墨灰 |
| [`muyang-print-poster`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-print-poster/SKILL.md) | 复古剪影、复古电影、日式版画 |
| [`muyang-soft-dream`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-soft-dream/SKILL.md) | 复古柔焦、柔焦烟灰、梦幻鎏金、梦幻彩虹、柔焦霓虹 |
| [`muyang-white-couture`](https://github.com/yokel1121/muyang-illustration-skills/blob/HEAD/skills/muyang-white-couture/SKILL.md) | 柔纱纯白、华丽银灰 |

</details>

<details>
<summary>yokel1121/muyang-illustration-skills：25 个内部风格／构图预设</summary>

这些是同一 Skill 或风格家族内部的选项，不另计为独立 Skill。

| 所属 Skill／家族 | 预设 |
| --- | --- |
| `muyang-cinematic-narrative` / 插画预设 | `清冷夏日`、`童话巨宠` |
| `muyang-dark-fashion` / 插画预设 | `暗调黑红`、`暗黑韩系`、`暗黑冷光` |
| `muyang-editorial-minimal` / 插画预设 | `精致极简`、`极简现代`、`极简冰蓝` |
| `muyang-fashion-colorblock` / 插画预设 | `蓝白时尚`、`韩系蓝白`、`黄黑撞色`、`粉蓝撞色` |
| `muyang-oriental-poetry` / 插画预设 | `庭院手绘`、`东方青绿`、`极简墨灰` |
| `muyang-print-poster` / 插画预设 | `复古剪影`、`复古电影`、`日式版画` |
| `muyang-soft-dream` / 插画预设 | `复古柔焦`、`柔焦烟灰`、`梦幻鎏金`、`梦幻彩虹`、`柔焦霓虹` |
| `muyang-white-couture` / 插画预设 | `柔纱纯白`、`华丽银灰` |

</details>

<a id="code"></a>

## 代码绘画与本地渲染

使用 SVG、HTML/CSS、Python 等生成画面；不一定依赖图像生成模型，也不一定是直接的照片滤镜。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [Buantum/flash4start_light](https://github.com/Buantum/flash4start_light) | [`painterly-svg-repaint`](https://github.com/Buantum/flash4start_light/blob/HEAD/.agents/skills/painterly-svg-repaint/SKILL.md) | painterly-svg-repaint：照片转油画笔触式 SVG；代码生成路线 | 未确认 |
| [cloveric/claude-drawing-skill](https://github.com/cloveric/claude-drawing-skill) | [`claude绘图`](https://github.com/cloveric/claude-drawing-skill/blob/HEAD/SKILL.md) | 程序化绘画多风格资源；当前 README 列 67 风格，非现成照片转换器 | [MIT](https://github.com/cloveric/claude-drawing-skill/blob/HEAD/LICENSE) |
| [yangcodingmaster/photo-distill](https://github.com/yangcodingmaster/photo-distill) | [`photo-distill`](https://github.com/yangcodingmaster/photo-distill/blob/HEAD/SKILL.md) | 照片语义转极简印刷设计，以 HTML/CSS/SVG 和浏览器渲染 | 未确认 |

<a id="resources"></a>

## 生成后端、提示词与索引

帮助发现风格或执行图像生成的辅助资源，单独列出，不与照片风格 Skill 混算。

| 仓库 | Skill／规模 | 效果与用途 | 许可证 |
| --- | --- | --- | --- |
| [ConardLi/garden-skills](https://github.com/ConardLi/garden-skills) | [`gpt-image-2`](https://github.com/ConardLi/garden-skills/blob/HEAD/skills/gpt-image-2/SKILL.md) | 仅收录 gpt-image-2；通用图像生成及案例库，非专门照片风格包 | [MIT](https://github.com/ConardLi/garden-skills/blob/HEAD/LICENSE) |
| [YouMind-OpenLab/ai-image-prompts-skill](https://github.com/YouMind-OpenLab/ai-image-prompts-skill) | [`ai-image-prompts-skill`](https://github.com/YouMind-OpenLab/ai-image-prompts-skill/blob/HEAD/SKILL.md) | 1 个提示词推荐 Skill，仓库宣称 10000+ 提示词；不是同等数量的 Skill | [MIT](https://github.com/YouMind-OpenLab/ai-image-prompts-skill/blob/HEAD/LICENSE) |
| [tluy/skill-zine-summary](https://github.com/tluy/skill-zine-summary) | 资源索引，不是 Skill 安装包 | 自述 58 项，样图与原仓库链接；含重复项与未开源项，不是安装包 | 未确认 |

> **YouMind-OpenLab/ai-image-prompts-skill 说明：** 代码或说明的许可证不代表示例图片和第三方素材许可。

<a id="licensing"></a>

## 许可证与整合说明

表中的许可标签是本次收录时对上游文件的摘要，不替代完整许可证。**收录链接不等于获得复制、修改、再分发或商业使用的授权。**

| 标签 | 整合时如何处理 |
| --- | --- |
| MIT | 可优先评估源码整合；保留版权声明和许可证，另查示例图片、字体、其他素材与上游衍生内容的条款。 |
| AGPL-3.0 | 单独保留并遵守其许可证义务，不将其统一改标为 MIT。 |
| 个人非商业许可 | 按具体条款检查使用者范围、商业用途与再分发条件；优先仅收录链接。 |
| PolyForm Noncommercial | 按完整非商业条款处理，不视作通用商业可用授权。 |
| 自定义／禁止再分发 | 仅收录链接；复制进合集前取得符合用途的许可。 |
| 未确认 | 本次未确认许可证，不等于确定无许可证，也不代表允许自由复制；合并源码前进一步核实。 |

### 需要特别留意的项目

- [Gathered Scenes 当前 LICENSE](https://github.com/Zeejay0/gathered-scenes-zine-skill/blob/HEAD/LICENSE) 为个人非商业许可；不要依据旧版本或第三方介绍推定最新版为 MIT。
- [Punk-Skill 当前 LICENSE](https://github.com/adrianpunk/Punk-Skill/blob/HEAD/LICENSE) 与历史版本的授权应分开核对。
- [travel-photo-abstraction](https://github.com/Evianis/travel-photo-abstraction/blob/HEAD/LICENSE) 当前自定义条款限制修改与再分发。
- [travel-memory-sticker-card](https://github.com/carolinaaafy/travel-memory-sticker-card/blob/HEAD/LICENSE) 限制未经许可打包再分发。
- `zine-poster-skill` 与 `linco-skills` 等存在其他 Zine 方案的来源关联；除根目录许可证外，还需核验所采用上游版本的授权链。

本目录只提供介绍和上游链接，不重新发布上游 Skill 源码或示例图片，也不为这些项目赋予统一许可证。未来如引入源码，建议为每项记录原仓库、固定 commit、原许可证、修改说明与素材授权。

<a id="contributing"></a>

## 收录与贡献

欢迎提交新的照片风格 Skill、补充效果示例链接，或修正失效链接、功能描述与许可证信息。

新增项目请提供：

1. 原始仓库链接与实际 `SKILL.md` 路径；同源镜像优先指向原作者。
2. 风格分类，以及照片会被保留、局部编辑还是完全重绘。
3. 一句话效果介绍，必要时附上游展示页或前后对比链接。
4. 图像生成／编辑模型、API 或本地运行依赖。
5. 许可证文件链接、素材例外与最近核验日期。

请区分独立 Skill、内部预设、提示词案例和辅助工具；避免把同一项目的镜像、历史版本或别名重复计数。新增条目只代表资料收录，不代表效果评测或维护状态背书。

感谢所有上游作者。每个项目的作者、维护方式与最新条款请通过原仓库查看。
