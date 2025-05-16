# Vibe Coding Best Practices

<p align="center">
  <img src="https://via.placeholder.com/150?text=Vibe+Coding" alt="Vibe Coding Logo" width="150" height="150">
</p>

<p align="center">
  <em>A collection of best practices for human-AI pair programming based on Vibe Coding principles</em>
</p>

<p align="center">
  <a href="#overview">Overview</a> •
  <a href="#key-principles">Key Principles</a> •
  <a href="#methods">Methods</a> •
  <a href="#impl">Implementations</a> •
  <a href="#getting-started">Getting Started</a> •
  <a href="#contributing">Contributing</a> •
  <a href="#license">License</a>
</p>

## Overview

**Vibe Coding Best Practices** is a curated collection of principles, methods, and practical implementations for effective human-AI collaboration in software development. Rather than being a rigid methodology, it offers practical guidance on how to leverage AI coding assistants more effectively throughout the software development lifecycle.

This project focuses on structuring the interaction between humans and AI coding assistants to achieve:

- Clear intent communication
- Effective context management
- Consistent and high-quality code generation
- Streamlined workflows across different development phases

## Key Principles

Vibe Coding is built on Ten Golden Principles that guide effective human-AI collaboration in software development. These principles focus on clear intent communication, iterative refinement, and effective context management.

```
Principle #1: Intent is the source of truth
Principle #2: Isomorphic mapping between human intent and AI understanding
...
```

Available in both languages:
- [Read in English →](./principles/golden-rules.en.md)
- [阅读中文版 →](./principles/golden-rules.zh.md)

## Methods

Our methods provide stage-specific guidance for applying Vibe Coding principles throughout the software development lifecycle:

- [需求分析 (Requirements Analysis)](./methods/requirements.md) - 通过AI辅助进行清晰意图定义和需求收集的技巧
- [设计 (Design)](./methods/design.md) - 与AI协作进行架构和设计的方法
- [实现 (Implementation)](./methods/implementation.md) - 高效代码生成和优化策略
- [维护 (Maintenance)](./methods/maintenance.md) - AI辅助重构、调试和文档编写

English versions are available in the [en/](./methods/en/) directory.

## Implementations {#impl}

We provide specific implementations and examples for popular AI coding assistants:

### Cursor

- [Overview](./impl/cursor/overview.md)
- [Rules](./impl/cursor/rules/) - Specific rule templates for Cursor

### Windsurf

- [Overview](./impl/windsurf/overview.md)
- [Rules](./impl/windsurf/rules/) - Global and workspace rule examples
- [Memories](./impl/windsurf/memories/) - Effective use of the memory system
- [Workflows](./impl/windsurf/workflows/) - Custom workflow configurations

## Getting Started

1. Start by understanding the core principles ([English](./principles/golden-rules.en.md) | [中文](./principles/golden-rules.zh.md))
2. Browse the methods for your current development phase ([中文](./methods/) | [English](./methods/en/))
3. Check the implementations section for your preferred coding assistant
4. Apply the patterns gradually in your workflow

## Contributing

We welcome contributions from the community! Whether you're sharing new best practices, improving documentation, or adding support for additional AI IDEs, please see our [Contributing Guide](./CONTRIBUTING.md) for details.

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

---

# Vibe Coding 最佳实践

<p align="center">
  <img src="https://via.placeholder.com/150?text=Vibe+Coding" alt="Vibe Coding 标志" width="150" height="150">
</p>

<p align="center">
  <em>基于 Vibe Coding 原则的人机协作编程最佳实践集</em>
</p>

<p align="center">
  <a href="#概述">概述</a> •
  <a href="#核心原则">核心原则</a> •
  <a href="#方法论">方法论</a> •
  <a href="#实现机制">实现机制</a> •
  <a href="#快速开始">快速开始</a> •
  <a href="#贡献指南">贡献指南</a> •
  <a href="#许可证">许可证</a>
</p>

## 概述

**Vibe Coding 最佳实践**是一套精心策划的原则、方法论和具体实现方案集合，旨在提升人类与AI在软件开发中的协作效率。它不是一种刻板的方法论，而是提供了如何在软件开发生命周期各阶段更有效地利用AI编程助手的实用指导。

本项目专注于构建人类与AI编程助手之间的交互结构，以实现：

- 清晰的意图传达
- 有效的上下文管理
- 一致且高质量的代码生成
- 贯穿不同开发阶段的流畅工作流

## 核心原则

Vibe Coding 建立在十大黄金法则基础上，这些原则指导人机在软件开发中的高效协作。这些原则聚焦于清晰的意图传达、迭代优化和有效的上下文管理。

```
原则一：意图是真理之源
原则二：人类意图与AI理解的同构映射
...
```

双语版本：
- [阅读中文版 →](./principles/golden-rules.zh.md)
- [Read in English →](./principles/golden-rules.en.md)

## 方法论

我们的方法论为软件开发生命周期各阶段应用Vibe Coding原则提供了具体指导：

- [需求分析](./methods/requirements.md) - 通过AI辅助进行清晰意图定义和需求收集的技巧
- [设计](./methods/design.md) - 与AI协作进行架构和设计的方法
- [实现](./methods/implementation.md) - 高效代码生成和优化策略
- [维护](./methods/maintenance.md) - AI辅助重构、调试和文档编写

英文版方法论文档位于 [en/](./methods/en/) 目录。

## 实现机制

我们为主流AI编程助手提供具体实现和示例（英文）：

### Cursor

- [概述](./impl/cursor/overview.md)
- [规则](./impl/cursor/rules/) - Cursor的具体规则模板

### Windsurf

- [概述](./impl/windsurf/overview.md)
- [规则](./impl/windsurf/rules/) - 全局和工作区规则示例
- [记忆系统](./impl/windsurf/memories/) - 记忆系统的有效使用
- [工作流](./impl/windsurf/workflows/) - 自定义工作流配置

## 快速开始

1. 首先了解核心原则（[中文](./principles/golden-rules.zh.md) | [English](./principles/golden-rules.en.md)）
2. 浏览适合您当前开发阶段的方法论（[中文](./methods/) | [English](./methods/en/)）
3. 查看您首选编程助手的实现机制
4. 在您的工作流中逐步应用这些模式

## 贡献指南

我们欢迎社区贡献！无论您是分享新的最佳实践、改进文档，还是为其他AI IDE添加支持，请查看我们的[贡献指南](./CONTRIBUTING.md)了解详情。

## 许可证

本项目采用MIT许可证 - 详情请参阅[LICENSE](./LICENSE)文件。
