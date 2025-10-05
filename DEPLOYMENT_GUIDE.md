# Chain Tools 部署指南

## 🚀 快速部署

本项目是一个静态网站，可以部署到任何静态托管服务。

---

## 方案 1: Vercel 部署（推荐）⭐

### 步骤

1. **准备 GitHub 仓库**
   ```bash
   cd d:/FannieKuku/chain-tools
   git init
   git add .
   git commit -m "Initial commit: Chain Tools landing page"
   ```

2. **推送到 GitHub**
   ```bash
   # 在 GitHub 创建新仓库 chain-tools
   git remote add origin https://github.com/0xFannie/chain-tools.git
   git branch -M main
   git push -u origin main
   ```

3. **连接 Vercel**
   - 访问 [vercel.com](https://vercel.com)
   - 点击 "Import Project"
   - 选择 GitHub 仓库 `chain-tools`
   - 点击 "Deploy"

4. **配置自定义域名**
   - 在 Vercel 项目设置中点击 "Domains"
   - 添加域名 `chain-tools.com`
   - 按照提示配置 DNS

### DNS 配置（在域名注册商）

```
A Record:
chain-tools.com → 76.76.21.21

CNAME Record:
www.chain-tools.com → cname.vercel-dns.com
```

### 自动部署

✅ 每次推送到 `main` 分支，Vercel 会自动部署

---

## 方案 2: Netlify 部署

### 步骤

1. **推送代码到 GitHub**（同上）

2. **连接 Netlify**
   - 访问 [netlify.com](https://netlify.com)
   - 点击 "New site from Git"
   - 选择 GitHub 仓库
   - 部署设置保持默认
   - 点击 "Deploy site"

3. **配置域名**
   - 在 Netlify 设置中添加自定义域名
   - 配置 DNS

### DNS 配置

```
A Record:
chain-tools.com → 75.2.60.5

CNAME Record:
www.chain-tools.com → [your-site].netlify.app
```

---

## 方案 3: GitHub Pages 部署

### 步骤

1. **推送代码到 GitHub**

2. **启用 GitHub Pages**
   - 进入仓库设置 → Pages
   - Source: Deploy from a branch
   - Branch: main / root
   - Save

3. **配置自定义域名**
   - 在 Pages 设置中添加 `chain-tools.com`
   - 创建 `CNAME` 文件

### DNS 配置

```
A Records:
chain-tools.com → 185.199.108.153
chain-tools.com → 185.199.109.153
chain-tools.com → 185.199.110.153
chain-tools.com → 185.199.111.153

CNAME Record:
www.chain-tools.com → 0xFannie.github.io
```

---

## 部署 MultiSig Deployer

### 选项 1: 子域名部署

1. **部署 MultiSig Deployer 到 Vercel**
   ```bash
   cd d:/FannieKuku/multisig-deployer
   vercel
   ```

2. **配置子域名**
   - 在 Vercel 添加域名 `multisig.chain-tools.com`
   
3. **DNS 设置**
   ```
   CNAME Record:
   multisig.chain-tools.com → [project].vercel.app
   ```

### 选项 2: 保持独立部署

MultiSig Deployer 可以保持独立部署，从 Landing Page 链接过去：

```
Landing Page: chain-tools.com
MultiSig Tool: [独立地址或GitHub Pages]
```

---

## 📋 部署检查清单

### 部署前

- [ ] 检查所有链接是否正确
- [ ] 测试响应式布局
- [ ] 优化图片和资源
- [ ] 检查 SEO 标签

### 部署后

- [ ] 测试网站访问
- [ ] 检查自定义域名
- [ ] 测试所有工具链接
- [ ] 配置 HTTPS（自动）
- [ ] 设置分析工具（可选）

---

## 🔧 维护和更新

### 添加新工具

1. 在 `index.html` 中添加新的工具卡片
2. 更新 `README.md`
3. 提交并推送到 GitHub
4. 自动部署完成

### 更新工具信息

编辑 `index.html` 中对应的工具卡片内容，推送即可。

---

## 🌐 CDN 和性能优化

### 已优化项

- ✅ 使用 CDN 加载 Tailwind CSS
- ✅ Google Fonts 预连接
- ✅ 最小化 JavaScript
- ✅ 优化图片（使用 SVG）

### 进一步优化（可选）

- 添加图片懒加载
- 使用 Cloudflare CDN
- 启用 HTTP/2
- 压缩资源文件

---

## 📊 监控和分析

### Google Analytics（可选）

在 `index.html` 的 `<head>` 中添加：

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🆘 故障排除

### 问题：域名未生效

- 等待 DNS 传播（最多 48 小时）
- 检查 DNS 配置是否正确
- 清除浏览器缓存

### 问题：HTTPS 未启用

- Vercel/Netlify 会自动配置 SSL
- 检查域名配置是否正确

### 问题：页面无法访问

- 检查部署状态
- 查看部署日志
- 确认文件路径正确

---

## 📞 支持

如有问题：
- 查看 [README](./README.md)
- 提交 [GitHub Issue](https://github.com/0xFannie/chain-tools/issues)
- 参考 Vercel/Netlify 文档

---

**下一步：**
1. ⏳ 推送代码到 GitHub
2. ⏳ 连接 Vercel
3. ⏳ 配置域名
4. ✅ 完成部署！

