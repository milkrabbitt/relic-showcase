# Relic · AI 角色产品工程记录

基于用户授权提供的人物资料和聊天素材构建 AI 角色。产品核心闭源，本仓库仅公开产品、架构、工程案例和脱敏验证摘要。

用户流程：手机导入 TXT / CSV / JSON 或电脑扫码授权上传 → 预览素材并确认说话人 → 确认人物资料 → 提取画像并试聊 → 在具备条件时独立连接微信机器人。所谓“蒸馏”使用 MiniMax 提取人物画像、语气和记忆上下文，不涉及模型权重训练。

**当前为开发与验收阶段，尚未正式发布。** iOS 与微信小程序已有真实后端；双方身份绑定已验证，新共享测试角色的资料可双向访问，既有聊天和额度在 iPhone 可读。手机小程序完整共享、记忆双向编辑和删除界面传播仍待验。当前机器人收发未启用，不能据历史记录宣称当下可用。

开发者主导需求范围、导入及确认流程、账号/数据归属设计、开发整合、调试验收与部署边界；使用 AI 编程助手实施部分代码、测试与文档。见[贡献与第三方说明](docs/ownership-and-attribution.md)。

- [产品与流程](docs/product.md) · [高层架构](docs/architecture.md)
- [工程案例](docs/engineering-case-studies.md)：重试结算、导入确认、身份与共享
- [真实进度](docs/progress.md) · [验证结果](docs/validation.md) · [后续路线](docs/roadmap.md)
- [简历项目描述](docs/resume.md)

本轮提供文字证据摘要，没有可供访客登录的公开演示服务，没有公开真实用户数据、源码或安装包。测试成功范围与限制分开记录，无用户量、收入或生产稳定性宣传。

Relic is a closed-source AI character product in active development. This repository documents product decisions, architecture, engineering trade-offs and scoped validation; it is not a source mirror or a production availability claim.
