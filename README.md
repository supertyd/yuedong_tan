# Supertyd 个人学术与技术主页 🚀

欢迎来到你的 GitHub Pages 个人主页仓库！这里已经为你搭建好了一个**极具现代感、响应式且功能丰富**的单页面个人网站/作品集。

该网站完全基于静态页面构建，无需任何复杂的后台或编译流程，非常适合部署在 GitHub Pages 上。

---

## ✨ 核心亮点

- 🎨 **现代视觉设计**：采用玻璃态（Glassmorphism）和流光渐变背景，极具未来科技感。
- 🌓 **双色主题支持**：支持**深色模式（Dark Mode）**与**浅色模式（Light Mode）**，可手动切换，并会自动根据用户的系统偏好保存设置（基于 `localStorage`）。
- 📱 **完美的响应式布局**：无论是手机、平板还是超宽显示器，都能完美自适应，并拥有精美的移动端抽屉导航。
- ⚡ **动画与交互**：
  - 动态打字效果（展示不同的职业身份）。
  - 项目卡片分类过滤器（前端/全栈/工具）。
  - 顺滑的滚动过渡与卡片悬停缩放效果。
  - 带有输入验证的精美联系表单。

---

## 🛠️ 项目结构

```text
├── index.html        # 主体网页文件 (HTML5 + Tailwind CSS + Vanilla JS)
├── .gitignore        # Git 忽略配置文件
└── README.md         # 项目使用与说明文档 (当前文件)
```

---

## 🚀 如何在本地预览

由于项目是纯静态的，你可以直接用浏览器打开 `index.html`。
为了更好的开发体验，推荐使用本地轻量服务器进行预览：

### 方法 1: 使用 Python (推荐，自带且无需安装)
在项目根目录下运行：
```bash
python3 -m http.server 8000
```
然后在浏览器中访问：`http://localhost:8000`

### 方法 2: 使用 VS Code 插件
如果你使用 VS Code，可以安装 **Live Server** 插件，右键点击 `index.html` 选择 "Open with Live Server" 即可。

---

## ✏️ 如何自定义修改内容

打开 `index.html`，你只需要修改其中的文本和配置即可：

### 1. 修改个人基本信息
在 `index.html` 的 **Hero Section**（约第 108 行）和 **About Section** 中，将所有的 `Supertyd` 或 `your.email@example.com` 替换为你的真实信息。

### 2. 更改动态打字词汇
在 `index.html` 的末尾 JavaScript 部分（约第 362 行），可以修改 `words` 数组来自定义打字效果中循环显示的文案：
```javascript
const words = ['Modern Websites', 'Clean Code', 'Responsive UIs', 'Interactive Designs'];
```

### 3. 添加/修改项目卡片
在 **Projects Section**（约第 210 行）中，每个 `<div class="project-card" data-category="...">` 代表一个项目。你可以根据需要添加、删除或修改它们。
- `data-category` 支持：`frontend` / `fullstack` / `tool`（对应顶部的分类过滤器）。

---

## 🌐 如何部署到 GitHub Pages

因为你的仓库名已经是 `supertyd.github.io`，所以部署非常简单！

1. 将代码推送到你的 GitHub 仓库主分支（通常是 `main` 或 `master`）：
   ```bash
   git add .
   git commit -m "feat: init modern personal portfolio website"
   git push origin main
   ```
2. 稍等 1-2 分钟，GitHub Actions 会自动帮你构建并发布。
3. 访问你的专属网址： **`https://supertyd.github.io`** 即可公开查看！

---

祝你玩得开心！如果有任何问题，随时可以让我帮你调整或添加新的模块（如：博客、时间轴、画廊等）！🌟
