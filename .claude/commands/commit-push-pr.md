---
allowed-tools: Bash(git status:*), Bash(git diff:*), Bash(git add:*), Bash(git commit:*), Bash(git push:*), Bash(gh pr create:*), Bash(git log:*), Bash(git branch:*)
description: 提交更改、推送到远程并创建一个 Pull Request
---


## your task

1. 查看当前 git 状态和更改内容
2. 如果有未提交的更改，提示用户输入提交信息，然后执行：
   - git add -A 暂存所有更改
   - git commit -m "<提交信息>"
3. 推送到远程仓库 (git push)
4. 创建一个 Pull Request：
   - 使用 gh pr create
   - 如果有远程分支，使用 --web 选项打开浏览器创建 PR
   - 否则提示用户先设置远程仓库
5. 展示结果