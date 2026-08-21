# Linux(Ext4)文件浏览器 — 下载与发布

在 Windows 中直接浏览、上传、下载 Linux(ext4) 磁盘文件的图形化工具。
基于系统自带的 WSL2 挂载机制，不装第三方驱动，不收集任何个人数据。

## 下载

见右侧 [Releases](../../releases) 页面，下载最新版安装包
`LinuxExt4FileBrowser-Setup-<版本>.exe`。

> 每个 Release 的说明中都附有安装包的 SHA256 校验值，下载后可核对：
> `powershell Get-FileHash <文件> -Algorithm SHA256`

## 系统要求

- Windows 10 版本 2004（内部版本 19041）及以上，或 Windows 11
- WSL2（应用会自动检测并引导安装）
- 挂载磁盘操作需要管理员权限（UAC）

## 相关文档

- [隐私政策](https://github.com/lighteninglin/ext4-file-browser-privacy/blob/main/PRIVACY.md)
- [安装程序退出码说明](installer-exit-codes.md)

## 版权

© 2026 林境工作室 (Linjing Studio). 保留所有权利。
本仓库仅用于发布安装包与公开文档，不含源代码。
