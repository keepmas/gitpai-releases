# GitPai Windows 下载与更新

此公开仓库仅用于分发 GitPai Windows x64 安装包、便携包和签名更新清单，不包含私有应用源码。

从 [Releases](https://github.com/keepmas/gitpai-releases/releases) 下载。安装包自包含，无需另装 .NET。

首次从 1.1.7 或更早版本升级时，请先正常停止加速并退出旧程序，再手动安装。安装器默认安装到当前用户目录，配置和日志独立保存，卸载保留用户数据。

1.1.8 起支持固定公开源、内置 P-256 公钥验证、下载校验、用户确认安装，以及普通/限期/紧急更新策略。程序不会强杀进程或未经确认静默安装。

**注意**：发布包由 Linux 交叉构建，Windows 实机 GUI、安装升级、代理/Hosts 恢复、UAC 和安全软件兼容性尚未完成验收。签名更新清单不是 Windows Authenticode，不代表通过 SmartScreen 信誉认证。请阅读每个 Release 的说明，并在目标设备验证。

公开更新公钥的 SPKI DER SHA-256 指纹：
`773d427c409c3ba581161eee09accb93b5a9bbae0ebbe4f83459676b8808be9b`

稳定更新入口使用 `updater` Release 下的 `stable-win-x64-v2.json`。此入口发布签名元数据，不是安装版本；请从具体版本 Release 下载安装器。公开仓库不保存签名私钥、用户配置、日志或 CA 私钥。
