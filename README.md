# Relic · AI 角色产品工程记录
Relic 基于用户授权的人物资料与素材生成 AI 角色。核心产品闭源，这个独立作品集展示产品决策、架构、工程案例和有范围的验证结果。

**2026-10-30：1.0.0 / build21 已实际安装 iPhone，签名归档并上传完成。内部 TestFlight 已向现有账户持有人发出邀请，尚未核实领取安装，未提交审核或正式发布。** 既有已付主机的独立持久 HTTPS 服务已运行，App 本人登录后角色读取、新共享角色创建、7条素材草稿上传及真实微信受保护读取通过；完整手机蒸馏聊天记忆闭环仍待验。

用户流程：导入 TXT / CSV / JSON 或授权电脑上传 → 预览与说话人确认 → 人物资料确认 → MiniMax 生成画像 → 聊天与记忆。这里的“蒸馏”是画像和上下文提取，不是训练模型权重。AI 角色不是真实自然人本人。

## 实际运行界面
下图为实际 iOS Simulator 运行的 Debug 合成资料原图，**不是私人聊天、真实业务验收或商店截图**。首页、详情、素材为 build19；另有 build20 导入核对、人格、记忆和长消息键盘实图。最终 build21 的全页复验尚未齐，不混用构建结论。

| 首页19 | 角色详情19 | 素材19 |
|---|---|---|
| ![合成首页](assets/ui/after-home.png) | ![合成角色详情](assets/ui/after-detail.png) | ![合成素材](assets/ui/materials-build19.png) |

[真实改前详情18](assets/ui/before-detail-build18.png) → [修复后详情19](assets/ui/after-detail.png)：运行发现预览提示压住导航标题，调整后重新运行并核对。另有[资料输入键盘19](assets/ui/profile-keyboard-build19.png)与[较早聊天17](assets/ui/after-chat.png)，不混作最终版本验收。

[导入核对20](assets/ui/import-review-build20.png) · [人格20](assets/ui/persona-build20.png) · [记忆20](assets/ui/memory-build20.png) · [长消息与键盘20](assets/ui/chat-long-keyboard-build20.png)

- [产品流程](docs/product.md) · [架构与数据归属](docs/architecture.md)
- [工程案例](docs/engineering-case-studies.md) · [验证结果](docs/validation.md)
- [当前进度](docs/progress.md) · [路线与限制](docs/roadmap.md)
- [开发者贡献](docs/ownership-and-attribution.md) · [简历摘要](docs/resume.md)

开发者主导需求、交互、身份与数据边界、整合和验收；使用 AI 编程助手辅助实施代码、测试、界面及文档。未提供访客业务演示服务，不公开核心源码、私有历史、用户素材或安装包，没有虚构用户量、收入或效果指标。

Relic is a closed-source AI character product in active development. These are scoped engineering results and synthetic UI captures, not a production availability claim.
