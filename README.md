# 幸运奶茶订单系统

一个精美的交互式订单页面，用于收集奶茶订单信息并保存。

## 功能特点

- 🎨 精美的手绘心形动画效果
- 💝 互动式「可以」按钮，点击后洒下星星
- 📝 订单信息表单（地址、手机号、奶茶名称）
- 💾 本地数据存储功能，可查看所有提交记录
- 📱 响应式设计，适配各种屏幕尺寸

## 技术栈

- HTML5
- CSS3 (动画、渐变、响应式)
- JavaScript (交互逻辑、数据存储)
- localStorage (本地数据持久化)

## 快速开始

### 本地运行

1. 克隆仓库
   ```bash
   git clone [your-repo-url]
   cd [repository-name]
   ```

2. 启动服务器
   
   使用Python内置服务器:
   ```bash
   python -m http.server 8000
   ```
   
   或使用Node.js:
   ```bash
   npx serve
   ```

3. 在浏览器中访问
   ```
   http://localhost:8000
   ```

## 使用说明

1. 页面加载后会显示手绘心形动画和文字
2. 点击「可以」按钮后会有星星散落效果
3. 接着会弹出订单信息填写表单
4. 填写地址、手机号和想喝的奶茶名称
5. 点击「确定」后信息会自动保存
6. 点击右上角「查看提交记录」可查看所有保存的订单信息

## 数据存储

- 所有订单数据使用localStorage存储在浏览器本地
- 数据包含：地址、手机号、奶茶名称、提交时间戳
- 即使刷新页面，数据也不会丢失

## 项目结构

```
.
├── index.html       # 主页面文件
├── .gitignore       # Git忽略文件
└── README.md        # 项目说明文档
```

## 部署说明

这个项目是一个纯静态网站，可以部署在任何静态网站托管服务上。以下是详细的部署指南：

### GitHub Pages 详细配置步骤

1. **上传项目到GitHub仓库**
   - 确保已将所有文件（index.html, .gitignore, README.md, .nojekyll）上传到GitHub
   - 注意：.nojekyll文件很重要，它告诉GitHub不要使用Jekyll处理文件，避免以下划线开头的文件和目录被忽略

2. **启用GitHub Pages**
   - 进入GitHub仓库页面
   - 点击顶部导航栏的「Settings」
   - 在左侧菜单中找到并点击「Pages」
   - 在「Build and deployment」部分的「Source」下拉菜单中：
     - 选择「Deploy from a branch」
     - 在「Branch」下拉菜单中选择您的主分支（通常是main或master）
     - 在右侧下拉菜单中选择「/ (root)」
   - 点击「Save」按钮

3. **等待部署完成**
   - GitHub Pages将开始构建和部署您的网站
   - 部署完成后，您将在页面顶部看到一个绿色的提示和您的网站URL
   - URL通常格式为：https://您的用户名.github.io/仓库名/

4. **常见问题排查**
   - 如果页面空白或404错误，请检查以下几点：
     - 确保index.html文件存在于仓库的根目录
     - 确认.nojekyll文件已正确上传
     - 检查GitHub Pages配置是否正确（分支和文件夹选择）
     - 查看仓库的Actions标签页，检查部署是否有错误

### 其他部署选项

- **Netlify**：连接GitHub仓库，自动部署
- **Vercel**：导入GitHub仓库，一键部署
- **AWS S3**：上传文件并配置静态网站托管
- **阿里云OSS**：上传文件并开启静态网站托管功能

## 开发指南

如需修改或扩展项目：

1. 修改`index.html`文件中的HTML结构和JavaScript逻辑
2. 所有CSS样式都在HTML文件的`<style>`标签中
3. 所有JavaScript代码都在HTML文件的`<script>`标签中

## 注意事项

- 本项目的数据存储在浏览器本地，不同设备或浏览器无法共享数据
- 在实际生产环境中，建议使用后端服务器存储数据
- 短信功能为模拟实现，实际使用需要对接短信服务API

## License

MIT