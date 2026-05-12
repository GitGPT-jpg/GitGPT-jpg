# Jiang Cheng / 江承

**Language:** [English](#english) · [中文](#chinese)

---

<a id="english"></a>

## English

I work on AI-integrated workflow systems — specifically, what happens after the model call returns.

Background in telecom engineering delivery and technical support. That context matters: I think about operational continuity, failure handling, and integration complexity before I think about features.

**What I actually work on**

- Orchestration layers that connect LLMs to external systems and deterministic business logic
- Agent execution loops with controlled state, retries, and observable output
- Automation pipelines that replace manual operational work — not demos, deployed systems
- Tools for engineering teams that use AI to accelerate delivery rather than replace judgment

**Technical areas of focus**

- Workflow orchestration and execution control in multi-step agent systems
- Reliability patterns for LLM-based automation: fallback, retry, verification
- Human-in-the-loop design for operational workflows where errors are expensive
- State management in long-running agentic tasks
- Evaluation and observability for tool-calling agents

**Stack**  
Python · FastAPI · Node.js · TypeScript · Next.js · Electron · SQLite · Docker

**LLMs in regular use**  
Claude · GPT-4 · Gemini · DeepSeek · GLM

---

### Projects

These are systems built around specific operational problems.

**[latam-intel-bot](https://github.com/GitGPT-jpg/latam-intel-bot)**  
Information pipeline for Latin America geopolitical monitoring. Multi-source ingestion (35 RSS feeds, 5 APIs), scheduled LLM report generation, WhatsApp Business delivery. The real engineering problem: normalizing inconsistent sources and keeping the pipeline running under partial failures.

**[android-llm-agent](https://github.com/GitGPT-jpg/android-llm-agent)**  
ADB-based agent for Android UI automation. OCR extracts screen state, LLM selects actions, a state machine manages multi-step execution. The core constraint: LLM outputs are non-deterministic; the surrounding system has to be.

**[voice-companion-agent](https://github.com/GitGPT-jpg/voice-companion-agent)**  
Conversational agent with persistent memory, dynamic persona, and TTS/RVC voice synthesis. The focus is long-horizon context management and interaction consistency across sessions — not just "it talks."

**[jianghu-nightrain](https://github.com/GitGPT-jpg/jianghu-nightrain)**  
Electron + Next.js productivity system with RPG-style goal tracking and AI-assisted planning. Local-first, Supabase sync.

---

### A few things I've come to believe

- The reliability of an AI system is mostly determined by the non-AI parts.
- Agents fail at edges, not the happy path. Design for that first.
- Orchestration logic is business logic. It shouldn't live inside a prompt.
- Observability on LLM outputs isn't optional once something is deployed.
- The gap between "works in demo" and "runs reliably" is most of the actual work.

---

### Current direction

- Agent runtime design: building execution environments that are testable and fault-tolerant
- Workflow patterns for operational AI: monitoring, triage, report generation, decision support
- The overlap between telecom OSS/BSS operational thinking and AI workflow architecture

---

[@GitGPT-jpg](https://github.com/GitGPT-jpg)

---

<a id="chinese"></a>

## 中文

我的工作聚焦于 AI 集成工作流系统 —— 具体来说，是模型调用返回之后发生的那些事情。

通信工程交付与技术支持出身。这个背景有实际影响：在考虑功能之前，我会先考虑运营连续性、故障处理和集成复杂度。

**实际在做的事**

- 编排层设计：将 LLM 与外部系统和确定性业务逻辑连接起来
- 带有状态控制、重试机制和可观测输出的 Agent 执行闭环
- 替代人工运营工作的自动化流水线 —— 不是演示，是已部署的系统
- 帮助工程团队用 AI 提升交付效率、而非替代工程判断的工具

**技术关注方向**

- 多步骤 Agent 系统中的工作流编排与执行控制
- 基于 LLM 的自动化可靠性模式：降级、重试、校验
- 高成本错误场景下的人机协同系统设计
- 长周期 Agentic 任务的状态管理
- 工具调用 Agent 的评测与可观测性

**技术栈**  
Python · FastAPI · Node.js · TypeScript · Next.js · Electron · SQLite · Docker

**日常使用的 LLM**  
Claude · GPT-4 · Gemini · DeepSeek · GLM

---

### 项目

这些系统围绕具体的运营问题而构建。

**[latam-intel-bot](https://github.com/GitGPT-jpg/latam-intel-bot)**  
面向拉丁美洲地缘政治监控的信息流水线。多源采集（35 个 RSS + 5 个 API），LLM 定时生成报告，WhatsApp Business 推送。工程难点在于跨不同来源的数据标准化，以及在部分节点故障时保持流水线稳定运行。

**[android-llm-agent](https://github.com/GitGPT-jpg/android-llm-agent)**  
基于 ADB 的 Android UI 自动化 Agent。OCR 提取屏幕状态，LLM 进行动作决策，状态机管理多步骤任务执行。核心约束：LLM 输出是非确定性的，外围系统必须是确定性的。

**[voice-companion-agent](https://github.com/GitGPT-jpg/voice-companion-agent)**  
具备持久记忆、动态人设和 TTS/RVC 语音合成的对话 Agent。重点是长程上下文管理和跨会话的交互一致性 —— 不只是"它会说话"。

**[jianghu-nightrain](https://github.com/GitGPT-jpg/jianghu-nightrain)**  
Electron + Next.js 效率系统，RPG 风格目标追踪 + AI 辅助规划。本地优先，支持 Supabase 同步。

---

### 一些实践中形成的判断

- AI 系统的可靠性，主要由非 AI 的部分决定。
- Agent 在边界条件下失败，而不是在 happy path 上。要优先针对这点设计。
- 编排逻辑就是业务逻辑。不应该让它住在 prompt 里。
- LLM 输出的可观测性，一旦上线就不是可选项。
- "演示可用"和"稳定运行"之间的差距，才是真正的大部分工作。

---

### 当前方向

- Agent 运行时设计：如何构建可测试、可容错的执行环境
- 面向运营场景的 AI 工作流模式：监控、分诊、报告生成、决策支持
- 通信行业 OSS/BSS 运营思维与 AI 工作流架构之间的交集

---

[@GitGPT-jpg](https://github.com/GitGPT-jpg)