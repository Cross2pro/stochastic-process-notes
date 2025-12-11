# 随机过程笔记项目说明

## 工作流程

1. **编写或编辑 Markdown 文件**
   - 在本项目目录下，所有笔记和课后题答案均以 `.md` 格式保存。

2. **Markdown 转 HTML**
   - 使用 `md2html.sh` 脚本将 Markdown 文件转换为 HTML 文件。
   - 脚本用法：
     ```bash
     ./md2html.sh 输入文件.md 输出文件.html
     ```
   - 例如：
     ```bash
     ./md2html.sh 随机过程课后题第三章答案.md print.html
     ```
   - 脚本会自动调用 pandoc，并应用 `style.css` 样式和 MathJax 数学公式支持。

3. **用浏览器打开 HTML 文件**
   - 在文件管理器中双击生成的 HTML 文件，或在终端输入：
     ```bash
     xdg-open print.html
     ```
   - 也可以用其它浏览器（如 Chrome、Firefox）打开。

4. **打印为 PDF**
   - 在浏览器中按 `Ctrl+P`，选择“另存为 PDF”或直接打印。

## 依赖环境
- 需要安装 pandoc。
- 推荐使用 Linux 或 macOS 环境。

## 附加说明
- `style.css` 可自定义页面样式。
- 数学公式自动支持，无需额外配置。

---
如有问题请提交 issue 或联系维护者。
