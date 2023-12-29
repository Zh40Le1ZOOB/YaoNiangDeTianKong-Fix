# 参与开发

## 注意事项

- 中文部分使用全角标点，英文部分使用半角标点。

- 严格区分英文大小写，尤其是专有名词。优先使用专有名词的显示名称（Display Name），如果没有则使用唯一名称（Unique Name）。

- 严格注意专有名词中空格的使用，如果原词中没有空格切勿添加空格，反之如果原词中有空格切勿删去空格。使用 AutoCorrect 检查纠正时如果专有名词被错误地纠正，请参考 AutoCorrect 自述文件 [Configuration](https://github.com/huacnlee/autocorrect#configuration) 部分在 AutoCorrect 配置文件`.autocorrectrc`中添加忽略规则。

## 简单修改

直接在对应章节的网页版点击右上角的修改按钮修改并创建 Pull request。

## 高级开发

1. 安装 Rust 环境。

2. 通过 Cargo 安装本项目使用的 mdBook 复刻。

```shell
cargo install --git https://github.com/Zh40Le1ZOOB/mdBook mdbook
```

3. 安装 [AutoCorrect](https://github.com/huacnlee/autocorrect)。

4. 复刻本项目仓库并克隆至本地。

```shell
git clone https://github.com/Zh40Le1ZOOB/YaoNiangDeTianKong-Fix
```

5. 使用任何文本编辑器修改并通过以下代码启动浏览器测试。

```shell
mdbook serve --open
```

6. 使用 AutoCorrect 检查纠正。

```shell
autocorrect --fix
```

7. 确认修改无误后使用 Git 提交并推送。

8. 创建 Pull request。

## 参与核心开发

您可能需要掌握以下技能：

- HTML & CSS & JavaScript 用于开发本项目的前端页面。

- Rust 用于为 mdBook 开发本项目需要的新功能。

以下的 TODO 是正在开发或待开发的功能，您可以通过 Issues、Pull request、Discussions 与开发者讨论。

TODO：

- 改进底部导航键样式及防烧屏措施。

- 本地阅读版本下载按钮。

- PDF 版本支持。

- DOCX 版本支持。

- TXT 版本支持。

- 让 mdBook 支持中文搜索。
