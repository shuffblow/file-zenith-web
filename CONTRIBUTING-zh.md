# 贡献指南

非常感谢你有兴趣为本项目贡献代码！为了使贡献过程尽可能顺利，请遵循以下指南。

## 如何开始

### 1. Fork 仓库

首先，fork 仓库到你的 GitHub 账户中。这会创建一个你自己的仓库副本。

### 2. 克隆仓库

在你的本地机器上克隆你刚刚 fork 的仓库：

```bash
git clone https://github.com/你的用户名/file-zenith-web.git
cd file-zenith-web
```

### 3. 添加上游远程仓库

为了保持你的仓库与原始仓库同步，请添加上游远程仓库：

```bash
git remote add upstream https://github.com/code-cracks/file-zenith-web.git
```

### 4. 创建新分支

在开始工作之前，请确保你创建了一个新的分支。分支名应遵循"功能类型/功能描述"的格式：

```bash
git checkout -b feat/功能描述
```

分支类型可以是：

- `feat`: 新功能
- `fix`: 修复
- `docs`: 文档
- `style`: 样式
- `refactor`: 重构
- `perf`: 性能优化
- `test`: 测试
- `chore`: 其他修改

例如：`feat/home`、`fix/login-bug`、`docs/api-guide`

## 开发流程

### 1. 安装依赖

在你开始开发之前，请安装所有的依赖：

```bash
pnpm install
```

### 2. 运行项目

为了确保你在一个正常运行的环境下进行开发，启动项目：

```bash
pnpm dev
```

### 3. 进行开发

请遵循以下开发准则：

- 确保代码清晰、简洁。
- 遵循项目的代码风格和规范（使用 ESLint 和 Prettier）。
- 如果你添加了新功能，请编写相应的测试。
- 如果你修复了 bug，请添加测试来防止将来再次出现。

### 4. 代码检查与格式化

在提交你的更改之前，请确保你进行了适当的代码格式化和 lint：

```bash
pnpm lint
pnpm format
```

你也可以运行类型检查来确保类型安全：

```bash
pnpm type-check
```

### 5. 提交更改

本项目使用 commitlint 和 commitizen 来规范提交信息。请使用以下命令来提交你的更改：

```bash
pnpm commit
```

这将启动交互式提交过程，引导你选择提交类型（如 feat、fix、docs 等）并填写提交信息。以下是填写各个字段的指南：

1. **选择提交类型（Select the type of change）**：

   - 使用方向键选择最适合你的更改的类型
   - 提交类型包括：
     - `feat`: 🚀 新功能
     - `fix`: 🧩 修复 bug
     - `docs`: 📚 文档变更
     - `style`: 🎨 代码格式变更（不影响代码运行）
     - `refactor`: ♻️ 代码重构（既不是新增功能，也不是修复 bug）
     - `perf`: ⚡️ 性能优化
     - `test`: ✅ 添加或修改测试
     - `build`: 📦️ 构建系统或外部依赖变更
     - `ci`: 🎡 CI 配置变更
     - `chore`: 🔨 其他变更（不修改 src 或测试文件）
     - `revert`: ⏪️ 回退之前的提交

2. **选择影响范围（Denote the SCOPE）**：

   - 这是可选的，用于指明你的更改影响的范围
   - 可以是组件名称、文件名、功能区域等
   - 如果更改影响多个范围或不确定，可以选择 "empty"
   - 如果需要自定义范围，可以选择 "custom" 并输入自定义范围

3. **简短描述（Write a SHORT description）**：

   - 用一句简短的话描述你的更改
   - 使用祈使句（命令式）语气，如 "添加用户登录功能" 而不是 "添加了用户登录功能"
   - 不需要首字母大写，也不需要在末尾加句号

4. **详细描述（Provide a LONGER description）**：

   - 这是可选的，用于提供更详细的更改说明
   - 可以描述更改的原因、实现方式等
   - 使用 "|" 来换行

5. **破坏性变更（BREAKING CHANGES）**：

   - 如果你的更改会破坏现有的 API 或功能，请在这里说明
   - 详细描述破坏性变更的内容和迁移方法
   - 使用 "|" 来换行

6. **关联的 Issues（List any ISSUES）**：

   - 如果你的更改与某个 Issue 相关，可以在这里列出
   - 格式为 "#Issue编号"，如 "#31", "#34"

7. **确认提交（Are you sure）**：
   - 检查你的提交信息，确认无误后选择 "yes"

完成以上步骤后，你的提交信息将被格式化并提交到仓库。

### 6. 同步你的分支

在你准备好提交你的更改之前，请确保你的分支是最新的：

```bash
git fetch upstream
git rebase upstream/main
```

### 7. 推送分支

将你的分支推送到你自己的仓库：

```bash
git push origin feat/功能描述
```

### 8. 创建 Pull Request

在 GitHub 上，导航到你 fork 的仓库，点击 "Compare & pull request" 按钮。请确保你详细描述了你所做的更改。

## 代码审查

所有的 Pull Request 都会被审查。请注意以下几点：

- 你的代码是否清晰且易于理解。
- 你是否遵循了项目的代码风格和规范。
- 你是否添加了适当的测试。
- 你的更改是否与现有的代码兼容。

## 常见问题

### 如何报告 Bug？

如果你发现了 Bug，请在 GitHub 上创建一个 Issue，并尽可能详细地描述 Bug 及其复现步骤。

### 如何请求新功能？

如果你有新功能的建议，请在 GitHub 上创建一个 Issue，详细描述你的建议及其潜在的用途。

## 联系我们

如果你有任何问题或需要帮助，请在 GitHub 上提问或创建 Issue。
