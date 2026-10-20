# 里程碑 1 验收清单

- 里程碑：M1 —— DeFi 索引与数据后端
- 验收人：Roger Le，Product Manager
- 结论口径：**通过** = 交付物可查、口径与申请一致；**部分** = 主体可用但有不满足项；
  **不适用** = 该交付物在 M1 的必选项之外或无法在本仓验证。

| 交付物编号 | 证据（仓内链接） | 核验结论 |
| :---- | :---- | :---- |
| 0a 许可证 | [database 仓 LICENSE](https://github.com/Query-Web3/database) | 通过：Apache 2.0 全文在仓内，与申请一致 |
| 0b 文档 | [database 仓 README](https://github.com/Query-Web3/database) | 通过：含表结构说明与本地起服务的步骤，能按文档跑通 |
| 0c 测试与测试指南 | [database 仓 README](https://github.com/Query-Web3/database) | 部分：核心 ETL 有测试，跨链协议规则变更时的回归覆盖不足 |
| 0d Docker | [database 仓 Dockerfile](https://github.com/Query-Web3/database) | 通过：镜像可构建，含数据库初始化 |
| 0e 文章 | [Polkadot 论坛帖](https://forum.polkadot.network/t/the-value-discovery-engine-of-polkadot-queryweb3/16400) | 通过：交付时已发布，内容与 M1 范围一致 |
| 1 DeFi 索引器 | [database 仓](https://github.com/Query-Web3/database) | 通过：Bifrost、Acala、Hydration、Moonbeam 四个协议已接入，规则按协议可配置 |
| 2 事实表与维度表 | [database 仓表结构说明](https://github.com/Query-Web3/database) | 通过：事实表按协议与时间粒度切分，维度表覆盖资产、链、协议三维 |
| 3 数据后端 | [backend 仓](https://github.com/Query-Web3/backend) | 部分：GraphQL 与 REST 查询可用，限流与缓存尚未纳入 M1 范围 |

证据列链接**逐字抄自** W3F 里程碑交付文档
`Grant-Milestone-Delivery/deliveries/queryWeb3-milestone-1.md` 的「Link」列（该列原样指向
database / backend 仓与 Polkadot 论坛帖），未凭空构造 URL。

## 验收方式与边界

1. **只看可复现的证据**：每条结论对应仓内文件或公开链接，不接受口头进度。
2. **「部分」不等于失败**：原因写清、是否影响后续里程碑单独判断；不影响 M2 的部分转入后续迭代。
3. **不在本表验证的事**：性能压测、线上 SLA、未来新增链的接入 —— 这些不属于 M1 的验收范围。
