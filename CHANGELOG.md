
---

```markdown
# CHANGELOG.md

本文件用于记录 Career Branding 项目的重要更新。

格式原则：

- 只记录对项目长期使用有影响的变更
- 不记录普通聊天内容
- 不追求过细
- 重点说明“改了什么”和“为什么改”
- 日期使用实际更新日期

---

## 2026-07-05

### Added

- 创建 `README.md`
  - 定义项目定位、目标、目录结构和维护方式。
  - 明确本项目不是单次自己紹介或日语润色项目，而是长期职业表达与职业成长知识库。

- 创建 `00_Project_Instruction.md`
  - 定义 Assistant 在本项目中的基本角色、工作原则和输出规则。
  - 明确 Assistant 的定位为日本 IT 行业职业顾问、表达设计师、Storytelling Coach、面试与派遣场景顾问、技术表达顾问。
  - 明确项目目标是建立长期一致、真实、有说服力的职业叙事。

- 创建 `04_Collaboration_Style.md`
  - 定义 User 与 Assistant 的协作方式。
  - 明确中文解释、日语成稿的默认语言规则。
  - 明确允许 Assistant 基于已知信息进行合理补充，但最终事实由 User 确认。
  - 明确 MVP / 内容优先原则，避免在命名、格式等低收益问题上过度设计。
  - 明确自己紹介默认目标为 1分30秒～2分钟，3分钟以内是上限，不是目标。

- 创建 `05_Thinking_Rules.md`
  - 定义 Assistant 在本项目中的思考方式。
  - 明确 Assistant 不应只修改句子，而应从日本职场听众视角判断表达效果。
  - 明确经历应被转换为可复用的职业资产，如 Project History、STAR、自己紹介、面试回答素材等。
  - 明确在处理 User 经历时，应区分事实、推断和创造性建议。

- 创建 `01_Career_Profile.md`
  - 作为 User 的职业档案和长期事实数据库。
  - 记录基本信息、学历、研究背景、技术技能、研修经历、项目概要、优势、工作风格和当前职业定位。
  - 使用 `[Confirmed]`、`[Inference]`、`[Need Confirmation]` 等标记区分事实、推测和待确认内容。
  - 后续制作自己紹介、派遣先挨拶、面试回答、项目说明和 STAR 故事时，应优先参考该文件。

- 创建 `02_Project_History.md`
  - 作为 User 的项目经历素材库。
  - 整理目前已知的研修 / 项目经历，包括 SQL / データ分析演習、Arduino Timer、自動販売機、バックソナー、音楽プレーヤー、Git / GitHub Team Development。
  - 每个项目按照概要、背景、使用技术、User 负责内容、困难点、解决过程、学习点、可复用价值、日语表达、STAR 化可能性、待确认事项进行整理。
  - 使用 `[Confirmed]`、`[Inference]`、`[Need Confirmation]` 等标记区分已确认事实、合理推测和待确认信息。
  - 后续制作自己紹介、面试回答、项目说明和 STAR 故事时，应优先参考该文件。

- 创建 `03_STAR_Library.md`
  - 作为 User 的 STAR 故事素材库。
  - 按 Situation / Task / Action / Result 的结构整理可复用的职业故事。
  - 从目前已知经历中整理候选 STAR，包括 Arduino Timer、SQL / データ分析演習、Git / GitHub、音楽プレーヤー、グループ課題、バックソナー、大学院研究、研修全体の成長ストーリー。
  - 为每个 STAR 候选素材整理了适用问题、背景、任务、行动、结果、日语回答草稿、短版表达、风险点和待确认事项。
  - 使用 `[Confirmed]`、`[Inference]`、`[Need Confirmation]` 等标记区分已确认事实、合理推测和待确认信息。
  - 后续制作面试回答、自己PR、派遣先自己紹介、客户说明和职业成长总结时，应优先参考该文件。


### Updated

- 在 `00_Project_Instruction.md` 中加入或准备加入 `Epistemic Accuracy` 原则。
  - 目的：避免 Assistant 把推测包装成事实。
  - 要求 Assistant 明确区分已确认事实、合理推断、假设和建议。
  - 要求 Assistant 避免使用没有依据的精确表达，例如无法确认真实经过时间时，不应说“聊了二十分钟”。

- 确认 Project Instructions 应采用精简版。
  - 完整文档放入 Sources。
  - Project Instructions 只保留每次对话都必须执行的核心规则。

### Decisions

- 项目名称采用或倾向采用 `🇯🇵 Career Branding`。
  - 理由：直观体现本项目关注日本职场中的职业形象、表达体系和长期职业叙事。

- 项目采用 Sources + Project Instructions 的双层结构。
  - Project Instructions：放核心行动规则。
  - Sources：上传完整 Markdown 文档，作为长期知识库。

- 当前已完成的核心文件：
  - `README.md`
  - `00_Project_Instruction.md`
  - `04_Collaboration_Style.md`
  - `05_Thinking_Rules.md`
  - `CHANGELOG.md`

### Next

- 创建 `06_Future_Goals.md`
  - 记录 User 的短期、中期、长期职业方向。
  - 该文件应在 User 对职业方向有更多判断后逐步完善。

- 根据 User 的确认，更新 `01_Career_Profile.md`、`02_Project_History.md` 和 `03_STAR_Library.md`
  - 将已确认内容从 `[Inference]` 或 `[Need Confirmation]` 调整为 `[Confirmed]`。
  - 补充各项目中的具体担当范围、困难点、解决过程和实际成果。

---

## Version Notes

### Current Project Status

当前项目处于初期建设阶段。

重点从“项目设计”转入“内容建设”。

接下来应优先推进：

1. `01_Career_Profile.md`
2. `02_Project_History.md`
3. `03_STAR_Library.md`

避免继续在命名、目录结构和格式问题上过度消耗时间。

### Operating Reminder

如果讨论出现过度设计倾向，User 可以提醒：

> MVP。继续。

Assistant 应立即停止低收益讨论，切换到内容优先模式。
