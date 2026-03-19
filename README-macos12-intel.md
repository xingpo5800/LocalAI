# LocalAI for macOS 12.7.6 Intel

这是一个为macOS 12.7.6 Monterey系统编译的LocalAI版本。

## 系统要求
- macOS 12.7.6 Monterey
- Intel i5-4590t CPU (64位)
- 至少4GB内存

## 编译信息
- 基于LocalAI最新源码
- Go版本：1.21
- 架构：amd64 (Intel 64位)
- 禁用了macOS 15+特性

## 安装方法
```bash
# 下载可执行文件
curl -L -o localai https://github.com/xingpo5800/LocalAI/releases/download/v2.0.0-macos12-intel/localai

# 赋予执行权限
chmod +x localai

# 移动到系统路径
sudo cp localai /usr/local/bin/

# 测试安装
localai --help
```

## 使用方法
```bash
# 启动LocalAI服务
localai

# 后台运行
nohup localai > localai.log 2>&1 &

# 查看日志
tail -f localai.log
```

## 配置文件
配置文件位置：`~/.localai/config.yaml`

## 模型下载
```bash
# 下载模型
localai-llama download llama3:2b
localai-llama download qwen:2b
```

## 注意事项
- 此版本为适配版本，可能无法使用最新特性
- 建议在测试环境中验证功能
- 如有问题请查看GitHub Issues