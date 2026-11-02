# RemoteOpsTool 下载

Windows 11 x64 远程运维工具。这里只发布程序包及说明，下载无需登录。

## 最新：Fix2

[下载 Fix2 ZIP](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/download/terminal-preview-20261102-fix2/RemoteOpsTool-Windows-x64-20261102-Fix2.zip)

[Fix2 版本说明](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/tag/terminal-preview-20261102-fix2) · [SHA-256 校验文件](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/download/terminal-preview-20261102-fix2/SHA256SUMS.txt)

SHA-256：

```text
FE1EE587334F879B33E996E55ED0DB7FB3A7A7C4DEE5DAB346BC7927F0B305AA
```

Fix1 在实际域账号下仍会从桌面目录以 RunAs 启动本机终端工作进程，日志显示远程连接前即出现 Access is denied。Fix2 会先把工作进程复制到 C:\ProgramData 下本次专用的临时目录，再使用所选凭据启动；不修改桌面目录权限，不复制凭据、设置或日志。原有弹窗 CMD/PowerShell、DameWare 和命令日志继续保留。

完整解压到新目录后运行 RemoteOpsTool.exe，保留 Assets 文件夹。需要 Edge WebView2 Runtime；无需安装 .NET SDK。每位使用者自行配置管理员凭据、PsExec 及 DameWare。

验证：529 项本地自动测试通过，Release 发布构建和包内资源完整性校验通过。实际公司域环境仍待复测，本地测试不能替代域内验收。

## 历史版本

首个试用版和 Fix1 均已被 Fix2 替代，仅供排查历史问题。