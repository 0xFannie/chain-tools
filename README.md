# Chain Tools - 区块链工具集合

<div align="center">

![Chain Tools](https://img.shields.io/badge/Chain-Tools-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-Active-success)

**专业、免费、开源的 Web3 开发和交互工具集合**

[访问网站](https://chain-tools.com) · [查看工具](#-可用工具) · [贡献代码](#-贡献)

</div>

---

## 🎯 项目简介

Chain Tools 是一个精心策划的区块链工具集合平台，旨在为 Web3 开发者和用户提供免费、开源、易用的工具。所有工具都注重安全性、易用性和现代化设计。

### ✨ 核心价值

- **🔓 完全免费** - 所有工具永久免费使用
- **🌐 开源透明** - 代码托管在 GitHub，可供审计
- **🛡️ 安全可靠** - 经过严格测试，注重安全
- **🎨 现代设计** - 美观易用的用户界面
- **⚡ 持续更新** - 定期添加新工具和功能

---

## 🛠️ 可用工具

### 1. MultiSig Wallet Deployer ✅

企业级多签名钱包管理系统，支持完整的多签交易流程。

**核心功能：**
- ✅ 完整的交易管理（提交、确认、撤销、执行）
- ✅ 支持多条区块链网络（Ethereum, Polygon, BSC, Arbitrum）
- ✅ 实时交易状态追踪和确认进度显示
- ✅ 现代化的用户界面
- ✅ 经过 14 个单元测试验证

**使用场景：**
- 🏢 公司资金管理 - 多个合伙人共同管理
- 🏛️ DAO 金库管理 - 理事会成员投票决策
- 👨‍👩‍👧‍👦 家庭资产管理 - 夫妻双方共同确认
- 🤝 项目资金托管 - 投资人和创始人双重保障

**技术栈：** Solidity 0.8.19, Next.js 13, TypeScript, Hardhat, Wagmi

**链接：**
- 🔗 [Live Demo](https://github.com/0xFannie/multisig-deployer)
- 📖 [完整文档](https://github.com/0xFannie/multisig-deployer#readme)
- 💻 [源代码](https://github.com/0xFannie/multisig-deployer)

---

### 2. 更多工具开发中... ⏳

我们正在开发更多实用的区块链工具，敬请期待！

**计划中的工具：**
- 💸 Token Batch Sender - 批量发送代币工具
- ⛽ Gas Tracker - 实时 Gas 费用追踪
- ✅ Contract Verifier - 智能合约一键验证
- 🖼️ NFT Minter - 简单易用的 NFT 铸造工具
- 🔍 Wallet Analyzer - 钱包资产分析工具
- 🔄 Token Swapper - 快速代币交换接口
- 📊 DAO Snapshot - DAO 投票和提案工具

---

## 🚀 快速开始

### 本地预览

这是一个简单的静态网站，可以直接在浏览器中打开：

```bash
# 克隆仓库
git clone https://github.com/0xFannie/chain-tools.git

# 进入目录
cd chain-tools

# 方式 1: 直接在浏览器中打开
# 打开 index.html 文件

# 方式 2: 使用 Python HTTP 服务器
python -m http.server 8000

# 方式 3: 使用 Node.js HTTP 服务器
npx http-server

# 方式 4: 使用 VS Code Live Server 扩展
# 右键 index.html → "Open with Live Server"
```

访问 `http://localhost:8000`

---

## 📦 部署指南

### Vercel 部署（推荐）⭐

**步骤：**

1. **准备 GitHub 仓库**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/chain-tools.git
   git push -u origin main
   ```

2. **连接 Vercel**
   - 访问 [vercel.com](https://vercel.com)
   - 使用 GitHub 账号登录
   - 点击 "Add New..." → "Project"
   - 选择 `chain-tools` 仓库
   - 点击 "Deploy"

3. **配置自定义域名**
   - 部署成功后，进入项目设置
   - 点击 "Domains"
   - 添加 `chain-tools.com`
   - 按照提示配置 DNS

**DNS 配置（在域名注册商）：**

```
类型: A
名称: @
值: 76.76.21.21

类型: CNAME
名称: www
值: cname.vercel-dns.com
```

**优势：**
- ✅ 自动 HTTPS
- ✅ 全球 CDN
- ✅ 自动部署（推送即部署）
- ✅ 免费套餐足够使用

---

### Netlify 部署

**步骤：**

1. 推送代码到 GitHub（同上）

2. **连接 Netlify**
   - 访问 [netlify.com](https://netlify.com)
   - 点击 "New site from Git"
   - 选择 GitHub 仓库
   - 点击 "Deploy site"

3. **配置域名**
   - 在 Netlify 设置中添加自定义域名
   - 配置 DNS

**DNS 配置：**

```
类型: A
名称: @
值: 75.2.60.5

类型: CNAME
名称: www
值: [your-site].netlify.app
```

---

### GitHub Pages 部署

**步骤：**

1. 推送代码到 GitHub

2. **启用 GitHub Pages**
   - 进入仓库设置 → Pages
   - Source: Deploy from a branch
   - Branch: main / root
   - Save

3. **配置自定义域名（可选）**
   - 在 Pages 设置中添加域名
   - 在仓库根目录创建 `CNAME` 文件，内容为你的域名

**DNS 配置：**

```
类型: A
名称: @
值: 185.199.108.153
值: 185.199.109.153
值: 185.199.110.153
值: 185.199.111.153

类型: CNAME
名称: www
值: YOUR_USERNAME.github.io
```

---

## 🎨 设计系统

### 配色方案

项目采用现代化的深色主题配色：

```css
primary-dark: #13172A   /* 深蓝黑 - 主要背景 */
primary-gray: #787E91   /* 灰蓝 - 次要文本 */
primary-light: #F8E3D6  /* 米色/桃色 - 强调色 */
primary-black: #05090E  /* 纯黑 - 深色背景 */
white: #FFFFFF          /* 纯白 - 主要文本 */
```

### 字体系统

- **主字体：** Poppins (300, 400, 500, 600, 700, 800)
- **代码字体：** Monospace
- **图标：** Lucide React / SVG Icons

### UI 特性

- ✨ 毛玻璃效果（Glassmorphism）
- 🎨 渐变按钮和文字
- 📱 完全响应式设计
- ⚡ 流畅的动画过渡
- 🎯 清晰的视觉层次

---

## 🔧 技术架构

### 前端技术栈

```
Landing Page (Static)
├── HTML5
├── Tailwind CSS (via CDN)
├── JavaScript (Vanilla)
└── Google Fonts (Poppins)

工具项目 (Next.js)
├── Next.js 13+
├── React 18+
├── TypeScript
├── Tailwind CSS
├── Wagmi (Web3)
└── Viem
```

### 部署架构

```
chain-tools.com                    # Landing Page (Vercel)
    ├── /                          # 主页
    ├── /tools                     # 工具列表（未来）
    └── /docs                      # 文档（未来）

子域名部署（可选）
├── multisig.chain-tools.com      # MultiSig Deployer
├── tools.chain-tools.com         # 其他工具
└── docs.chain-tools.com          # 文档中心
```

---

## 📚 项目结构

```
chain-tools/
├── index.html              # Landing Page 主页面
├── README.md               # 项目说明文档（本文件）
├── vercel.json             # Vercel 部署配置
├── .gitignore              # Git 忽略文件
└── LICENSE                 # MIT 许可证
```

---

## 🤝 贡献

我们欢迎所有形式的贡献！

### 如何贡献新工具

如果你有好的工具想法或已开发的工具：

1. **Fork 本仓库**
2. **创建新的工具项目**
   - 遵循现有的设计风格
   - 使用相同的配色方案
   - 提供完整的文档
3. **在 Landing Page 添加工具卡片**
   - 编辑 `index.html`
   - 复制现有工具卡片模板
   - 填写工具信息
4. **提交 Pull Request**

### 贡献指南

- ✅ 确保代码经过测试
- ✅ 遵循现有的设计风格和配色
- ✅ 提供清晰的文档和使用说明
- ✅ 工具必须开源且免费
- ✅ 注重安全性和用户隐私

### 工具开发建议

**技术要求：**
- 使用 Next.js + TypeScript（推荐）
- 集成 Wagmi 和 Viem（Web3 工具）
- 使用 Tailwind CSS 样式
- 完整的单元测试

**设计要求：**
- 响应式布局
- 使用项目配色方案
- Poppins 字体
- 现代化 UI 设计

---

## 📝 许可证

MIT License - 详见 [LICENSE](./LICENSE) 文件

---

## 👤 作者

**0xFannie.eth**

- GitHub: [@0xFannie](https://github.com/0xFannie)
- Website: [chain-tools.com](https://chain-tools.com)

---

## 💖 支持项目

如果这个项目对你有帮助：

- ⭐ 给项目一个 Star
- 🐛 报告 Bug 或提出建议
- 🔀 Fork 并贡献代码
- 📢 分享给更多人
- 💬 加入讨论和反馈

---

## 🔗 相关链接

### 工具项目
- [MultiSig Deployer](https://github.com/0xFannie/multisig-deployer) - 多签钱包管理工具

### 官方网站
- [Chain Tools](https://chain-tools.com) - 主站（即将上线）

### 文档和资源
- [部署指南](#-部署指南) - 如何部署到生产环境
- [设计系统](#-设计系统) - UI 设计规范
- [贡献指南](#-贡献) - 如何参与贡献

---

## 📊 项目路线图

### ✅ Phase 1: 基础设施（已完成）
- [x] Landing Page 设计和开发
- [x] 第一个工具：MultiSig Deployer
- [x] 项目文档和部署指南
- [x] Git 仓库和版本控制

### 🚧 Phase 2: 上线和推广（进行中）
- [ ] 部署到生产环境
- [ ] 配置自定义域名
- [ ] SEO 优化
- [ ] 在 Product Hunt 发布
- [ ] 社交媒体推广

### 📅 Phase 3: 扩展工具集（计划中）
- [ ] 开发 Token Batch Sender
- [ ] 开发 Gas Tracker
- [ ] 开发 Contract Verifier
- [ ] 建立用户反馈渠道
- [ ] 多语言支持

### 🔮 Phase 4: 社区建设（未来）
- [ ] 建立开发者社区
- [ ] 提供 API 服务
- [ ] 移动端适配优化
- [ ] 集成更多区块链网络

---

## ❓ 常见问题

### Q: 所有工具都是免费的吗？
A: 是的！所有工具永久免费使用，无需注册或付费。

### Q: 代码是开源的吗？
A: 是的，所有代码都在 GitHub 上开源，遵循 MIT 许可证。

### Q: 如何添加新工具到平台？
A: 请查看[贡献指南](#-贡献)，我们欢迎所有符合要求的工具。

### Q: 工具的安全性如何？
A: 所有工具都经过严格测试，代码开源可审计。我们建议在使用前先在测试网测试。

### Q: 支持哪些区块链网络？
A: 目前支持 Ethereum、Polygon、BSC、Arbitrum 等主流网络，未来会支持更多。

### Q: 如何报告 Bug 或提出建议？
A: 请在 GitHub Issues 中提交，我们会及时回复。

### Q: 可以用于商业项目吗？
A: 可以！MIT 许可证允许商业使用。

---

## 🎯 关于 Chain Tools

Chain Tools 诞生于一个简单的想法：**让区块链交互变得更简单、更安全、更易用**。

我们相信：
- 🌍 优秀的工具应该开源和免费
- 🔐 安全性和易用性同样重要
- 🤝 社区驱动才能走得更远
- 📈 持续改进胜过完美开始

加入我们，一起构建更好的 Web3 工具生态！

---

## 🙏 致谢

感谢所有使用、测试和贡献的开发者！

特别感谢：
- Next.js 和 Vercel 团队
- Tailwind CSS 团队
- Wagmi 和 Viem 团队
- 所有开源贡献者

---

<div align="center">

**0xFannie.eth Made with ❤️ for Web3 Community**

[⬆ 回到顶部](#chain-tools---区块链工具集合)

</div>
