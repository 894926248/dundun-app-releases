# DunDun APP distributions

本仓库只发布 APP 安装包、更新清单和发行说明。整个项目源码由私有仓库 `894926248/dundun-api` 管理。

## 目录

```text
distributions/
  README.md                 # 分发包隔离与命名约定
  dundun/                   # DunDun 自有品牌分发
    README.md
```

代理专属分发加入 `distributions/<distribution-id>/`，与 `dundun` 平级。分发标识使用固定的小写英文、数字和短横线，不随品牌显示名称变化。只在有真实代理时创建其目录。

安装包及大文件上传至 GitHub Releases assets，不提交到 Git 文件历史。目录管理分发说明和后续实际接入的更新入口，不创建指向不存在版本的清单。

每个分发包独立发布、独立更新；不能使用仓库级 `/releases/latest` 为所有客户端选版本。自动更新尚未接入，本仓库初始化不表示客户端已具备更新能力。
