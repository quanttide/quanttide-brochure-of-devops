# 量潮DevOps云命令行工具开始内测

量潮DevOps云命令行工具，现开启内部测试。

## 概述

纯 Rust 实现的 CLI 工具，提供发布管理和代码管理能力。当前代码管理功能以 Git 子模块为主。

## 功能

### 代码管理

```bash
# 查看子模块状态
qtcloud-devops code status

# 同步子模块
qtcloud-devops code sync my-module

# 退役子模块
qtcloud-devops code retire old-module
```

当前以 Git 子模块管理为主。

### 发布管理

```bash
# 预发布版本
qtcloud-devops release stage -v cli/v0.4.1-rc.1

# 正式发布
qtcloud-devops release publish -v cli/v0.4.1 -y

# 退役版本
qtcloud-devops release retire -v v0.3.0

# 查看发布状态
qtcloud-devops release status
```

## 安装

```bash
pip install qtcloud-devops-cli
```

或通过 cargo 安装：

```bash
cargo install qtcloud-devops-cli
```

## 文档

完整文档：https://quanttide.github.io/qtcloud-devops/

## 问题反馈

内测期间如遇到问题，请在仓库提交 Issue：

https://github.com/quanttide/qtcloud-devops/issues
