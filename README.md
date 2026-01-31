## 📝 项目简介

这是一个为高中开发者（高一学生）设计的个人主页项目，采用现代、简约且温暖的设计风格。项目完全响应式，适配各种设备，包含完整的个人展示、技能展示、作品集和联系方式。

## ✨ 核心特性

### 🎨 设计风格
- **温暖配色方案**：使用奶油色背景、陶土色和鼠尾草绿等柔和色调
- **玻璃拟态效果**：现代UI设计，半透明模糊卡片
- **优雅字体组合**：Varela Round + ZCOOL QingKe HuangYou
- **圆角设计语言**：所有元素采用一致的圆角风格

### 📱 响应式布局
- 完全适配移动端、平板和桌面端
- 自适应导航栏和菜单
- 弹性布局，确保在各种屏幕尺寸下完美显示

### 🎯 交互体验
- **聚光灯跟随效果**：鼠标移动时的聚光灯动画
- **自适应圆圈按钮**：动态尺寸的交互式按钮
- **平滑滚动**：页面内导航的平滑过渡
- **悬停动画**：元素悬停时的微妙动画效果

## 🚀 快速开始

### 前置要求
- 现代浏览器（Chrome, Firefox, Safari, Edge）
- 网络连接（用于加载CDN资源）

### 安装与使用

1. **克隆仓库**
   ```bash
   git clone https://github.com/XiaoQius/xusn-portfolio.git
   cd xusn-portfolio
   ```

2. **直接使用**
   - 项目是纯HTML/CSS/JS，无需构建步骤
   - 直接在浏览器中打开 `index.html`
   - 作为个人网站部署到任何静态托管服务

3. **自定义内容**
   - 修改HTML中的个人信息
   - 替换头像URL
   - 更新技能进度和项目信息
   - 修改联系方式和链接

## 📁 项目结构

```
xusn-portfolio/
├── index.html          # 主页面
├── 404.html           # 404错误页面
├── assets/            # 静态资源（可选）
│   ├── images/        # 图片
│   └── fonts/         # 字体文件
└── README.md          # 项目说明
```

## 🎨 设计系统

### 颜色方案
```css
cream: #FDFBF7         /* 主背景色 */
warm-800: #5C4F42     /* 主要文字/按钮 */
clay-500: #C4956A     /* 强调色/按钮 */
sage-500: #7A9E77     /* 次要强调色 */
```

### 字体组合
- **标题**：ZCOOL QingKe HuangYou (思源宋体)
- **正文**：Varela Round (圆体)
- **回退**：PingFang SC, Microsoft YaHei

### 组件风格
- **玻璃卡片**：半透明背景 + 模糊效果
- **圆角按钮**：统一圆角半径
- **渐变文字**：用于标题和强调文本

## 📦 依赖说明

### CDN 资源
```html
<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Varela+Round&family=ZCOOL+QingKe+HuangYou&display=swap" rel="stylesheet">

<!-- Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
```

### 本地资源（可选）
如果希望完全离线使用，可以下载上述资源到本地。

## 🔧 自定义指南

### 1. 修改个人信息
在 `index.html` 中找到以下部分并替换内容：

```html
<!-- 头像 -->
<img src="你的头像URL" alt="你的名字">

<!-- 标题 -->
<h1>你的名字</h1>
<p>你的描述</p>

<!-- 联系方式 -->
<a href="mailto:你的邮箱">你的邮箱</a>
<a href="https://github.com/你的用户名">GitHub</a>
```

### 2. 更新技能展示
```html
<div class="progress-fill" data-width="85%"></div>
<!-- 修改 data-width 值来调整进度条 -->
```

### 3. 添加/修改项目
```html
<div class="group glass-card rounded-[2rem] overflow-hidden hover-float">
    <div class="h-44 rounded-2xl bg-gradient-to-br ...">
        <i class="fas fa-globe ..."></i>
    </div>
    <h3>项目名称</h3>
    <p>项目描述</p>
    <a href="项目链接">查看详情</a>
</div>
```

### 4. 更改配色方案
在 `<style>` 标签中修改CSS变量：

```css
:root {
    --cream: #FDFBF7;
    --warm-800: #5C4F42;
    --clay-500: #C4956A;
    --sage-500: #7A9E77;
}
```

## 🌐 部署建议

### 静态托管服务
1. **GitHub Pages**（推荐）
   ```bash
   # 在仓库设置中启用GitHub Pages
   # 选择gh-pages分支作为源
   ```

2. **Vercel / Netlify**
   - 连接GitHub仓库
   - 自动部署

3. **Cloudflare Pages**
   - 免费的静态网站托管
   - 自动HTTPS

### 本地测试
```bash
# 使用Python内置服务器
python -m http.server 8000

# 或使用Node.js（需要安装http-server）
npx http-server
```

## 📱 移动端优化

### 触摸交互
- 按钮大小适配触摸操作
- 避免使用纯悬停效果（在移动设备上无效）
- 使用 `:active` 状态提供反馈

### 性能优化
- 使用CDN加载资源
- 图片懒加载（可选）
- 最小化第三方脚本

## 🎯 适用场景

- 高中生/大学生个人作品集
- 开发者简历展示
- 个人博客首页
- 作品集网站
- 求职简历页面

## 📝 贡献指南

欢迎贡献！请遵循以下步骤：

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

## 📄 许可证

本项目采用 **MIT 许可证** - 详见 [LICENSE](LICENSE) 文件

## 🙏 致谢

- [Tailwind CSS](https://tailwindcss.com/) - 样式框架
- [Font Awesome](https://fontawesome.com/) - 图标库
- [Google Fonts](https://fonts.google.com/) - 字体
- [hitokoto](https://hitokoto.cn/) - 一言API（可选）

## 📞 联系方式

如有问题或建议，请通过以下方式联系：

- GitHub Issues: [创建Issue](https://github.com/XiaoQius/xusn-portfolio/issues)
- 邮箱: 你的邮箱
- 项目链接: [https://github.com/XiaoQius/xusn-portfolio](https://github.com/XiaoQius/xusn-portfolio)

## 🌟 支持

如果这个项目对你有帮助，请给项目一个 ⭐️ Star！

---

**项目状态**: ✅ 稳定版本 v1.0.0

**最后更新**: 2026年1月

**作者**: XUSN (绪深)
