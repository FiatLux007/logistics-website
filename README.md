# 鸿运物流网站

一个使用GitHub Pages部署的现代化货运物流公司网站。

## 🚀 在线演示

访问地址：`https://你的用户名.github.io/logistics-website`

## 📋 功能特色

- **响应式设计**：完美适配桌面、平板和手机设备
- **现代化UI**：使用渐变色和阴影效果的现代设计风格
- **在线报价**：智能运费计算器
- **联系表单**：完整的客户咨询表单
- **动画效果**：流畅的滚动动画和交互效果
- **SEO优化**：完善的meta标签和结构化数据

## 🏗️ 网站结构

```
logistics-website/
├── index.html          # 首页
├── about.html           # 关于我们
├── services.html        # 服务介绍
├── contact.html         # 联系我们
├── quote.html           # 在线报价
├── css/
│   └── style.css        # 主要样式文件
├── js/
│   └── main.js          # JavaScript功能
├── images/              # 图片文件夹
└── README.md           # 项目说明
```

## 🛠️ 本地开发

### 1. 克隆项目
```bash
git clone https://github.com/你的用户名/logistics-website.git
cd logistics-website
```

### 2. 本地预览
由于是静态网站，可以直接用浏览器打开`index.html`文件预览。

或者使用简单的HTTP服务器：
```bash
# Python 3
python -m http.server 8000

# Node.js
npx serve .

# PHP
php -S localhost:8000
```

然后访问 `http://localhost:8000`

## 📦 部署到GitHub Pages

### 方法一：GitHub网页界面
1. 登录GitHub，进入仓库
2. 点击 Settings > Pages
3. Source 选择 "Deploy from a branch"
4. Branch 选择 "main"，文件夹选择 "/ (root)"
5. 点击 Save

### 方法二：命令行部署
```bash
# 添加所有文件
git add .

# 提交更改
git commit -m "Initial website setup"

# 推送到GitHub
git push origin main
```

部署完成后，网站将在 `https://你的用户名.github.io/logistics-website` 可访问。

## 🎨 自定义配置

### 修改公司信息
在以下文件中更新你的公司信息：
- `index.html` - 首页公司介绍
- `contact.html` - 联系方式和地址
- `about.html` - 公司历史和团队信息

### 修改颜色主题
在 `css/style.css` 中修改CSS变量：
```css
:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    --accent-color: #f093fb;
}
```

### 添加真实图片
1. 将图片放入 `images/` 文件夹
2. 更新HTML中的图片路径
3. 建议的图片尺寸：
   - 英雄区域背景：1920x1080px
   - 服务图片：400x300px
   - 团队照片：300x300px

## 🔧 高级功能

### 集成地图API
在 `contact.html` 中替换地图占位符：
```html
<!-- 百度地图 -->
<div id="map" style="width:100%;height:400px;"></div>
<script src="//api.map.baidu.com/api?v=3.0&ak=您的密钥"></script>

<!-- 高德地图 -->
<div id="map" style="width:100%;height:400px;"></div>
<script src="//webapi.amap.com/maps?v=1.4.15&key=您的密钥"></script>
```

### 添加表单后端处理
推荐使用：
- **Formspree**：简单的表单处理服务
- **Netlify Forms**：如果迁移到Netlify
- **EmailJS**：纯前端邮件发送服务

### Google Analytics集成
在每个HTML文件的 `<head>` 中添加：
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

## 📱 响应式断点

- **桌面端**：1200px+
- **平板端**：768px - 1199px
- **手机端**：767px及以下

## 🌐 浏览器支持

- Chrome (推荐)
- Firefox
- Safari
- Edge
- IE11+ (基本支持)

## 📝 许可证

MIT License - 可自由使用和修改

## 🤝 贡献

欢迎提交Issue和Pull Request来改进这个项目！

## 📞 技术支持

如果在使用过程中遇到问题，可以：
1. 查看GitHub Issues
2. 提交新的Issue
3. 发邮件至：support@example.com

---

**祝你的物流网站建设顺利！** 🚛✨