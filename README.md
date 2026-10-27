# PUP 2.0
### A Desktop Creature with Its Own Life

**一个生活在 Windows 桌面上、拥有自主行为的轻量 AI 角色。**

**项目类型**：角色交互设计 / 自主行为设计 / AI 辅助原型开发  
**平台与工具**：Windows · Godot (.NET / C#) · Blender · Optional AI API  
**当前状态**：原型持续开发中（Prototype in Development）

---

## 项目概述 · Overview

Pup 是一只生活在 Windows 桌面空间里的数字生物。用户专注于自己的事情时，Pup 仍有自身的状态、注意力、活动和休息节奏；当用户触摸、拖动、召唤或与它交谈时，它会根据当前情境作出回应，然后回到自己的生活。

项目围绕一个交互设计问题展开：

> **如何设计一个具有自主性、行为连续性和社交边界的陪伴角色？**

Pup is a lightweight desktop creature designed around **autonomy, behavioral continuity, and respectful social boundaries**. It alternates between quiet peripheral presence and direct user interaction, without requiring constant attention.

## 核心交互 · Key Interactions

| 设计方向 | 原型中的表现 |
| --- | --- |
| **自主生活 / Autonomous Life** | 内部 Energy、Curiosity、Connection、Settledness 等状态影响观察、探索、移动、休息及活动选择 |
| **自主活动 / Self-initiated Activities** | 在合适条件下可选择跳舞（Dance）或追逐临时出现的蝴蝶（Butterfly Chase） |
| **即时互动 / Direct Interaction** | 点击触摸、拖动与释放、附近双击召唤至指定桌面位置 |
| **注意力与身体表达 / Embodied Expression** | 眼神、表情、身体形变、移动与疲劳状态相互协调 |
| **状态连续性 / State Continuity** | 清醒、困倦、休息、醒来具有连续的表现过程；睡眠中的普通触摸与拖动保留同一次休息生命周期 |
| **社交边界 / Social Boundaries** | 有限的主动关注尝试；用户未回应时结束尝试，不将其解释为关系惩罚 |
| **可选 AI 认知 / Optional AI** | 在明确授权与运行时约束内生成语言、情绪和合法行动选择；AI 不可用时本地自主行为仍继续 |

Pup 的**自主追蝴蝶**与**用户触发的鼠标交互**来自不同的行为机制。当前鼠标互动包含召唤、触摸、拖动与有限注视；不将它描述为独立的持续追鼠标活动。

## 行为设计方法 · Design Approach

**Internal State → Goal / Activity Selection → Action & Presentation → Real Outcome → State Update**

- 内部状态与人格倾向影响自主行动，但不把单个数值直接映射为固定动画。
- 活动由实际的生命周期和执行结果管理。Dance 与 Butterfly Chase 属于短期活动：中断后结束，不自动续做。
- 用户的直接操作和执行安全边界优先于普通自主活动。
- 行为经历可参与短时情感评价；例如“跳舞”并不固定等于“开心”。

## 我的职责 · My Role

负责项目概念、角色交互目标、行为规则与边界、设计合同及持续迭代；通过实际桌面原型观察动作节奏、身体表达和交互衔接问题，提出修改并进行开发者验收。

原型采用 **AI-assisted programming（AI 辅助编程）**方式开发。我负责设计决策、需求与规则定义、调试集成及体验判断；不将 AI 生成代码表述为全部由本人手写。

## 当前进度 · Project Status

- **已接入**：本地生命与目标系统、Dance / Butterfly Chase 活动、主要鼠标交互、桌面运动、部分眼睛/情感表达及休息生命周期。
- **已进行**：开发者本机交互与视觉检查、部分自动化回归验证。
- **仍在进行**：真实桌面长期体验调校、部分边界场景验收、Dance 持续时间与部分活动语义优化。
- **尚未开展**：正式外部用户测试；长期记忆和关系成长也不属于当前已交付能力。

因此，本仓库展示的是**开发中的设计原型**，并不宣称已经验证长期陪伴或心理健康效果。

## Windows 原型与演示 · Download & Demo

**Windows 独立运行包：[下载 v0.1.0-preview（Windows x64）](https://github.com/pupupu20000107/pup2-showcase/releases/tag/v0.1.0-preview)**  
包含独立运行文件、使用说明、第三方许可证声明与 SHA-256 校验文件。

实际运行截图、交互演示以及作品集PDF将逐步补充。此公开仓库用于**项目展示与原型分发**，不包含完整的私人开发源码或内部工作记录。

## 隐私与使用说明 · Privacy & Usage

当前版本不提供通用截图、屏幕内容识别、摄像头监控或任意键盘/剪贴板内容采集。可选 AI 功能需要用户自行配置支持的 API；发布包不会包含项目开发者的 API 密钥。

**This is a design portfolio showcase, not an open-source code release.** No reuse license is granted unless stated separately.
