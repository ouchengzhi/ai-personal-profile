# 更新档案

## 流程

1. 新建 Issue，说明要修改的章节和理由（可用「档案更新申请」模板）。
2. 从 `main` 建分支，例如 `profile/communication-style`。
3. 修改 `README.md`，追加 `CHANGELOG.md` 条目。
4. 提交 PR，说明变更内容，合并回 `main`。

## 提交信息约定

`类型(范围): 简短说明`

- 类型：`docs`（内容）、`fix`（纠错）、`chore`（维护）。
- 范围：如 `profile`、`issues`、`workflow`。
- 示例：`docs(profile): 更新常用工具与技术栈`

## 追溯与回退

- 查看历史：`git log --oneline --decorate`
- 查看某次改动：`git show <提交哈希>`
- 安全回退（保留历史）：`git revert <提交哈希>`
- 对比两个版本：`git diff <旧提交> <新提交>`

> 已推送到远端的提交不要用 `git reset --hard` 或强制推送覆盖；用 `git revert` 才能保证所有人都能追溯。

## 隐私提醒

本仓库公开可见。不要提交密钥、令牌、隐私数据或他人的个人信息。
