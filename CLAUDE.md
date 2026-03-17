# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个用于学习和探索 Claude Code（Anthropic 的 CLI 工具）的项目。项目主要包含对 Claude Code 功能的实践和自定义配置。

## 架构和文件结构

- **根目录**：包含项目配置文件和文档
- **.claude/commands/**：自定义 slash commands 配置目录
  - `git-init.md`：初始化 git 仓库的命令
  - `commit-push-pr.md`：提交代码、推送到远程并创建 Pull Request 的命令

## 常用命令

### 自定义 Slash Commands

项目提供了两个自定义命令，可通过 `/git-init` 和 `/commit-push-pr` 使用：

#### 1. `/git-init`（初始化 git 仓库）

**功能**：

- 初始化新的 git 仓库
- 自动创建初始提交（包含所有文件）
- 展示操作结果

**使用场景**：在新项目或未初始化的项目中快速设置 git 仓库

#### 2. `/commit-push-pr`（提交和创建 PR）

**功能**：

- 检查 git 状态和更改内容
- 暂存并提交更改（支持自定义提交信息）
- 推送到远程仓库
- 使用 GitHub CLI 创建 Pull Request
- 处理远程分支和仓库设置

**使用场景**：完成代码更改后，快速提交并创建 PR 的完整工作流程

## 开发工作流程

1. 使用 `/git-init` 初始化项目（如果未初始化）
2. 进行代码更改
3. 使用 `/commit-push-pr` 提交更改并创建 PR
4. 遵循标准的 git 工作流程

## 配置说明

- `git-init` 命令配置文件：`.claude/commands/git-init.md`
- `commit-push-pr` 命令配置文件：`.claude/commands/commit-push-pr.md`

这些配置文件定义了命令的行为、允许使用的工具和执行步骤。
