# 安装程序错误代码说明 / Installer Exit Codes

Linux(Ext4)文件浏览器的安装程序由 Inno Setup 6 打包生成，未定义自定义错误代码，
直接沿用 Inno Setup 标准退出码：

| 退出码 | 含义 | 对应场景 |
|---|---|---|
| 0 | 安装成功 | installationSuccessful |
| 1 | 初始化失败（如 /VERYSILENT 但前置条件不满足） | miscellaneous |
| 2 | 用户在安装开始前点击"取消" | installationCancelledByUser |
| 4 | 磁盘空间不足或目录不可写 | diskSpaceIsFull |
| 5 | 用户在安装过程中点击"取消" | installationCancelledByUser |
| 8 | 需要重启系统才能完成安装 | rebootRequired |

在 `/VERYSILENT /NORESTART` 静默模式下，安装程序不会弹窗；
失败时以上退出码会作为进程退出码返回。

## 常见问题

- **杀毒软件拦截**：安装包未购买代码签名证书，部分杀软可能误报。如遇拦截，
  请核对安装包的 SHA256 与发布页面公布值一致后添加信任。
- **权限不足**：安装目录为 `%ProgramFiles%\LinuxFileBrowser`，需要管理员权限；
  安装器会自动请求 UAC 提权。

支持渠道：见商店列表中的"支持联系方式"。
