# 里程碑 1 验收清单

- 里程碑：M1 —— DeFi 索引与数据后端
- 验收人：Roger Le，Product Manager
- 判定对象：**证据链接存在性与实现是否核验**。全表只有一条判定规则：
  交付文档给出了可公开访问的证据链接，但本文件**没有逐项执行验核** → 部分（实现未核验）。
  没有链接 → 不通过。不因交付物不同换尺子；只有真的跑过验证才能升级为「通过」。

| 交付物编号 | 证据（仓内链接） | 核验结论 |
| :---- | :---- | :---- |
| 0a 许可证 | [database 仓](https://github.com/Query-Web3/database) | 部分：仓址可公开访问，实现未核验 |
| 0b 文档 | [database 仓](https://github.com/Query-Web3/database) | 部分：仓址可公开访问，实现未核验 |
| 0c 测试与测试指南 | [database 仓](https://github.com/Query-Web3/database) | 部分：仓址可公开访问，实现未核验 |
| 0d Docker | [database 仓](https://github.com/Query-Web3/database) | 部分：仓址可公开访问，实现未核验 |
| 0e 文章 | [Polkadot 论坛帖](https://forum.polkadot.network/t/the-value-discovery-engine-of-polkadot-queryweb3/16400) | 部分：帖址可公开访问，实现未核验 |
| 1 DeFi 索引器 | [database 仓](https://github.com/Query-Web3/database) | 部分：仓址可公开访问，实现未核验 |
| 2 事实表与维度表 | [database 仓](https://github.com/Query-Web3/database) | 部分：仓址可公开访问，实现未核验 |
| 3 数据后端 | [backend 仓](https://github.com/Query-Web3/backend) | 部分：仓址可公开访问，实现未核验 |

证据列链接**逐字抄自** W3F 里程碑交付文档
`Grant-Milestone-Delivery/deliveries/queryWeb3-milestone-1.md` 的「Link」列（该列原样指向
database / backend 仓与 Polkadot 论坛帖），未凭空构造 URL。

## 验收方式与边界

1. **证据可访问 ≠ 已验收**：本表只确认证据链接可公开打开；「许可证是什么」「镜像能不能构建」
   「测试覆盖多少」都没在本文件里跑过，故全部判**部分**。升级为「通过」的唯一方式是逐项执行验证
   并把输出附在本文件里。
2. **口径统一**：证据是仓址就按仓址判，是帖址就按帖址判，不因交付物不同而换尺子；若要更细的
   结论，正确做法是把证据换成指向具体文件的链接，而不是在本表里补主观判断。
3. **不在本表验证的事**：性能压测、线上 SLA、数据时效（见 PRD §6 的实现要求）、后续里程碑范围。
