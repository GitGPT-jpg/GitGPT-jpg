# Jiang Cheng / 江承

**Language:** [English](#english) · [中文](#chinese)

---

<a id="english"></a>

## English

Most of what I build is about getting AI to *do* things — not respond, execute.

Not chat interfaces. Workflows.

Specifically: pulling information from multiple sources, running it through analysis, generating reports, pushing output somewhere useful. Stringing together steps that would otherwise require someone sitting there manually coordinating each one.

I came up in telecom engineering delivery — field work, integration, operations. That background shows up in how I think about systems:

- Will this still run at 3am?
- What happens when step 4 of 7 fails?
- How does the system recover, and what state is it in when it does?

After you deploy a few AI pipelines in practice, the interesting problems stop being "which model" and start being: state management, retry logic, tool-call stability, long-task execution, context management, workflow orchestration.

That's where most of my attention is now.

**Stack**  
Python · FastAPI · Node.js · TypeScript · Next.js · Electron · SQLite · Docker

---

### Some things I built

**[latam-intel-bot](https://github.com/GitGPT-jpg/latam-intel-bot)**  
Automated intelligence workflow for Latin America news monitoring. The problem is easy to describe: collect → normalize → analyze → deliver. Making it run reliably across 35 RSS feeds and 5 APIs without constant babysitting was the actual work.

**[android-llm-agent](https://github.com/GitGPT-jpg/android-llm-agent)**  
Android automation agent using ADB + OCR + LLM for multi-step UI task execution. Building this made clear that the hard parts of agents aren't the model — they're state, tool-call chains, error recovery, and what to do when the UI doesn't look like what the model expected.

**[voice-companion-agent](https://github.com/GitGPT-jpg/voice-companion-agent)**  
Conversational agent with persistent memory, dynamic persona, and TTS/RVC voice. The interesting part is session-to-session consistency — how do you maintain a coherent identity across separate conversations?

**[jianghu-nightrain](https://github.com/GitGPT-jpg/jianghu-nightrain)**  
Electron + Next.js productivity system. RPG-style goal tracking with AI-assisted planning. Local-first.

---

### What I've come to think

Most AI systems don't fail because the model wasn't good enough.

They fail because:
- The workflow around the model wasn't designed for failure
- State wasn't tracked properly
- No one thought about what happens when step 4 of 7 times out

The engineering layer is where most of the real work lives.

---

[@GitGPT-jpg](https://github.com/GitGPT-jpg)

---

<a id="chinese"></a>

## 中文

我折腾的大部分东西，都是让 AI 去"执行事情"，而不是聊天。

不是对话框，是工作流。

具体来说：从多个来源采集信息，经过分析处理，生成报告，推送到目标位置。把那些原本需要有人盯着手动协调的步骤，串成一条自动跑的流程。

我做工程交付出身 —— 通信行业，现场，集成，运维。这个背景会影响我看系统的方式：

- 这个东西凌晨三点还能跑吗？
- 第 4 步失败了，后面怎么办？
- 系统怎么恢复，恢复后处于什么状态？

真正部署过几条 AI 流水线之后，有趣的问题就不再是"用哪个模型"了。

变成了：状态管理、重试逻辑、工具调用稳定性、长任务执行、上下文管理、workflow orchestration。

这些是我现在主要花注意力的地方。

**技术栈**  
Python · FastAPI · Node.js · TypeScript · Next.js · Electron · SQLite · Docker

---

### 做过的一些东西

**[latam-intel-bot](https://github.com/GitGPT-jpg/latam-intel-bot)**  
拉美新闻监控的自动化情报工作流。要解决的问题很容易描述：采集 → 标准化 → 分析 → 推送。真正的工作是让它跑在 35 个 RSS 源和 5 个 API 上，不需要人持续盯着。

**[android-llm-agent](https://github.com/GitGPT-jpg/android-llm-agent)**  
基于 ADB + OCR + LLM 的 Android 多步骤 UI 自动化 Agent。做这个项目之后越来越清楚：Agent 难的部分不是模型，是状态、工具调用链路、错误恢复，以及 UI 和模型预期不符时怎么办。

**[voice-companion-agent](https://github.com/GitGPT-jpg/voice-companion-agent)**  
有持久记忆、动态人设和 TTS/RVC 语音的对话 Agent。有意思的部分在于跨会话的一致性 —— 怎么在不同对话之间维持连贯的"身份"。

**[jianghu-nightrain](https://github.com/GitGPT-jpg/jianghu-nightrain)**  
Electron + Next.js 效率系统。RPG 风格目标追踪 + AI 辅助规划。本地优先。

---

### 逐渐形成的一些判断

大部分 AI 系统最后失败，不是因为模型不够强。

而是：
- 模型外面的 workflow 没有为失败做设计
- 状态没有正确追踪
- 没人想过第 4 步超时后会发生什么

工程层，才是大部分真正工作所在的地方。

---

[@GitGPT-jpg](https://github.com/GitGPT-jpg)