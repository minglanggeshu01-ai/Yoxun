# 惠州市毅迅电子科技有限公司 — 企业官网（欧美现代风格）

**工贸一体锂电池制造商**全静态企业官网 · HTML5 + Tailwind CSS + Vanilla JS

> 🎨 **Design**: Dark & white palette · Gold accent · Inter font · Glass morphism · Bold typography

## 📁 文件结构

```
├── index.html          ← 首页（全屏Hero · 数据条 · 公司简介 · 产品线 · 合作客户 · CTA）
├── product.html        ← 产品中心（分类筛选 · 9款产品 · 点击弹窗详情）
├── case.html           ← 案例展示（4个国际项目 · 左右交替布局）
├── about.html          ← 关于我们（公司介绍 · 核心优势 · 工厂实景 · 认证资质）
├── contact.html        ← 在线留言（Formspree表单 · 联系信息卡片 · 微信二维码）
├── css/
│   └── style.css       ← 自定义样式（CSS变量 · 动画 · 组件 · 毛玻璃导航）
├── js/
│   └── main.js         ← 共享JS（轮播 · 筛选 · 弹窗 · 滚动动画 · 统计计数）
├── img/                ← 图片文件夹
└── README.md
```

## 🚀 快速启动

双击 `index.html` 直接浏览器打开，或本地服务器：

```bash
cd 项目文件夹
python -m http.server 8080
# 浏览器访问 http://localhost:8080
```

## 🎨 设计风格

| 元素 | 说明 |
|------|------|
| **配色** | 深黑 #0a0c10 + 纯白 + 金色点缀 #c6903f |
| **字体** | Inter (Google Fonts) + 系统后备字体 |
| **导航** | 毛玻璃效果 (backdrop-filter blur) |
| **卡片** | 深色/浅色卡片 + hover悬浮阴影 |
| **标题** | 超大粗体 (font-black) + 紧凑字距 |
| **动画** | 平滑过渡 · 统计数字滚动 · 渐显效果 |

## 🔧 一键替换指南

### 1. 公司信息（全局搜索替换）
搜索关键词 → 替换为你的信息：
- `+86 158 2656 0159` → 你的电话
- `minglanggeshu01@gmail.com` → 你的邮箱
- `广东省惠州市惠城区` → 你的地址
- `粤ICP备XXXXXXXX号-1` → 你的备案号

### 2. 图片替换（放入 `img/` 文件夹）
| 文件名 | 用途 | 建议尺寸 |
|--------|------|----------|
| `logo.png` | 网站Logo | 200×80 |
| `hero-bg.jpg` | 首页全屏Hero背景 | 1920×1080 |
| `about-factory.jpg` | 公司展示图 | 600×450 |
| `about-company.jpg` | 关于我们大图 | 600×450 |
| `product-*.jpg` | 产品图片（8张） | 600×400 |
| `case1.jpg` ~ `case4.jpg` | 案例图 | 800×500 |
| `factory1.jpg` ~ `factory6.jpg` | 工厂实景 | 600×400 |
| `partner1.png` ~ `partner6.png` | 客户Logo | 160×60 |
| `cert-*.png` | 认证证书 | 120×80 |
| `qrcode-wechat.jpg` | 微信二维码 | 200×200 |

### 3. Formspree 留言对接
1. 注册 [formspree.io](https://formspree.io)
2. 拿到 Form ID 后替换 `index.html` 和 `contact.html` 中的 `xxxxxxxx`
3. 免费版：50条/月

### 4. 产品数据
编辑 `product.html`，搜索 `【可修改】`，修改 `openModal()` 调用里的标题、规格、特性数组和图片。

### 5. 案例数据
编辑 `case.html`，搜索 `【可修改】`，修改案例标题、地区、描述和图片。

### 6. 换肤
编辑 `css/style.css` 中的 `:root` 变量：
```css
--dark: #0a0c10;          /* 主背景黑 */
--accent: #c6903f;        /* 强调金色 */
--radius: 12px;           /* 圆角 */
```

## ✨ 技术特性
- **纯静态** — 可部署到 GitHub Pages / Netlify / Vercel / 阿里云OSS
- **响应式** — Tailwind CSS breakpoints，手机/平板/电脑全适配
- **SEO** — 每页独立 meta title/description/keywords + alt标签
- **Formspree** — 无需后端即可接收留言到邮箱
- **注释清晰** — 所有可修改位置标注 `【可修改】` / `【可替换】`

## 📤 部署
| 平台 | 说明 |
|------|------|
| GitHub Pages | 免费，push即部署 |
| Netlify | 免费，拖拽文件夹 |
| Vercel | 免费，GitHub自动部署 |
| 阿里云OSS | 国内访问快，需备案 |

---

*代码中搜索 `【可修改】` 定位所有可自定义的文字、图片和配置项。*
