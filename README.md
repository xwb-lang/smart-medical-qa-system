# 智能医疗问答系统
> 基于 Spring Boot + Ollama 本地大模型开发的医疗领域智能问答系统，实现流式对话、多轮上下文管理、安全可控的医疗问答输出。

---

## ✨ 项目亮点
1. **本地大模型集成（DeepSeek + Ollama + Spring AI）**
基于 Ollama 本地部署 DeepSeek 大模型，通过 Spring AI 实现无缝接入，不依赖第三方 API，既保证了数据隐私，也实现了低延迟的医疗问答响应。

2. **SSE 流式响应（逐字输出效果）**
   采用 Server-Sent Events 实现回答实时推送到前端，无等待、体验流畅。

3. **医疗专属 Prompt 工程**
   构建专业医疗角色提示词，让回答更安全、更专业、更贴合医疗场景。

4. **多轮对话上下文管理**
   自动保存聊天记录，支持上下文理解，实现连贯的多轮智能问答。

5. **完整前后端交互架构**
   标准 MVC 架构，代码规范、结构清晰，可直接作为企业级 AI 项目模板。

---

## 🛠️ 技术栈
- 后端：Spring Boot、Spring AI、Ollama
- 通信：SSE（流式响应）
- 数据库：MySQL、MyBatis
- 工具：Lombok、Hutool
- 大模型：本地部署开源大模型

---

## 📐 系统架构图
```mermaid
graph TD
    A[前端页面] --> B[Spring Boot 后端]
    B --> C[Ollama 本地大模型]
    B --> D[MySQL 聊天记录存储]

## 项目演示
### 1. 流式对话主界面
![对话主界面](docs/screenshots/chat-ui.png)

### 2. SSE流式响应核心代码
![SSE实现代码](docs/screenshots/sse-code.png)

### 3. 医疗场景Prompt配置
![Prompt工程代码](docs/screenshots/prompt-code.png)
