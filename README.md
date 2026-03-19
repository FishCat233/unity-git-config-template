<div align="center">

<h1>Unity Git Config Template</h1>

![GitHub Release](https://img.shields.io/github/v/release/FishCat233/unity-git-config-template) ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/FishCat233/unity-git-config-template/total)
[![wakatime](https://wakatime.com/badge/github/FishCat233/unity-git-config-template.svg)](https://wakatime.com/badge/github/FishCat233/unity-git-config-template)

<h5>专为 Unity 项目优化的 Git 配置文件模板</h5>

![访问次数](https://count.getloli.com/get/@fishcat233-unity-git-template?theme=rule34)

</div>

> [!WARNING]
> 
> 以下内容由 AI 编写，可能包含错误或不完整的信息。
>
> 具体情况请以源码为准。

## 📖 项目介绍

Unity Git Config Template 是一个专为 Unity 项目优化的 Git 配置文件模板，包含精心配置的 `.gitignore` 和 `.gitattributes` 文件，帮助开发者更好地管理 Unity 项目的版本控制。

## ✨ 特性

- **智能的 `.gitignore`**: 自动忽略 Unity 生成的临时文件、构建文件、日志文件等
- **优化的 `.gitattributes`**: 正确处理文本文件和二进制文件，支持 Git LFS
- **跨平台兼容**: 处理不同操作系统的换行符差异
- **性能优化**: 减少不必要的文件提交，提升 Git 操作效率
- **团队协作友好**: 统一的配置标准，避免团队成员间的配置冲突

## 🚀 快速开始

### 安装方法

#### 方法一：直接下载（推荐）

1. 下载本仓库的 `.gitignore` 和 `.gitattributes` 文件
2. 将文件放置到你的 Unity 项目根目录
3. 如果项目已存在同名文件，请先备份再替换

#### 方法二：Git 克隆

```bash
git clone https://github.com/FishCat233/unity-git-config-template.git
cd unity-git-config-template
# 复制配置文件到你的 Unity 项目
cp .gitignore /path/to/your/unity/project/
cp .gitattributes /path/to/your/unity/project/
```

### 配置 Git LFS（可选但推荐）

如果你的项目包含大量二进制资源文件（如图片、音频、模型等），建议启用 Git LFS：

```bash
# 安装 Git LFS
git lfs install

# 跟踪二进制文件类型
git lfs track "*.png"
git lfs track "*.jpg"
git lfs track "*.fbx"
git lfs track "*.wav"
# ... 更多文件类型请参考 .gitattributes 文件
```

建议直接复制 `.gitattributes` 作为模板在此基础上按需求进行修改。

## 📁 文件说明

### .gitignore

此文件定义了 Unity 项目中应该被 Git 忽略的文件和目录，包括：

- Unity 生成的临时文件（Library/, Temp/, Obj/ 等）
- 构建输出文件（Build/, Builds/）
- 日志文件（Logs/, *.log）
- IDE 配置文件（.vs/, .consulo/）
- 个人设置文件（*.DotSettings.user）

### .gitattributes

此文件定义了 Git 如何处理不同类型的文件：

- **文本文件处理**: 确保 Unity 脚本和配置文件正确处理换行符
- **Git LFS 配置**: 自动将大型二进制文件通过 Git LFS 管理
- **文件类型识别**: 正确识别 Unity 特有的文件格式

## 💡 使用建议

### 最佳实践

1. **项目初始化时使用**: 在创建新的 Unity 项目时立即应用此配置
2. **团队项目统一**: 确保团队所有成员使用相同的 Git 配置
3. **定期更新**: 关注本仓库的更新，获取最新的 Unity 版本支持

### 常见问题

**Q: 我已经有现有的 Git 仓库，如何应用此配置？**
A: 直接替换现有的 `.gitignore` 和 `.gitattributes` 文件，然后提交更改。注意：已跟踪的文件需要手动移除。

**Q: Git LFS 是必须的吗？**
A: 不是必须的，但强烈推荐。Git LFS 可以显著减少仓库大小并提升性能。

**Q: 如何验证配置是否正确工作？**
A: 运行 `git status` 检查是否忽略了正确的文件，使用 `git lfs ls-files` 检查 LFS 跟踪的文件。

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个模板！

### 贡献指南

1. Fork 本仓库
2. 创建你的功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个 Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🙏 致谢

感谢所有为 Unity 社区贡献 Git 配置模板的开发者们！

---

⭐ 如果这个项目对你有帮助，请给个 Star！
