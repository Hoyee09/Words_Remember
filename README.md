# 英文背单词与检测

一个无需后端、无需安装依赖的英文单词学习与检测网站。

## 功能

- 695 个词条，包含音标、词性、中文释义和例句
- 英译中随机选择题，正确答案与干扰项位置随机
- 全部词汇、已掌握、未掌握三个视图
- 中文释义可逐条显示或一键全部显示
- 全部词汇支持随机打乱顺序
- 学习进度保存在浏览器本地

## 本地使用

直接双击 `index.html` 即可。

## 部署到 GitHub Pages

### 方式一：GitHub Actions 自动部署（推荐）

1. 在 GitHub 新建一个仓库。
2. 把本文件夹中的全部文件上传到仓库，包括 `.github` 文件夹和 `.nojekyll`。
3. 打开仓库的 `Settings` → `Pages`。
4. 在 `Build and deployment` 中把 `Source` 选择为 `GitHub Actions`。
5. 向 `main` 或 `master` 分支推送代码。
6. 在仓库的 `Actions` 页面等待 `Deploy static site to GitHub Pages` 完成。

发布地址通常为：

```text
https://你的用户名.github.io/仓库名/
```

### 方式二：从分支直接发布

1. 把全部文件上传到 `main` 分支。
2. 打开仓库的 `Settings` → `Pages`。
3. 在 `Build and deployment` 中选择 `Deploy from a branch`。
4. 分支选择 `main`，目录选择 `/(root)`，然后保存。

## 文件说明

- `index.html`：完整网站，HTML、CSS、JavaScript 和词库均在其中
- `.github/workflows/pages.yml`：GitHub Pages 自动部署配置
- `.nojekyll`：避免 GitHub Pages 使用 Jekyll 处理站点
- `README.md`：使用与部署说明

网站不依赖外部 CDN，发布后只需要这个静态页面即可运行。
