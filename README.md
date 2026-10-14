# 蔡利莹 · 个人作品集网站

按 PPT《蔡利莹个人作品集.pptx》(34 页) 1:1 复刻的单文件作品集网站。

## 打开方式

### 方式 A：双击打开（最简单）
直接双击 `index.html`，浏览器会打开本地预览。

### 方式 B：本地服务器（推荐）
如果方式 A 字体加载有问题，在当前目录运行：

```bash
# Python 3
python3 -m http.server 8000

# Node.js
npx serve .
```

然后浏览器打开 `http://localhost:8000`

## 文件结构

```
portfolio-website/
├── index.html      # 单文件网站（含 HTML + CSS + JS）
└── README.md       # 本说明
```

## 设计说明

- **视觉系统**：完全沿用 PPT 配色（深蓝 #002FA7 + 暖黄 #F2CF5D）和编号系统
- **结构**：34 个 section，严格对应 PPT 一页
- **字体**：Noto Serif SC（标题）+ Noto Sans SC（正文）+ Inter（英文）
- **响应式**：375 / 768 / 1440 三档断点
- **动效**：滚动渐入 + 数据计数动画

## 图片占位

PPT 中的 15 张图片用浅灰底 + "图位 N - 描述" 占位。  
要替换成真实图片时：
1. 把图片放到 `images/` 目录（自己创建）
2. 把 `<div class="img-placeholder ...">图位 N</div>` 替换为 `<img src="images/xxx.jpg" />`

## 后续可优化方向

- [ ] 替换占位图为真实图片
- [ ] 部署到 CloudStudio / Vercel / Netlify
- [ ] 添加深色模式切换
- [ ] 增加更细的滚动动效
