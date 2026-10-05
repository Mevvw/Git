# Git — Mevvw 的个人工作区主仓

日常工作区的总仓库：所有项目、配置、文档以子目录形式进入本仓库统一管理。

## 目录规则

| 路径 | 用途 |
|---|---|
| `projects/<name>/` | 独立小项目（脚本、工具、实验） |
| `docs/` | 长期维护的文档、笔记 |
| `configs/` | 可复用的配置片段（git、编辑器、环境） |
| `templates/` | 项目脚手架模板 |

> 新项目从这里建子目录开始，不要在仓库根目录散放文件。

## 分支与提交

- 主分支：`main`，长期保持可推可拉
- 提交信息：`类型: 摘要`（如 `feat: 新增xx` / `fix: 修复xx` / `docs: 文档` / `chore: 杂务`）
- 不确定的大改动先开分支，稳定后合回 `main`

## 本机工具链

- Git for Windows 2.56 安装于 `D:\Git-app`（`cmd` 已在系统 PATH）
- 远程：`https://github.com/Mevvw/Git.git`（用户名内嵌于 remote URL）
- 凭据：Windows 凭据管理器托管，助手为 `git-credential-manager`
- 网络访问 GitHub 走本地代理（schannel 吊销检查已按仓库关闭）

## 常用命令

```bash
git status -sb          # 看状态
git pull --ff-only      # 拉取（不自动合并）
git push                # 推送（已配 upstream）
```
