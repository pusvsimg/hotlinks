# HotLinks - 现代化网站导航

![HotLinks Logo](https://github.com/bbylw/hotlinks/blob/main/demo.png)

> 一个由 Claude 3.7 Sonnet AI 辅助开发的现代化网站导航项目，UI和配色模仿 youporn 风格设计。

## 🌟 特点

- **现代化UI设计**：采用优雅的卡片布局和流畅的动画效果
- **精美配色方案**：以橙色渐变为主题，搭配深色模式支持
- **响应式布局**：完美适配各种设备屏幕
- **智能分类**：网站资源分类清晰，快速定位
- **实时搜索**：支持即时搜索功能
- **深色模式**：内置优雅的深色主题切换
- **动态内容生成**：使用JavaScript动态生成网站卡片，便于维护和更新

## 🎨 设计特色

- 渐变主题色：#ff5e00 → #f90
- 现代化卡片设计
- 平滑过渡动画
- 精心设计的图标和排版
- 优雅的阴影效果

## 🛠️ 技术栈

- HTML5
- CSS3 (现代特性)
- 原生JavaScript
- Font Awesome 图标 (v6.4.2)
- 动态内容生成

## 🚀 部署指南

### GitHub Pages 部署

1. Fork 本仓库
2. 进入仓库设置 Settings → Pages
3. Source 选择 main 分支
4. 保存后等待部署完成

### Cloudflare Pages 部署

1. 在 Cloudflare Dashboard 中选择 Pages
2. 点击 "Create a project"
3. 连接你的 GitHub 账号并选择本仓库
4. 部署设置：
   - 构建命令：留空
   - 构建输出目录：留空
5. 点击 "Save and Deploy"

## 🤖 AI 开发说明

本项目由 Claude 3.7 Sonnet AI 辅助开发，主要负责：

- UI/UX 设计方案
- 代码实现和优化
- 文档编写

## 📝 开源协议

MIT License

## 🔧 自定义配置

### 网站分类

当前网站分类包括：

- **Ai搜索** - AI相关工具和搜索引擎
- **社交媒体** - 社交网络和媒体平台
- **实用工具** - 各类在线工具和服务
- **科技资讯** - 科技新闻和资讯网站
- **云存储** - 云存储和文件共享服务
- **电子邮箱** - 电子邮件服务提供商

### 添加新网站

在 `index.html` 文件中的 `categoriesData` 对象中添加新的网站数据：

```javascript
const categoriesData = {
  categoryName: [
    // 添加新网站
    { href: "https://example.com", icon: "fas fa-icon-name", title: "网站名称" },
  ],
  // 其他分类...
};
```

### 添加新分类

1. 在导航栏中添加新分类链接：

```html
<ul class="nav-links">
  <!-- 添加新分类 -->
  <li><a href="#new-category" data-target="new-category">新分类名称</a></li>
</ul>
```

2. 在 `categoriesData` 对象中添加新分类：

```javascript
const categoriesData = {
  // 现有分类...
  
  // 添加新分类
  "new-category": [
    { href: "https://example.com", icon: "fas fa-icon-name", title: "网站名称" },
    // 添加更多网站...
  ],
};
```

### Font Awesome 图标

访问 [Font Awesome Icons](https://fontawesome.com/icons) 查找合适的图标类名。支持以下图标类型：

- `fa-solid` - 实心图标
- `fa-regular` - 线框图标
- `fa-brands` - 品牌图标

## 🙏 致谢

- [Font Awesome](https://fontawesome.com) - 图标支持
- [Google Fonts](https://fonts.google.com) - 字体支持
- Claude 3.7 Sonnet - AI 开发助手
- [PornNav](https://github.com/bbylw/p) - 原始项目灵感

---

> 🎉 欢迎 Star 和 Fork！如果觉得项目不错，请点个 Star 支持一下！
