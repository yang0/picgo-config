# PicGo 图床配置仓库

一个用于管理 PicGo 图床配置的仓库，方便快速配置和备份图床设置。

## 📦 什么是 PicGo

PicGo 是一个用于快速上传图片并获取图片 URL 链接的工具，支持多种图床服务：

- GitHub
- SM.MS
- 七牛云
- 腾讯云 COS
- 阿里云 OSS
- Imgur
- Cloudflare R2
- 又拍云
- 等 60+ 图床服务

## 🚀 快速开始

### 安装 PicGo

**Windows**:
```bash
# 使用 Scoop
scoop install picgo

# 或者从官网下载
# https://github.com/Molunerfinn/PicGo/releases
```

**macOS**:
```bash
# 使用 Homebrew
brew install --cask picgo
```

**Linux**:
```bash
# 从官网下载 AppImage
# https://github.com/Molunerfinn/PicGo/releases
```

### 配置说明

1. 复制 `config.example.json` 为 `config.json`
2. 根据你的图床服务修改配置文件
3. 在 PicGo 应用中导入配置或手动配置

### 常用图床配置示例

#### GitHub 图床
```json
{
  "picBed": {
    "current": "github",
    "github": {
      "repo": "username/repo-name",
      "token": "your-github-token",
      "path": "images/",
      "branch": "main",
      "customUrl": "https://cdn.jsdelivr.net/gh/username/repo-name@main"
    }
  }
}
```

#### SM.MS 图床
```json
{
  "picBed": {
    "current": "smms",
    "smms": {
      "token": "your-smms-token"
    }
  }
}
```

#### 七牛云
```json
{
  "picBed": {
    "current": "qiniu",
    "qiniu": {
      "accessKey": "your-access-key",
      "secretKey": "your-secret-key",
      "bucket": "your-bucket-name",
      "url": "https://your-domain.com",
      "area": "z0",
      "path": "images/"
    }
  }
}
```

## ✨ 功能特性

- 🖼️ 支持 60+ 图床服务
- ⌨️ 全局快捷键上传 `Ctrl+Shift+P`
- 📋 剪贴板图片自动上传
- 🎯 拖拽上传
- 🔗 上传后自动复制链接（Markdown/HTML/URL 格式）
- 🔌 插件系统支持扩展功能
- 📝 支持 Typora、Obsidian、VS Code 等编辑器集成

## 🔧 常用快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl+Shift+P` | 快捷上传剪贴板图片 |
| `Ctrl+Shift+O` | 打开 PicGo 主窗口 |
| `Ctrl+Shift+D` | 打开上传历史 |

## 📚 相关链接

- **官方网站**: https://picgo.app/
- **文档**: https://docs.picgo.app/
- **GitHub 仓库**: https://github.com/Molunerfinn/PicGo
- **插件市场**: https://github.com/PicGo/Awesome-PicGo
- **PicGo-Core (命令行版本)**: https://github.com/PicGo/PicGo-Core

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

MIT License
