# 贡献指南（Contributing Guide）

欢迎为本项目做出贡献！本指南说明如何搭建开发环境、命名分支、编写提交信息以及提交 Pull Request。

## 开发环境配置

1. 克隆仓库并进入目录：

   ```bash
   git clone https://github.com/lijun9527x-rgb/claude-code.git
   cd claude-code
   ```

2. 安装依赖：

   ```bash
   npm install
   ```

3. 运行测试：

   ```bash
   npm test
   ```

4. 启动本地开发环境：

   ```bash
   npm run dev
   ```

## 分支命名规范

- `feature/<描述>`：新功能
- `fix/<描述>`：缺陷修复
- `docs/<描述>`：文档变更
- `refactor/<描述>`：重构
- `chore/<描述>`：构建、依赖或辅助性维护

命名要求：

- 一律使用小写字母；
- 单词之间使用中划线 `-` 分隔；
- 描述尽量简短明确，例如 `docs/add-contributing-guide`。

## 提交信息规范

遵循 [Conventional Commits](https://www.conventionalcommits.org/) 规范，格式为 `<type>: <description>`：

- `feat:` 新功能
- `fix:` 修复缺陷
- `docs:` 文档变更
- `refactor:` 重构（不改变外部行为）
- `test:` 新增或修改测试
- `chore:` 构建过程或辅助工具变动

示例：

```text
docs: add contributing guide
fix: correct timeout handling in upload
```

## Pull Request 流程

1. 从最新的默认分支（`main`）创建自己的工作分支。
2. 在分支上完成修改，并遵循上述提交信息规范提交。
3. 推送分支到远程仓库：

   ```bash
   git push origin docs/add-contributing-guide
   ```

4. 在 GitHub 上针对 `main` 分支创建 Pull Request，标题简明描述变更，正文说明修改内容与测试方式。
5. 检查 CI 是否通过，并根据审查意见进行修改。
6. 由维护者确认后合并，不要自行合并 PR。
