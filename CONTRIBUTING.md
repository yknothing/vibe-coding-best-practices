# 贡献指南

感谢您考虑为 Vibe Coding 最佳实践项目做出贡献！本指南将帮助您了解如何参与项目，提交高质量的贡献，并与社区有效协作。

## 贡献类型

您可以通过多种方式为本项目做出贡献：

- **最佳实践分享**：分享您在 AI 辅助开发中的实践经验
- **规则模板**：提供 Cursor、Windsurf 等 AI IDE 的有效规则配置
- **文档改进**：完善现有文档，修复错误或添加示例
- **新 IDE 支持**：为其他 AI 编程助手添加实现指南
- **案例研究**：提供实际项目中应用 Vibe Coding 的案例

## 贡献流程

### 1. 选择或创建 Issue

- 浏览现有 [Issues](https://github.com/username/vibe-coding-best-practices/issues) 查找您可以帮助解决的问题
- 如果您想提出新的改进或修复，请先创建一个新 Issue 描述您的想法
- 等待维护者的反馈，确认您的贡献方向与项目目标一致

### 2. Fork 和克隆仓库

```bash
git clone https://github.com/YOUR-USERNAME/vibe-coding-best-practices.git
cd vibe-coding-best-practices
git remote add upstream https://github.com/original-owner/vibe-coding-best-practices.git
```

### 3. 创建分支

```bash
git checkout -b feature/your-feature-name
```

### 4. 开发和测试

- 按照项目结构和风格指南进行开发
- 确保您的贡献遵循本文档后续部分描述的规范
- 如适用，添加必要的测试或文档

### 5. 提交更改

```bash
git add .
git commit -m "feat: add new playbook for refactoring patterns"
```

请遵循以下提交信息格式：
- `feat: ` 新功能或内容
- `fix: ` 错误修复
- `docs: ` 文档更新
- `style: ` 格式调整
- `refactor: ` 重构
- `example: ` 添加示例

### 6. 同步上游更改

```bash
git fetch upstream
git rebase upstream/main
```

### 7. 推送更改

```bash
git push origin feature/your-feature-name
```

### 8. 创建 Pull Request

- 前往 GitHub 仓库页面，创建 Pull Request
- 提供清晰的描述，解释您的贡献解决了什么问题
- 关联相关 Issue
- 等待维护者审查

## 内容贡献指南

### Playbooks

添加或修改 Playbooks 时，请遵循以下结构：

```markdown
# [活动名称] 最佳实践

*简短描述*

## 概述

[详细介绍此 Playbook 的目的和价值]

## 核心原则

[列出相关的 Vibe Coding 原则]

## 实践步骤

### 1. [步骤名称]

**目标**：[步骤目标]

**最佳实践**：
- [实践点1]
- [实践点2]
...

**反模式**：
- [应避免的做法]
...

**示例**：
```[示例代码或提示]```

[其他步骤...]

## 成功指标

- [指标1]
- [指标2]
...

## IDE 实现参考

- [相关IDE实现链接]
```

### AI IDE 规则

添加 AI IDE 规则示例时，请：

- 清晰注明适用的 IDE 和版本
- 提供规则的目的和预期效果
- 包含实际使用的示例和注意事项
- 解释规则如何实现 Vibe Coding 原则

### 文档改进

改进文档时，请注意：

- 保持语言简洁明了
- 提供具体、可操作的指导
- 使用 Markdown 格式化增强可读性
- 添加相关链接，便于导航

## 评审标准

贡献将基于以下标准进行评审：

1. **符合项目目标**：是否符合 Vibe Coding 的核心理念
2. **质量和完整性**：内容是否准确、完整、结构良好
3. **实用性**：是否提供可直接应用的实践指导
4. **通用性**：是否对广泛用户有价值，而非过于特殊的场景

## 行为准则

- 尊重其他贡献者和维护者
- 接受建设性批评和反馈
- 以专业方式参与讨论
- 关注问题和技术，而非个人

## 许可证

贡献本项目，即表示您同意您的工作将在与项目相同的[MIT许可证](LICENSE)下发布。

---

再次感谢您的贡献！如有任何问题，请随时在 Issue 中提问或联系项目维护者。
