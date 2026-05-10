---
name: github_tutorial
description: 从零开始的 GitHub 操作教程。完全小白版。
type: system
importance: medium
last_updated: 2026-05-10
---

# GitHub 从零开始教程

> 假设你完全不会 GitHub。按顺序一步一步做就行。

---

## 第一步：注册 GitHub 账号

1. 打开浏览器，访问 https://github.com
2. 点击右上角的 **Sign up**
3. 输入你的邮箱，设置密码（至少 8 位，建议用你常用的密码管理器生成）
4. 给自己起一个用户名（比如 `zhouzhengofficial`）
5. 验证邮箱（GitHub 会发一封验证邮件，点里面的链接）
6. 完成注册

---

## 第二步：创建仓库（Repository）

仓库就是存你文件的地方，类似一个文件夹。

1. 登录 GitHub 后，点右上角的 **+** 号 → **New repository**
2. **Repository name** 填：`my-ai-os`
3. **Description** 可填：`周正 AI 人格操作系统`
4. **Public / Private**：选 **Private**（私人仓库，别人看不到）
5. **不要勾** "Add a README file"（我们已经有了）
6. 点下面的 **Create repository**

创建成功后，你会看到一个页面，上面有一些代码。先放着，下一步用。

---

## 第三步：上传你的文件

### 方法 A：直接网页上传（最简单，适合第一次）

1. 在你刚创建的仓库页面，点 **uploading an existing file**（蓝色链接）
2. 打开你电脑上的 `C:\Users\Administrator\my-ai-os` 文件夹
3. **全选**所有文件和文件夹，**拖进**浏览器页面
4. 往下滑，点 **Commit changes**
5. 在弹窗里点 **Commit changes**（直接确认）

完成！你的文件已经上传到 GitHub 了。

### 方法 B：用命令行（后续维护用）

> 这个方法在你电脑装了 Git 之后才能用。但强烈建议学会，因为后面更新文件会方便很多。

1. **安装 Git**：访问 https://git-scm.com/download/win，下载安装，一路点"下一步"
2. 装好后，在桌面点右键 → **Git Bash Here**
3. 在弹出的黑窗口里，一行一行输入以下命令（每输一行按一次回车）：

```bash
cd ~/my-ai-os
```

```bash
git init
```

```bash
git add .
```

```bash
git commit -m "第一次提交：周正AI人格OS初始化"
```

```bash
git branch -M main
```

```bash
git remote add origin https://github.com/你的用户名/my-ai-os.git
```

> 把上面的 `你的用户名` 换成你注册时用的用户名

```bash
git push -u origin main
```

这时会弹出一个浏览器窗口让你登录 GitHub，登录就行。

---

## 第四步：后续怎么更新文件

当你修改了 `my-ai-os/` 里的文件后，按以下步骤上传更新：

1. 打开 **Git Bash**
2. 依次输入：

```bash
cd ~/my-ai-os
git add .
git commit -m "更新说明（比如：补充了商业模块内容）"
git push
```

三行命令搞定。

---

## 第五步：怎么用 Claude Code 连接

每次启动 Claude Code 时，它会自动读取当前目录下的文件。

1. 在终端里进入你的项目目录：

```bash
cd ~/my-ai-os
```

2. 启动 Claude Code：

```bash
claude
```

Claude Code 会自动读取 `AI_START.md` 和所有模块文件，按照你的人格系统来工作。

如果你把项目上传到了 GitHub，更换电脑时只需要：

```bash
git clone https://github.com/你的用户名/my-ai-os.git
cd my-ai-os
claude
```

---

## 第六步：如何备份

你上传到 GitHub 之后，就已经自动备份了。

额外建议：
- **密码**用密码管理器记（推荐 Bitwarden 或 Apple 钥匙串）
- 不要跟别人分享你的 Private 仓库
- 定期（比如每月一次）运行 `git push` 确保最新版本在云端

---

## 第七步：长期维护建议

- **每次修改了重要内容** → 运行 `git add .` + `git commit -m "说明"` + `git push`
- **不要上传敏感信息**（密码、API Key 等）→ .gitignore 已经帮你屏蔽了常见文件
- **定期整理** 6_memory/ 和 7_ai_training/ 里的内容

---

## 常见问题

**Q：忘记了 GitHub 密码？**
A：去 https://github.com/password_reset 用邮箱重置

**Q：上传时提示文件太大？**
A：GitHub 单文件不能超过 100MB。你的 AI OS 文件都很小，不会有这个问题

**Q：想删除仓库？**
A：进仓库 Settings → 拉到最下面 → Danger Zone → Delete this repository

**Q：想从私有改成公开？**
A：进仓库 Settings → 拉到中间 → Change visibility → 选 Public

---

## 词汇表

| 术语 | 意思 |
|------|------|
| Repository | 仓库，存文件的地方 |
| Commit | 提交，把修改保存成一个版本 |
| Push | 上传，把本地的版本传到云端 |
| Clone | 克隆，从云端下载到本地 |
| Branch | 分支，创建独立的版本线（初期不需要用） |
| Main | 主分支，你最主要的版本线 |
