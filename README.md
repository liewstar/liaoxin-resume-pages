# Liaoxin Resume Pages

这个仓库用于 GitHub Pages 展示简历首页，打开后直接显示前两页简历（HTML 渲染）。

## 文件结构

- `index.html`：页面入口
- `resume.pdf`：简历 PDF 原件

## 本地预览

```bash
python -m http.server 8000
```

打开 `http://localhost:8000` 即可。

## 发布到 GitHub Pages

1. 在 GitHub 新建仓库，例如 `liaoxin-resume-pages`
2. 上传本目录所有文件，或者执行命令：

```bash
git init
git add .
git commit -m "init resume pages"
git branch -M main
git remote add origin https://github.com/<你的用户名>/liaoxin-resume-pages.git
git push -u origin main
```

3. 进入仓库 `Settings -> Pages`
4. `Build and deployment` 选择 `Deploy from a branch`
5. Branch 选择 `main`，目录选择 `/ (root)`，保存

几分钟后访问：

`https://<你的用户名>.github.io/liaoxin-resume-pages/`

## 替换简历

新简历直接覆盖 `resume.pdf`，然后提交并推送即可。
