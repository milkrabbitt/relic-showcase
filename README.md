# Relic · AI 角色产品工程记录
Relic 基于用户授权的人物资料与素材生成 AI 角色。核心产品闭源，这个独立作品集展示产品决策、架构、工程案例和有范围的验证结果。

**2026-11-01：内部TestFlight 1.0.0 / build21 已在iPhone实际安装并跑通同一隔离角色的系统文件导入、确认、真实蒸馏、聊天、记忆与冷启动回读。** 共享读取和人工记忆反向保存也有手机证据。源码22修复前台记忆显示，尚未打包安装；首版整体与审核条件仍未全部满足。

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


## 2026-11-01 实际手机验证

内部TestFlight 1.0.0(21)已在iPhone实际领取、安装并打开，保留原账号与关联。同一个隔离合成角色完成：系统Files选择下载TXT→7条UTF-8解析→双方与人物资料确认→真实MiniMax画像→手机发送聊天→3个回复气泡→记忆按钮修改及清空→冷启动后回读。实际额度从200到199，多气泡按一个逻辑回复结算；记忆操作未扣次数。这是一个代表性成功路径，尚未覆盖所有用户、格式或异常组合。

同机微信小程序实际开发版读取了相同资料、人格、聊天、额度、未读与清空结果。小程序正常手机按钮保存人工记忆后，iOS重新进入记忆页读到相同内容；没有重新绑定或用模拟身份代替。

还发现iOS已打开记忆页返回前台时编辑区保留旧值：服务器已保存，重新进入正确。源码build22已补安全刷新、保留未保存草稿、版本冲突提示和显式读取最新版本；状态测试执行及完整源代码设备SDK类型检查通过。Xcode构建输出写入受限，22尚未打包、安装或上传，不能借21结果宣称22真机通过。

普通自动记忆消费缺口及清空竞态的兼容候选已完成本地验证，云端最终升级仍未确认，不宣称所有用户已生效。普通独立真实账号、双端冲突/删除缓存、电脑摄像头扫码、微信机器人实际收发、主动调度、最终全页截图及审核材料仍未通过。未提交审核或正式发布。

[合成TXT素材预发布](https://github.com/milkrabbitt/relic-showcase/releases/tag/import-sample-20261030)仅提供完全虚构测试资料，不是App发布。现有公开截图仍属于各自标注的旧构建；新手机截图曾实际查看，但尚无已保存并审核可公开的最终图片。
