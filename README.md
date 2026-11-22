# BPAI 企业级 AI 平台

BPAI 面向企业的算法、应用和运维团队。团队可以在同一套 GPU 基础设施上开发、训练和部署模型，开展强化学习（RL）和模型后训练，并开发、评估和运行 AI Agent。项目统一管理权限、资产、调度、可观测性和内部成本。仓库当前处于产品与架构设计阶段。

| 阅读入口 | 适合了解的问题 |
| --- | --- |
| [设计路线图](design-roadmap.md) | 要设计哪些内容，按什么顺序推进，每一步怎样完成？ |
| [产品设计](product-design.md) | 团队如何提交训练和 RL 作业、评估模型，以及开发和运行 Agent？ |
| [系统架构](system-architecture.md) | 控制面、计算集群、RL 作业、Agent 运行时和计量如何协作？ |
| [模块实现设计](module-design.md) | 如何执行训练、归档 RL 实验、运行 Agent 并对账？ |

## Design Before Development

BPAI 当前以设计为主。先按真实任务核对产品流程，再确定接口、状态、权限和恢复规则。

- 产品设计交代使用者、目标、操作、结果和异常处理，并给出可核对的验收场景。
- 系统架构说明组件职责、跨模块接口、版本与权限，以及遇到故障时怎样恢复和核对成本。
- 模块实现设计把同一验收场景拆成输入、执行、产物、状态变化和核对方法。

从需求到验收能够逐项对应后，再开始功能开发。当前从[设计路线图的第 1 步](design-roadmap.md#第一步怎么走查)开始。

## Language

Documentation and direct conversations with the user may use Chinese. Use English for everything else, including file and directory names, code and comments, configuration, API fields, UI and CLI text, logs, and error messages. Use English for branch names, commit messages, issues, and pull requests.
