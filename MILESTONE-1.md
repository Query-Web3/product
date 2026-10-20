# 里程碑 1 验收清单

- 里程碑：M1 —— DeFi 索引与数据后端
- 验收人：Roger Le，Product Manager
- 判定对象：**证据链接**，不是产物质量。全表只有一条判定规则：
  交付文档为该项交付物给出了**可公开访问的证据链接** → 通过；没给 → 部分。
  同一类证据（仓址 / 帖址）在同一列里必须得到同一个结论，不按交付物分别加尺子。

| 交付物编号 | 证据（仓内链接） | 核验结论 |
| :---- | :---- | :---- |
| 0a 许可证 | [database 仓](https://github.com/Query-Web3/database) | 通过：仓址，可公开访问 |
| 0b 文档 | [database 仓](https://github.com/Query-Web3/database) | 通过：仓址，可公开访问 |
| 0c 测试与测试指南 | [database 仓](https://github.com/Query-Web3/database) | 通过：仓址，可公开访问 |
| 0d Docker | [database 仓](https://github.com/Query-Web3/database) | 通过：仓址，可公开访问 |
| 0e 文章 | [Polkadot 论坛帖](https://forum.polkadot.network/t/the-value-discovery-engine-of-polkadot-queryweb3/16400) | 通过：帖址，可公开访问 |
| 1 DeFi 索引器 | [database 仓](https://github.com/Query-Web3/database) | 通过：仓址，可公开访问 |
| 2 事实表与维度表 | [database 仓](https://github.com/Query-Web3/database) | 通过：仓址，可公开访问 |
| 3 数据后端 | [backend 仓](https://github.com/Query-Web3/backend) | 通过：仓址，可公开访问 |

证据列链接**逐字抄自** W3F 里程碑交付文档
`Grant-Milestone-Delivery/deliveries/queryWeb3-milestone-1.md` 的「Link」列（该列原样指向
database / backend 仓与 Polkadot 论坛帖），未凭空构造 URL。

## 验收方式与边界

1. **只核证据，不核实现**：本表回答「有没有证据链接、能不能公开打开」，不回答「许可证是什么」
   「文档写得好不好」「镜像能不能构建」「测试覆盖多少」—— 后者要进仓逐项执行，不在本文件可核范围。
2. **口径统一**：证据是仓址就按仓址判，是帖址就按帖址判，不因交付物不同而换尺子；若要更细的
   结论，正确做法是把证据换成指向具体文件的链接，而不是在本表里补主观判断。
3. **不在本表验证的事**：性能压测、线上 SLA、数据时效（T+1 等 §6 目标）、后续里程碑范围。
