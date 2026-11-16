# DunDun APP releases

本仓库只用于 APP 安装包、更新清单和发行说明。整个 DunDun API 项目的源码保存在私有仓库 `894926248/dundun-api`。

- 自有品牌包：[distributions/dundun](distributions/dundun/README.md)
- 分发隔离规则：[distributions/README.md](distributions/README.md)

Windows x64 正式安装版支持自动检查及后台下载更新，准备好后由用户选择重启安装。客户端仅访问对应 distribution-id 的更新清单，不使用仓库级 latest Release，避免自有包和代理包串更。

安装包和校验文件放在 GitHub Releases assets，大文件不提交到 Git 历史。新代理在 distributions/ 下使用独立目录；只加入允许公开的信息，不上传源码、凭据或用户数据。
