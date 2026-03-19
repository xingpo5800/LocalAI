# 触发macOS 12.7.6 Intel编译

这个文件用于触发GitHub Actions编译macOS 12.7.6 Intel版本。

## 编译配置
- 系统：macOS 12.7.6 Monterey
- CPU：Intel i5-4590t (64位)
- Go版本：1.21
- 架构：amd64
- 禁用macOS 15+特性

## 编译步骤
1. Fork https://github.com/mudler/LocalAI
2. 添加workflow权限
3. 推送此文件触发编译
4. 等待编译完成
5. 下载编译版本

## 需要的权限
- GitHub Actions workflow权限
- Releases发布权限

## 编译完成后
- 下载地址：https://github.com/xingpo5800/LocalAI/releases
- 文件名：localai-macos12-intel
- 安装方法：sudo cp localai /usr/local/bin/