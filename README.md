# 北京岩馆速查 · H5

> 北京 34 家室内攀岩馆速查地图 · 8 大城区 · v5.5

## 📦 项目结构

```
.
├── index.html      # 主页面（含全部 CSS/JS）
├── data.json       # 34 家岩馆数据
├── vercel.json     # Vercel 部署配置
└── README.md       # 本文件
```

## 🚀 部署到 Vercel

### 方式 A：网页拖拽上传（推荐新手）

1. 登录 https://vercel.com/new
2. 把整个文件夹（或解压后的 zip 内容）拖到上传区
3. 点击 **Deploy**，30 秒后获得网址

### 方式 B：CLI 部署（需 Node.js 环境）

```bash
npm i -g vercel
cd climbing-h5-deploy
vercel
```

## 🛠️ 本地预览

由于 `index.html` 通过 `fetch('./data.json')` 加载数据，必须在 HTTP 服务器下打开（直接双击会因 CORS 失败）：

```bash
# 任选一种
python3 -m http.server 8000
# 或
npx serve .
```

然后浏览器访问 http://localhost:8000

## ✏️ 更新数据

改 `data.json` 里的店铺信息，重新 push / 上传，Vercel 会自动重新部署。

## 📱 移动端优先

页面针对 iPhone Safari / 微信内置浏览器优化，建议在手机上访问。
