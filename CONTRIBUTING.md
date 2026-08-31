# Contributing

感谢你对 claude-code 项目的关注与支持!

这份指南介绍如何为该项目贡献代码、文档或其他改动。请阅读并遵循以下约定。

## 开发环境配置

1. 克隆仓库并切换工作目录:

   ```bash
   git clone https://github.com/lijun9527x-rgb/claude-code.git
   cd claude-code
   ```

2. 安装依赖:

   ```bash
   npm install
   ```

3. 运行测试:

   ```bash
   npm test
   ```

4. 本地运行以验证改动。确保 Node.js 版本符合 package.json 中 engines 字段的要求。

## 分支命名规范

请基于默认分支(通常是 `main` 或 `master`)创建功能分支,并使用形如 `<type>/<short-description>` 的命名约定:

- `feat/<描述>`:新功能,例如 `feat/add-logging`
- `fix/<描述>`:缺陷修复,例如 `fix/parse-error`
- `docs/<描述>`:文档改动,例如 `docs/add-contributing-guide`
- `refactor/<描述>`:重构,例如 `refactor/stream-handler`
- `test/<描述>`:测试改动,例如 `test/unit-for-parser`
- `chore/<描述>`:杂项任务,例如 `chore/update-deps`

分支名应使用小写字母、数字、连字符,不要包含空格。

## 提交信息规范

提交信息应当清晰地描述改动内容,遵循 Conventional Commits 约定:

- 格式:`<type>(<scope>): <subject>`
- `type` 可选值:`feat`、`fix`、`docs`、`refactor`、`test`、`chore` 等
- `scope` 可选,表示影响的范围
- `subject` 使用祈使句,首个字母小写,不超过 72 字符

示例:

```
docs: add contributing guide
feat(cli): support interactive mode
fix(auth): handle token refresh failure
```

## Pull Request 流程

1. 在新分支上完成改动并提交。
2. 确保所有测试通过:运行 `npm test`。
3. 推送分支到远端:

   ```bash
   git push -u origin <branch-name>
   ```

4. 创建 Pull Request,标题遵循提交信息规范,例如 `docs: add contributing guide`。
5. 在 PR 描述中说明改动内容、动机以及测试方式。
6. 等待维护者评审;根据反馈更新分支并推送,PR 会自动更新。
