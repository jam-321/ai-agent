# ai-agent（AI Agent 主线工程）

> 主线目标：开发一个真正可用的 AI Agent，并发布到互联网（产品化/上线）。

## 项目结构

| 目录 | 说明 |
| --- | --- |
| `backend/` | Spring Boot 3.5 + Spring AI 1.1 后端服务 |
| `frontend/` | Vue 3 + Vite 前端（网页聊天） |
| `docker/` | Docker Compose 中间件编排（MySQL / Redis） |
| `docs/design.md` | 完整方案设计 |

## 快速开始

### 前端

```bash
cd frontend
npm install
npm run dev   # development，http://127.0.0.1:5173
npm run test  # test，http://127.0.0.1:5174
npm run prod  # 构建 production 并本地预览，http://127.0.0.1:4173
```

> 注意：本机 PATH 中仍有 Node 16 时，`npm run ...` 可能调用旧 Node。需把
> `E:\soft\nodejs\node-v22.23.2-win-x64` 调整到系统 PATH 的旧 Node 目录之前。

### 后端

```bash
cd backend
mvn spring-boot:run
```

更多设计见 `docs/design.md`。
