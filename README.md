# Agent Safety · Interactive Demos

两个采用统一浅色风格的中文 AI Agent 安全演示。

| 演示 | 入口 | 内容 |
| --- | --- | --- |
| AgentAuditor | [agentauditor/index.html](agentauditor/index.html) | 任务逐步执行，风险路径与审计发现同步呈现 |
| MobileProbe | [mobileprobe/index.html](mobileprobe/index.html) | 四个移动智能体安全案例的手机截图回放 |

首页 `index.html` 提供两个演示的切换入口。

## 本地使用

下载整个仓库，双击相应 `index.html` 打开。无需安装依赖或配置 API Key。

MobileProbe 需要保留整个 `mobileprobe/` 目录，尤其是 `assets/`。

## 在线访问

GitHub Pages 入口：https://hongkun16.github.io/agentauditor-demo/

AgentAuditor 的另一个公开演示地址：https://agentauditor-live-demo.riceagingintelligenc.chatgpt.site

## 交互

- **AgentAuditor**：选择任务、发送、暂停/继续、倍速与重播；点击风险发现定位操作。
- **MobileProbe**：切换四个案例、逐步播放、拖动进度、调速、放大画面、演示视图。

## 证据边界

AgentAuditor 为预设案例驱动的展示页面，不调用真实模型或外部工具，不代表实时审计或模型评测结果。

MobileProbe 为手动采集的手机截图回放；点击标记为独立说明图层，部分坐标为推断。购物案例只到结算页，未提交订单或付款；两个假弹窗案例仅证明点击并关闭弹窗，不推断后续操作。详见 [素材与证据说明](mobileprobe/SOURCES.md)。

## 研究参考

- AgentAuditor: Human-Level Safety and Security Evaluation for LLM Agents
- [论文](https://arxiv.org/abs/2506.00641)
- [原研究项目](https://github.com/Astarojth/AgentAuditor-ASSEBench)

本仓库为交互演示，不是研究项目的完整实现。
