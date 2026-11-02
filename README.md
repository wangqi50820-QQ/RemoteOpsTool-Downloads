# RemoteOpsTool 下载

Windows x64 远程运维工具。这里只发布程序包及说明，下载无需登录。

[下载 Fix1 修正版 ZIP](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/download/terminal-preview-20261102-fix1/RemoteOpsTool-Windows-x64-20261102-Fix1.zip)

[版本说明和校验文件](https://github.com/wangqi50820-QQ/RemoteOpsTool-Downloads/releases/tag/terminal-preview-20261102-fix1)

Fix1 补齐内嵌终端的本机 RunAs 凭据启动，针对旧功能可用而新终端提示 PSEXESVC Access is denied 的问题。请使用 Fix1 替换首个试用包。

完整解压到新目录后运行 RemoteOpsTool.exe，保留 Assets 文件夹。Windows 11 x64，需要 Edge WebView2 Runtime，无需 .NET SDK。每位使用者自行配置管理员凭据、PsExec 及 DameWare。

527 项本地自动测试通过；实际公司域环境仍待复测。