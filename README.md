# 📸 照片上传网站

一个美观、现代化的网页版照片上传应用，支持拖拽上传、预览和管理照片。

## ✨ 特性

- 🎨 **精美设计** - 现代化的UI界面，流畅的动画效果
- 🖱️ **拖拽上传** - 简单便捷的拖拽上传体验
- 💾 **本地存储** - 照片安全保存在浏览器中
- 📥 **一键下载** - 随时下载你的照片
- 📱 **响应式布局** - 完美适配各种设备

## 🚀 快速开始

### 本地运行

1. 克隆或下载此项目
2. 在项目根目录启动本地服务器：

```bash
# 使用 Python 3
python3 -m http.server 8000

# 或使用 Node.js (http-server)
npx http-server -p 8000
```

3. 在浏览器中访问 `http://localhost:8000`

## 📦 部署到 GitHub Pages

### 方法一：通过 GitHub 界面部署

1. **创建 GitHub 仓库**
   - 访问 [GitHub](https://github.com) 并登录
   - 点击右上角的 "+" → "New repository"
   - 填写仓库名称（例如：photo-uploader）
   - 选择 "Public" 或 "Private"
   - 点击 "Create repository"

2. **上传项目文件**
   - 在仓库页面点击 "uploading an existing file"
   - 将项目中的所有文件拖拽到上传区域
   - 填写提交信息，点击 "Commit changes"

3. **启用 GitHub Pages**
   - 进入仓库的 "Settings"
   - 在左侧菜单中找到 "Pages"（在 "Code and automation" 部分）
   - 在 "Build and deployment" 下：
     - "Source" 选择 "Deploy from a branch"
     - "Branch" 选择 `main` 或 `master`（根据你的默认分支）
     - 文件夹选择 `/ (root)`
   - 点击 "Save"
   - 等待几分钟，你的网站就会部署成功！

4. **访问你的网站**
   - 部署成功后，GitHub 会显示网站地址
   - 通常是：`https://<你的用户名>.github.io/<仓库名>/`

### 方法二：通过 Git 命令行部署

1. **初始化 Git 仓库**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. **连接到 GitHub 仓库**
   ```bash
   git remote add origin https://github.com/<你的用户名>/<仓库名>.git
   git branch -M main
   git push -u origin main
   ```

3. **按照方法一的第3步启用 GitHub Pages**

## 🎯 使用说明

1. **上传照片**
   - 点击 "选择照片" 按钮选择文件
   - 或直接拖拽照片到上传区域
   - 支持同时上传多张照片

2. **管理照片**
   - 鼠标悬停在照片卡片上会显示操作按钮
   - 点击下载按钮保存照片
   - 点击删除按钮移除照片
   - 点击 "清空全部" 删除所有照片

3. **支持的格式**
   - JPG / JPEG
   - PNG
   - GIF
   - WebP

## 🛠️ 技术栈

- **HTML5** - 页面结构
- **CSS3** - 样式和动画
- **JavaScript (ES6+)** - 交互逻辑
- **LocalStorage** - 本地数据存储
- **FileReader API** - 文件处理

## 📂 项目结构

```
photo-uploader/
├── index.html      # 主页面（包含HTML、CSS、JavaScript）
├── README.md       # 项目说明文档
└── images/         # 图片资源文件夹
```

## 🎨 设计风格

- **主色调**：珊瑚红 (#FF6B6B) + 薄荷绿 (#4ECDC4)
- **字体**：Playfair Display (标题) + Poppins (正文)
- **设计理念**：简洁、现代、温暖、友好

## 💡 注意事项

- 照片存储在浏览器的 LocalStorage 中，清除浏览器数据会丢失照片
- LocalStorage 容量有限（通常 5-10MB），不适合存储大量高清照片
- 建议定期下载重要照片到本地

## 📝 许可证

MIT License - 详见 LICENSE 文件

---

❤️ 用心设计，简单易用
