# RoboCup Team Git Guide

这个仓库用于 RoboCup 校内赛协作开发。请把 `main` 分支当作稳定版本，日常修改放到自己的功能分支里。

## 第一次使用

1. 克隆仓库到电脑。
2. 用 VS Code 打开项目文件夹。
3. 新建自己的分支，例如 `feature/goalkeeper` 或 `feature/strategy`.
4. 修改代码后提交，再推送到 GitHub。
5. 在 GitHub 上发 Pull Request，请队友检查后合并。

## 每天开始写代码前

```bash
git switch main
git pull
git switch 你的分支名
git merge main
```

这样可以先拿到队友最新的改动，减少冲突。

## 常用命令

查看当前状态：

```bash
git status
```

提交自己的修改：

```bash
git add .
git commit -m "说明这次改了什么"
```

把分支上传到 GitHub：

```bash
git push -u origin 你的分支名
```

之后同一个分支再次上传，只需要：

```bash
git push
```

## 分支命名建议

- `feature/goalkeeper`
- `feature/striker`
- `feature/team-communication`
- `feature/path-planning`
- `fix/start-script`

## 注意事项

- 不要直接把未经测试的大改动合并进 `main`.
- 不要提交本机配置、运行日志、临时文件和无关大文件。
- 如果两个人要改同一个文件，先沟通一下分工。
- 比赛前给稳定版本打标签，例如 `v0.1-practice` 或 `v1.0-campus-match`.
