# RemoteOpsTool 下载

Windows 11 x64 远程运维工具。这里只发布程序包及说明，下载无需登录。

## 最新：Fix3

[下载 Fix3 ZIP](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/download/terminal-preview-20261102-fix3/RemoteOpsTool-Windows-x64-20261102-Fix3.zip)

[Fix3 版本说明](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/tag/terminal-preview-20261102-fix3) · [SHA-256 校验文件](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/download/terminal-preview-20261102-fix3/SHA256SUMS.txt)

SHA-256：

```text
1276DF205DC5D291858691D508481B9F82F5569F3AAF60A74C245E58D2A2AF13
```

Fix2 在实际域环境中已启动本机工作进程，但在跨账号命名管道连接阶段 15 秒超时。Fix3 移除该命名管道，改用父子进程继承的标准输入/输出传递启动信息和终端数据。所选域管理员账号仍用于启动工作进程，PsExec 仍收到显式远端凭据。程序继续使用 C:\ProgramData 临时目录，不修改桌面目录权限，不复制凭据、设置或日志。原有弹窗 CMD/PowerShell、DameWare 和命令日志继续保留。

完整解压到新目录后运行 RemoteOpsTool.exe，保留 Assets 文件夹。需要 Edge WebView2 Runtime；无需安装 .NET SDK。每位使用者自行配置管理员凭据、PsExec 及 DameWare。

验证：529 项本地自动测试通过，Release 发布构建及真实工作进程继承标准流往返通过。实际公司域环境仍待复测，本地测试不能替代域内验收。

## 历史版本

首个试用版、Fix1 和 Fix2 均已被 Fix3 替代，仅供排查历史问题。