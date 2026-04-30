# 🧠 HUMAN OS — 个人数字操作系统（Personal Operating System）

> 一个基于多 Agent 协作的 AI 系统，将“自我成长”转化为可执行、可反馈、可进化的闭环系统。

---

## 🚀 项目简介

HUMAN OS 是一个面向个人的智能操作系统，通过构建 **多 Agent 协作架构**，实现：

- 🎯 目标拆解（Goal → Plan）
- ⚡ 行动执行（Plan → Action）
- 🔁 复盘优化（Action → Reflection）
- 🧠 长期记忆（Memory）

帮助用户从“想做”走向“做到”，并持续进化。

---

## 🧩 核心架构

系统由 3 个核心 Agent 组成：

| Agent | 职责 |
|------|------|
| Planner | 将目标拆解为可执行步骤 |
| Executor | 提供具体行动建议 |
| Reviewer | 复盘行为并优化策略 |

同时配备：

- 🧠 Memory System（长期记忆存储）
- 🤖 LLM Engine（大模型推理核心）

---

## 🏗️ 技术架构
Frontend（待扩展）
↓
FastAPI Backend
↓
Agent Layer（Planner / Executor / Reviewer）
↓
LLM（OpenAI API）
↓
Memory（JSON / 可扩展向量数据库）

---

## 📁 项目结构
human_os/
│
├── main.py # API入口
├── agents/ # 多Agent模块
│ ├── planner.py
│ ├── executor.py
│ └── reviewer.py
│
├── core/
│ └── llm.py # LLM调用封装
│
├── memory/
│ └── store.py # 记忆系统
│
├── data/
│ └── memory.json # 本地数据存储
│
└── requirements.txt

---

## ⚙️ 快速开始

### 1️⃣ 安装依赖

```bash
pip install -r requirements.txt

---

## ⚙️ 快速开始

### 1️⃣ 安装依赖

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=your_api_key
3️⃣ 启动服务
uvicorn main:app --reload
