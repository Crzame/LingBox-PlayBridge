# LingBox 插件命名规范

用户于 2026-10-28 确定以下约定。

## 主程序

- 中文名称：灵匣。
- 英文名称：LingBox。
- 主程序名称不带插件前缀。

宿主当前源码来自 ZTools。程序标题、图标、安装器、应用标识、更新通道和旧数据迁移需要单独实施，不能仅凭仓库名称变更就认为已经完成品牌迁移。保留原项目版权及许可证信息。

## 新插件

以后创建的插件展示名、GitHub 仓库名和发布包名统一以 `LingBox-` 开头。

| 用途 | 游桥示例 |
| --- | --- |
| 展示名 | LingBox-PlayBridge |
| 中文副标题 | 游桥 · 双端远程游戏助手 |
| GitHub 仓库 | Crzame/LingBox-PlayBridge |
| 发布包 | LingBox-PlayBridge-vX.Y.Z-win-x64.zip |
| 内部 ID | `crzame.playbridge` |

内部插件 ID 使用宿主要求的两段小写 `publisher.name` 格式，与展示名分开。插件更名时保持内部 ID 稳定，避免丢失配置、授权或升级关系；已有插件的内部 ID 不批量改写。

第三方开发者也可以按此约定创建插件，例如：

- `LingBox-Clipboard`，内部 ID 为 `alice.clipboard`。
- `LingBox-Translate`，内部 ID 为 `bob.translate`。
- `LingBox-ImageTools`，内部 ID 为 `carol.image-tools`。

`LingBox-` 前缀表示生态命名约定，不代表官方审核或实际兼容性保证。宿主仍应校验清单、API 版本、平台、包摘要、权限和发布者来源。
