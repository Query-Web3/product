# 里程碑 1 验收清单

- 里程碑：M1 —— DeFi 索引与数据后端
- 验收人：Roger Le，Product Manager
- 判定对象：**证据**，不是产物质量。每行回答「这项交付物在交付文档里有没有可公开访问的证据、
  证据指向哪个仓或帖子」，而不回答「测试覆盖多少」「镜像能不能构建」—— 后者要逐仓跑，
  不在本文件的可核范围内，故一律不做断言。

| 交付物编号 | 证据（仓内链接） | 核验结论 |
| :---- | :---- | :---- |
| 0a 许可证 | [database 仓](https://github.com/Query-Web3/database) | 通过：证据指向 database 仓根，许可证位于仓根 |
| 0b 文档 | [database 仓](https://github.com/Query-Web3/database) | 通过：证据指向 database 仓根，文档位于仓根 |
| 0c 测试与测试指南 | [database 仓](https://github.com/Query-Web3/database) | 部分：证据只给到仓根地址，未单列测试指南条目，指南是否独立成文需进仓核对 |
| 0d Docker | [database 仓](https://github.com/Query-Web3/database) | 部分：证据只给到仓根地址，未单列 Dockerfile 条目，容器化交付物需进仓定位 |
| 0e 文章 | [Polkadot 论坛帖](https://forum.polkadot.network/t/the-value-discovery-engine-of-polkadot-queryweb3/16400) | 通过：证据是可公开访问的论坛帖地址，不依赖仓内文件 |
| 1 DeFi 索引器 | [database 仓](https://github.com/Query-Web3/database) | 通过：证据指向 database 仓，索引器为该仓的主交付物 |
| 2 事实表与维度表 | [database 仓](https://github.com/Query-Web3/database) | 通过：证据指向 database 仓，表结构归属该仓 |
| 3 数据后端 | [backend 仓](https://github.com/Query-Web3/backend) | 通过：证据指向独立的 backend 仓；限流与缓存在申请里属后续里程碑，不构成本行判定依据 |

证据列链接**逐字抄自** W3F 里程碑交付文档
`Grant-Milestone-Delivery/deliveries/queryWeb3-milestone-1.md` 的「Link」列（该列原样指向
database / backend 仓与 Polkadot 论坛帖），未凭空构造 URL。

## 验收方式与边界

1. **结论只落在证据上**：通过 = 证据可公开访问且指向的仓/帖与交付物匹配；部分 = 证据粒度粗于
   交付物（只到仓根），需进仓才能定位；不做出「功能可用 / 构建通过」这类本表无法验证的判断。
2. **「部分」不等于失败**：它说的是证据粒度，不是交付质量；补齐方式是把证据替换为仓内具体路径。
3. **不在本表验证的事**：性能压测、线上 SLA、测试覆盖率、容器构建结果、未来新增链的接入 ——
   这些不属于本文件的可核范围。
