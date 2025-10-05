# Chain Tools 快速启动指南

## 🎉 恭喜！项目已准备就绪

你现在拥有一个完整的 Chain Tools landing page，所有文件已创建完毕并提交到本地 Git 仓库。

---

## ✅ 已完成的工作

1. ✅ 创建了现代化的 Landing Page (`index.html`)
2. ✅ 编写了完整的 README 文档
3. ✅ 配置了部署文件 (Vercel, .gitignore)
4. ✅ 初始化了 Git 仓库并完成首次提交
5. ✅ 创建了详细的部署指南

---

## 🚀 接下来的3个步骤

### 步骤 1: 在 GitHub 创建仓库

1. 访问 [GitHub](https://github.com/new)
2. 仓库名称：`chain-tools`
3. 描述：`Free and open-source blockchain tools collection`
4. 选择 `Public`
5. **不要**初始化 README、.gitignore 或 license
6. 点击 "Create repository"

### 步骤 2: 推送代码到 GitHub

在命令行执行：

```bash
cd D:\FannieKuku\chain-tools

# 添加远程仓库
git remote add origin https://github.com/0xFannie/chain-tools.git

# 重命名分支为 main
git branch -M main

# 推送代码
git push -u origin main
```

### 步骤 3: 部署到 Vercel

1. **访问 Vercel**
   - 打开 [vercel.com](https://vercel.com)
   - 使用 GitHub 账号登录

2. **导入项目**
   - 点击 "Add New..." → "Project"
   - 选择 `chain-tools` 仓库
   - 点击 "Import"

3. **配置项目**
   - Project Name: `chain-tools`
   - Framework Preset: `Other`
   - Root Directory: `./`
   - 其他设置保持默认
   - 点击 "Deploy"

4. **配置自定义域名**
   - 部署成功后，进入项目设置
   - 点击 "Domains"
   - 添加 `chain-tools.com`
   - 按照提示配置 DNS

---

## 🌐 DNS 配置

在你的域名注册商（如 Namecheap, GoDaddy）添加以下记录：

### Vercel DNS 配置

```
类型: A
名称: @
值: 76.76.21.21
TTL: 自动

类型: CNAME
名称: www
值: cname.vercel-dns.com
TTL: 自动
```

⏱️ DNS 生效需要几分钟到48小时不等

---

## 📱 预览 Landing Page

在浏览器中打开本地文件：

```
D:\FannieKuku\chain-tools\index.html
```

或者启动本地服务器：

```bash
# 使用 Python
python -m http.server 8000

# 使用 Node.js
npx http-server

# 使用 VS Code Live Server 扩展
```

然后访问 `http://localhost:8000`

---

## 🔗 部署 MultiSig Deployer

### 选项 A: 使用子域名（推荐）

1. **部署 MultiSig Deployer**
   ```bash
   cd D:\FannieKuku\multisig-deployer
   vercel
   ```

2. **在 Vercel 添加自定义域名**
   - 进入 multisig-deployer 项目设置
   - 添加域名 `multisig.chain-tools.com`

3. **配置 DNS**
   ```
   类型: CNAME
   名称: multisig
   值: [你的项目].vercel.app
   ```

### 选项 B: 保持独立

MultiSig Deployer 可以保持独立部署，用户通过 Landing Page 链接访问。

---

## 📋 验证清单

部署完成后，检查以下项目：

- [ ] Landing page 可以访问
- [ ] 自定义域名已生效
- [ ] HTTPS 已启用（Vercel 自动配置）
- [ ] 所有链接正常工作
- [ ] MultiSig Deployer 链接正确
- [ ] GitHub 仓库已公开
- [ ] README 显示正常
- [ ] 响应式布局在手机上正常

---

## 🎨 自定义 Landing Page

### 添加新工具

在 `index.html` 中找到工具卡片部分，复制现有的工具卡片代码并修改：

```html
<div class="glass-card rounded-3xl p-8 md:p-10">
    <!-- 工具信息 -->
    <h3>工具名称</h3>
    <p>工具描述</p>
    <!-- ... -->
</div>
```

### 修改配色

在 `index.html` 的 `<script>` 标签中修改：

```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                primary: {
                    dark: '#13172A',  // 修改这里
                    gray: '#787E91',
                    light: '#F8E3D6',
                    black: '#05090E',
                }
            }
        }
    }
}
```

### 修改内容

直接编辑 `index.html`，所有文本和内容都在这个文件中。

---

## 📊 添加分析（可选）

### Google Analytics

1. 创建 GA4 账号
2. 获取跟踪 ID
3. 在 `index.html` 的 `<head>` 中添加跟踪代码

### Vercel Analytics

在 Vercel 项目设置中一键启用（免费）。

---

## 🔄 更新网站

修改文件后：

```bash
git add .
git commit -m "Update landing page"
git push
```

Vercel 会自动部署更新！✨

---

## 🆘 常见问题

### Q: 域名没有生效？
**A:** DNS 传播需要时间，最多48小时。可以用 [DNS Checker](https://dnschecker.org) 检查状态。

### Q: 如何更新 MultiSig Deployer 链接？
**A:** 编辑 `index.html`，找到对应的 `<a>` 标签修改 `href` 属性。

### Q: 可以添加自己的分析工具吗？
**A:** 可以！在 `<head>` 中添加任何第三方脚本。

### Q: 如何添加更多工具？
**A:** 复制现有工具卡片的 HTML 代码，修改内容即可。

---

## 📞 需要帮助？

- 📖 查看 [DEPLOYMENT_GUIDE.md](./DEPLOYMENT_GUIDE.md)
- 🐛 提交 [GitHub Issue](https://github.com/0xFannie/chain-tools/issues)
- 💬 查看 Vercel 文档

---

## 🎯 后续计划

- [ ] 完善 SEO 优化
- [ ] 添加更多工具
- [ ] 创建工具使用教程
- [ ] 建立社区
- [ ] 收集用户反馈

---

## 🎉 现在就开始吧！

执行上面的3个步骤，你的 Chain Tools 网站就可以上线了！

**祝你好运！** 🚀

---

<div align="center">

Made with ❤️ by 0xFannie.eth

</div>

