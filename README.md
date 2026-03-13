# Wheat Market (Genius Launch Pad) Registry

这是 Wheat Community (麦穗社区) 的核心 Agent 资产注册中心。

## 目录结构
- `/assets`: 存放标准化的 `.wheat.yaml` 配置文件，每一个文件对应一款独立分发的 AI Agent。

## 首发种子资产清单
1. **Wheat Deep Researcher** (`deep-researcher.wheat.yaml`): 深度调研 Agent，集成 `tavily-search` 和 `markdown-converter`。
2. **Wheat Web Navigator** (`wheat-web-navigator.wheat.yaml`): 网页自动化执行 Agent，集成 `agent-browser` 控制。
3. **Wheat DevOps Assistant** (`wheat-devops-assistant.wheat.yaml`): 开源项目维护 Agent，集成 `gh-issues` 和 `github` 操作。

## 未来接入计划
- **API 接口暴露**: 这个目录将连接至 `https://wheatcoin-community-production.up.railway.app/launch.html` 的前端展示。
- **命令行下发**: 构建 `npx wheat-market add <asset>` 的 CLI 工具拉取本仓库的配置到用户本地。
- **代币结算网关**: 读取 `pricing` 节点判断 `$WHC` 持仓门槛。