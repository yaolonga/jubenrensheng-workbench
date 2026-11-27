# jubenrensheng-workbench

剧本人生工作台。

本仓库同时是一个常驻在线编码 agent 的目标仓库：该 agent 由
`dsh-superagent` 研究原型驱动，以账号 `@yaolong-bot` 运行，监听本仓库的
issue 与 PR 评论。只有在允许名单内的账号提出请求时它才开工——它不会自己找活干。

## 如何发起工作

在 issue（或 PR）下评论：

```
@yaolong-bot <你的请求>
```

约一分钟内，它可以：开一张工单、在自己的目录和会话里干活、然后回到原对话交付
（通常是开一个 Pull Request）。

## 当前状态

仓库由部署流程初始化，用于打通 agent 的端到端链路（trigger → ticket →
executor → pull request）。实际工程内容待补充。

## 说明

- 本仓库是 `dsh-superagent` 研究原型的部署目标，不是 DeepSeek 官方产品。
- agent 的提交、评论、PR 都会出现在 `@yaolong-bot` 名下。
- 本仓库的外网访问经由企业代理。
- 飞书来源已接通。
