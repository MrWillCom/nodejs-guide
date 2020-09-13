# Git

[Git](https://git-scm.com/) 是非常著名的代码版本管理系统，它由 Linus Torvalds 开发，功能强大、稳定，是管理代码的最佳选择。

使用 Git 需要会使用[命令行](./command-line.md)，但如果你有 [GUI 客户端](#GUI-客户端)，则不必学习命令行。

## 命令

以下是常用的 Git 命令，更多命令请参阅[参考文献](#参考文献)：

### 克隆

如下命令可以克隆本仓库：

```sh
git clone https://github.com/techs-docs/nodejs-guide.git
```

使用方法如下：

```sh
git clone [仓库链接]
```

### 拉取

拉取操作用于同步远程仓库的修改：

```sh
git pull
```

### 提交

提交用于提交当前的修改，需要提供提交注释：

```sh
git commit -m "注释"
```

### 推送

推送将会把所有提交推送到远程仓库：

```sh
git push
```

## GUI 客户端

你可以在 [Git 官网](https://git-scm.com/downloads/guis)上找到很多 GUI 客户端，

## 参考文献

- [Git - Documentation](https://git-scm.com/doc)
- [Git - Book](https://git-scm.com/book)
- [Git - Book（简体中文）](https://git-scm.com/book/zh)
