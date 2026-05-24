# 💖 比心手势识别 - Heart Gesture Detection

一个使用摄像头和机器学习的交互式网页，当你在摄像头前比心时，会在屏幕上渲染爱心动画！

## 特性

- 📷 **实时摄像头** - 访问你的摄像头并显示实时画面
- 👋 **手势识别** - 使用 Google MediaPipe Hands 进行高精度手势检测
- 💗 **爱心动画** - 检测到比心手势时，在手势位置生成彩色爱心动画
- 🎨 **美观设计** - 渐变紫色背景，圆角设计，响应式布局

## 如何使用

1. 在浏览器中打开项目
2. 允许浏览器访问你的摄像头
3. 等待模型加载完成
4. 在摄像头前用双手比出爱心形状（拇指和食指触碰形成爱心）
5. 系统会在手势位置生成彩色爱心动画！

## 技术栈

- **HTML5** - 页面结构
- **CSS3** - 样式设计
- **JavaScript** - 交互逻辑
- **MediaPipe Hands** - 手势识别模型
- **Canvas API** - 动画渲染

## 项目结构

```
/workspace/
├── index.html          # 主页面
├── README.md           # 项目说明
└── images/             # 图片资源
```

## 本地运行

1. 克隆项目
2. 在项目根目录启动本地服务器，例如：
   ```bash
   # 使用 Python
   python3 -m http.server 8000
   
   # 或使用 Node.js (http-server)
   npx http-server -p 8000
   ```
3. 在浏览器中访问 `http://localhost:8000`

## GitHub Pages 部署

这个项目可以使用 GitHub Pages 免费托管：

1. 确保项目已推送到 GitHub
2. 在 GitHub 仓库的 Settings -> Pages 中：
   - Source 选择 `Deploy from a branch`
   - Branch 选择 `main` 或 `master`
   - 点击 Save
3. 几分钟后，你就可以通过 `https://<your-username>.github.io/<repo-name>/` 访问了！

## 手势识别原理

系统通过检测双手关键点的相对位置来识别比心手势：
- 检测到两只手
- 两只手的拇指尖距离较近
- 两只手的食指尖距离较近
- 双手保持适当距离
- 其他手指并拢

## 许可证

MIT License
