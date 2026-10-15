# Awesome Photo Skills

**从一张照片，找到下一种表达。**

照片 → 水彩 · 纸雕 · Zine · 明信片 · 像素 · 电影感

A curated collection of AI agent skills for turning photos into art.

[选择风格](#choose) · [对比演示](#examples) · [完整目录](docs/catalog.md) · [使用方式](#start) · [参与贡献](CONTRIBUTING.md)

> 收录快照 **2026-10-11**：79 个相关仓库 / 108 个已核验的相关 `SKILL.md` / 98 个内部预设。三者不是同一种计数，也不等于独立照片风格数量。此次整理日期：2026-10-15。

<a id="examples"></a>

## 先看效果

对比演示按 **同一张输入图 → 不同 Skill 的独立输出图** 组织，方便比较主体保留、材质和构图变化。

本次计划先制作水彩旅行卡、纸雕微缩场景、像素消散三组对比。**共享输入图已生成，三种转换暂未成功**：参考图转换接口返回 429，当前没有可展示的前后对比结果。

<a href="examples/images/source.png"><img src="examples/images/source.png" alt="AI 生成的虚构湖岸输入图：小屋、柏树与木船" width="320"></a>

*共享输入图 · AI 生成的虚构场景，非实拍照片。*

| 演示方向 | 重点观察 | 准备状态 |
| --- | --- | --- |
| 水彩旅行卡 | 透明水彩、纸纹与侧边档案栏 | [提示词已准备](examples/prompts/watercolor.md)，转换待重试 |
| 纸雕微缩场景 | 纸层厚度、立体空间与留白 | [提示词已准备](examples/prompts/papercraft.md)，转换待重试 |
| 像素消散 | 主体识别、有限色阶与边缘消散 | [提示词已准备](examples/prompts/pixel.md)，转换待重试 |

[查看演示方案与来源记录 →](examples/README.md)

<a id="choose"></a>

## 按你想要的效果选

| 创作方向 | 分类入口 |
| --- | --- |
| 纸张与手作 | [纸艺 / 拼贴 / Zine](docs/catalog/zine.md) · [旅行卡片 / 明信片 / 贴纸](docs/catalog/travel.md) · [印章 / 记忆档案](docs/catalog/archive.md) |
| 绘画与抽象 | [水彩 / 钢笔 / 手绘](docs/catalog/painting.md) · [东方水墨](docs/catalog/ink.md) · [极简 / 抽象](docs/catalog/minimal.md) · [扁平 / 几何](docs/catalog/flat.md) |
| 照片与插画混合 | [照片与插画双联](docs/catalog/diptych.md) · [真实照片加涂鸦](docs/catalog/doodle.md) · [超现实 / 波普拼贴](docs/catalog/surreal.md) |
| 印刷与影像 | [版画 / Riso / 网点](docs/catalog/print.md) · [像素 / CRT](docs/catalog/pixel.md) · [摄影 / 胶片 / 电影](docs/catalog/cinema.md) |
| 特定主体 | [人像 / 宠物 / IP](docs/catalog/portrait.md) · [文化 / 建筑 / 物件](docs/catalog/objects.md) |
| 多风格与工作流 | [多风格合集](docs/catalog/collections.md) · [艺术指导 / 系列工作流](docs/catalog/workflow.md) · [扩展插画预设](docs/catalog/illustration-library.md) |
| 工具与资源 | [代码绘画 / 本地渲染](docs/catalog/code.md) · [生成后端 / 提示词 / 索引](docs/catalog/resources.md) |

## 不知道从哪里开始？

| 你的需求 | 推荐入口 | 选择理由 |
| --- | --- | --- |
| 一次浏览多种独立风格 | [photo-to-poster-skills](docs/catalog/collections.md) | 14 个独立 Skill，覆盖水彩、厚涂、纸雕、像素等 |
| 让工具按照片选择风格 | [PosterLoom](https://github.com/liuweispace/posterloom-sklls) | 29 个直接风格契约与 1 个混合契约 |
| 做撕纸拼贴或语义提炼 | [Gathered Scenes](docs/catalog/zine.md) | 保留摄影与完全重绘两条主线；个人非商业许可 |
| 浏览上游样图 | [skill-zine-summary](https://github.com/tluy/skill-zine-summary) | 带样图与原仓库链接的资源索引 |
| 用本地代码处理照片 | [代码绘画与本地渲染](docs/catalog/code.md) | 集中查看本地渲染路线；不同项目能力各异 |

<a id="start"></a>

## 怎么使用

1. **选效果**：从分类页查看项目介绍，打开实际 `SKILL.md` 链接。
2. **查依赖和许可**：按上游说明确认宿主、模型、API 或本地工具要求。
3. **提供照片并调用 Skill**：在支持该技能的宿主中上传照片，说明希望保留的主体和期望输出。

多数风格 Skill 提供艺术指导和提示词规则，出图仍依赖宿主的图像生成／编辑能力；部分项目只返回提示词。本仓库是精选目录，不是统一安装包，没有适用于所有项目的安装命令。

## 目录里有什么

```text
README.md              首页：选择风格与演示入口
CONTRIBUTING.md         收录规则与演示贡献要求
docs/
  catalog.md           全部分类索引
  catalog/             20 个分类的完整条目与预设
  licensing.md         许可证说明与特殊条款
examples/
  README.md            对比演示方案、状态和素材规则
  manifest.json        来源、版本与生成状态
  prompts/             输入图与三种转换的提示词
  images/              已生成的共享输入图
```

## 收录边界

目录在原收录时核对了 README、相关 `SKILL.md` 和可取得的许可证文件，未逐项运行评测。链接一般指向上游当前版本；功能、路径和授权可能变化。独立 Skill、内部预设、路由审核工作流与辅助工具分别标注。

[许可证与整合说明](docs/licensing.md) · [收录与贡献](CONTRIBUTING.md)

<details>
<summary>原 README 分类链接兼容入口</summary>

<a id="collections"></a>

[多风格合集](docs/catalog/collections.md)

<a id="zine"></a>

[纸艺、拼贴与 Zine](docs/catalog/zine.md)

<a id="minimal"></a>

[极简与抽象](docs/catalog/minimal.md)

<a id="diptych"></a>

[照片与插画双联](docs/catalog/diptych.md)

<a id="travel"></a>

[旅行卡片、明信片与贴纸](docs/catalog/travel.md)

<a id="painting"></a>

[水彩、钢笔与手绘](docs/catalog/painting.md)

<a id="ink"></a>

[东方水墨](docs/catalog/ink.md)

<a id="print"></a>

[版画、Riso 与网点印刷](docs/catalog/print.md)

<a id="archive"></a>

[印章与记忆档案](docs/catalog/archive.md)

<a id="flat"></a>

[扁平与几何插画](docs/catalog/flat.md)

<a id="surreal"></a>

[超现实与波普拼贴](docs/catalog/surreal.md)

<a id="doodle"></a>

[真实照片加涂鸦](docs/catalog/doodle.md)

<a id="portrait"></a>

[人像、宠物与 IP](docs/catalog/portrait.md)

<a id="pixel"></a>

[像素与 CRT](docs/catalog/pixel.md)

<a id="cinema"></a>

[摄影、胶片与电影](docs/catalog/cinema.md)

<a id="objects"></a>

[文化、建筑与物件设计](docs/catalog/objects.md)

<a id="workflow"></a>

[艺术指导与系列工作流](docs/catalog/workflow.md)

<a id="illustration-library"></a>

[扩展插画预设](docs/catalog/illustration-library.md)

<a id="code"></a>

[代码绘画与本地渲染](docs/catalog/code.md)

<a id="resources"></a>

[生成后端、提示词与索引](docs/catalog/resources.md)

<a id="licensing"></a>

[许可证与整合说明](docs/licensing.md)

<a id="contributing"></a>

[收录与贡献](CONTRIBUTING.md)

</details>

感谢所有上游作者。作者、维护方式与最新条款请通过原仓库查看。
