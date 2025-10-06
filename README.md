# Chain Tools - 区块链工具集合 | Blockchain Tools Collection

<div align="center">

![Chain Tools](https://img.shields.io/badge/Chain-Tools-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-Active-success)

**专业、免费、开源的 Web3 开发和交互工具集合**

**Professional, Free, Open Source Web3 Development and Interaction Tools Collection**

[🌐 访问网站 Visit Website](https://chain-tools.com) · [🛠️ 查看工具 View Tools](#-可用工具--available-tools) · [🤝 贡献代码 Contribute](#-贡献--contributing)

</div>

---

## 📖 Language | 语言

- [🇨🇳 中文](#中文文档)
- [🇬🇧 English](#english-documentation)

---

<a name="中文文档"></a>

# 🇨🇳 中文文档

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
- ✅ 支持 14+ 条区块链网络（Ethereum, Polygon, BSC, Arbitrum, Optimism, Avalanche, Fantom, Base, Linea, zkSync Era, Scroll, Polygon zkEVM, Sepolia, Goerli）
- ✅ 实时交易状态追踪和确认进度显示
- ✅ 合约地址管理和历史记录
- ✅ 分享链接功能，方便多方协作
- ✅ 现代化的用户界面
- ✅ 经过 14 个单元测试验证

**使用场景：**
- 🏢 公司资金管理 - 多个合伙人共同管理
- 🏛️ DAO 金库管理 - 理事会成员投票决策
- 👨‍👩‍👧‍👦 家庭资产管理 - 夫妻双方共同确认
- 🤝 项目资金托管 - 投资人和创始人双重保障

**技术栈：** Solidity 0.8.19, Next.js 14, TypeScript, Hardhat, Wagmi v2

**在线访问：** https://multisig.chain-tools.com

---

### 2. Solana Private Key Recovery ✅

Solana 私钥恢复工具（第三方集成）

**功能说明：**
- 从大小写不匹配的助记词中恢复 Solana 钱包私钥
- 验证钱包地址和资产
- 导出正确的私钥

**在线访问：** https://address-recovery.joysteps.io/

⚠️ **注意：** 这是第三方工具集成，请谨慎使用并保管好您的私钥。

---

## 🚀 快速开始

### MultiSig Wallet Deployer 使用指南

1. **访问应用**
   ```
   https://multisig.chain-tools.com
   ```

2. **连接钱包**
   - 点击"连接钱包"按钮
   - 选择您的钱包（MetaMask, WalletConnect 等）
   - 选择目标网络

3. **部署多签钱包**
   - 切换到"部署新合约"标签
   - 输入所有者地址（至少 2 个）
   - 设置所需确认比例（如 50%, 67%, 100%）
   - 点击"部署合约"并确认交易

4. **分享给其他所有者**
   - 部署成功后，点击"分享给其他所有者"
   - 将链接发送给其他所有者

5. **管理交易**
   - 切换到"交易管理"标签
   - 提交新交易：输入接收地址和金额
   - 确认交易：查看待确认交易并签名
   - 执行交易：达到所需确认数后执行

---

## 🔧 本地开发

### Prerequisites 前置要求

- Node.js 16+
- npm 或 yarn
- Git

### MultiSig Deployer 本地运行

```bash
# 克隆仓库
git clone https://github.com/0xFannie/multisig-deployer.git
cd multisig-deployer

# 安装依赖
npm install

# 配置环境变量
cp .env.example .env.local
# 编辑 .env.local 填入您的配置

# 启动开发服务器
npm run dev

# 访问 http://localhost:3000
```

### 运行测试

```bash
# 运行智能合约测试
npx hardhat test

# 查看测试覆盖率
npx hardhat coverage
```

---

## 📚 技术架构

### MultiSig Wallet Deployer

**前端技术栈：**
- Next.js 14 - React 框架
- TypeScript - 类型安全
- Tailwind CSS - 样式框架
- Wagmi v2 - Web3 React Hooks
- Viem - 以太坊交互库

**智能合约：**
- Solidity 0.8.19
- Hardhat - 开发环境
- OpenZeppelin - 安全库

**支持的网络：**
- Layer 1 主网：Ethereum, Polygon PoS, BNB Chain, Avalanche, Fantom
- Layer 2：Arbitrum One, Optimism, Base
- zkEVM：zkSync Era, Scroll, Polygon zkEVM, Linea
- 测试网：Sepolia, Goerli

---

## 👤 作者

**0xfannie.eth**

- 🔗 GitHub: [@0xFannie](https://github.com/0xFannie)
- 🌐 Website: [xifangzhang.work](https://xifangzhang.work)
- 💼 Public Wallets:
  - **0xfannie.eth** (EVM): `0x36C1ad1E9eB589E20fF739FAD024a7ff3113Ba27`
  - **Catalizer.eth** (EVM): `0xF9147fb1c9799fA61bC9a41B28FFf2EE80654fd5`
  - **fannie.sol** (Solana): `4SUKuF4jt2ya6No5okHGvk5tsezAZaf3bVHvCf1pNqrC`

---

## 🤝 贡献

我们欢迎任何形式的贡献！

### 如何贡献

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

### 贡献指南

- 遵循现有代码风格
- 添加适当的测试
- 更新相关文档
- 确保所有测试通过

---

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

---

## 🔗 相关链接

### 工具项目
- [MultiSig Deployer](https://github.com/0xFannie/multisig-deployer) - 多签钱包管理工具
- [Solana Private Key Recovery](https://address-recovery.joysteps.io/) - Solana 私钥导出工具（第三方集成）

### 官方网站
- [Chain Tools](https://chain-tools.com) - 主站

---

## 💬 联系方式

- GitHub Issues: [提交问题](https://github.com/0xFannie/chain-tools/issues)
- Twitter: [@0xFannie](https://twitter.com/0xFannie)
- Website: [xifangzhang.work](https://xifangzhang.work)

---

## 🙏 致谢

感谢所有为这个项目做出贡献的开发者和用户！

特别感谢：
- OpenZeppelin - 智能合约安全库
- Wagmi Team - 优秀的 React Hooks 库
- Next.js Team - 强大的 React 框架

---

## ⚠️ 免责声明

请注意：
- 使用前请充分测试
- 本工具不提供任何形式的担保
- 使用者需自行承担使用风险
- 请妥善保管您的私钥和助记词
- 建议在测试网络先进行测试

---

<div align="center">

**0xfannie.eth Made with ❤️ for Web3 Community**

[⬆ 返回顶部](#chain-tools---区块链工具集合--blockchain-tools-collection)

</div>

---
---
---

<a name="english-documentation"></a>

# 🇬🇧 English Documentation

## 🎯 Project Overview

Chain Tools is a curated blockchain tools collection platform designed to provide free, open-source, and easy-to-use tools for Web3 developers and users. All tools prioritize security, usability, and modern design.

### ✨ Core Values

- **🔓 Completely Free** - All tools are permanently free to use
- **🌐 Open & Transparent** - Code hosted on GitHub for auditing
- **🛡️ Secure & Reliable** - Rigorously tested with security focus
- **🎨 Modern Design** - Beautiful and user-friendly interfaces
- **⚡ Continuous Updates** - Regular addition of new tools and features

---

## 🛠️ Available Tools

### 1. MultiSig Wallet Deployer ✅

Enterprise-grade multi-signature wallet management system supporting complete multi-sig transaction workflows.

**Core Features:**
- ✅ Complete transaction management (submit, confirm, revoke, execute)
- ✅ Support for 14+ blockchain networks (Ethereum, Polygon, BSC, Arbitrum, Optimism, Avalanche, Fantom, Base, Linea, zkSync Era, Scroll, Polygon zkEVM, Sepolia, Goerli)
- ✅ Real-time transaction status tracking and confirmation progress display
- ✅ Contract address management and history
- ✅ Shareable links for multi-party collaboration
- ✅ Modern user interface
- ✅ Verified by 14 unit tests

**Use Cases:**
- 🏢 Corporate Treasury - Multi-partner fund management
- 🏛️ DAO Treasury - Council member voting decisions
- 👨‍👩‍👧‍👦 Family Asset Management - Joint confirmation by both spouses
- 🤝 Project Fund Escrow - Dual guarantee for investors and founders

**Tech Stack:** Solidity 0.8.19, Next.js 14, TypeScript, Hardhat, Wagmi v2

**Live Demo:** https://multisig.chain-tools.com

---

### 2. Solana Private Key Recovery ✅

Solana Private Key Recovery Tool (Third-party Integration)

**Features:**
- Recover Solana wallet private keys from case-mismatched mnemonics
- Verify wallet addresses and assets
- Export correct private keys

**Live Demo:** https://address-recovery.joysteps.io/

⚠️ **Note:** This is a third-party tool integration. Please use cautiously and protect your private keys.

---

## 🚀 Quick Start

### MultiSig Wallet Deployer Usage Guide

1. **Access the Application**
   ```
   https://multisig.chain-tools.com
   ```

2. **Connect Wallet**
   - Click "Connect Wallet" button
   - Select your wallet (MetaMask, WalletConnect, etc.)
   - Choose target network

3. **Deploy MultiSig Wallet**
   - Switch to "Deploy New Contract" tab
   - Enter owner addresses (minimum 2)
   - Set required confirmation ratio (e.g., 50%, 67%, 100%)
   - Click "Deploy Contract" and confirm transaction

4. **Share with Other Owners**
   - After successful deployment, click "Share with Other Owners"
   - Send the link to other owners

5. **Manage Transactions**
   - Switch to "Transaction Management" tab
   - Submit new transaction: Enter recipient address and amount
   - Confirm transaction: View pending transactions and sign
   - Execute transaction: Execute after required confirmations reached

---

## 🔧 Local Development

### Prerequisites

- Node.js 16+
- npm or yarn
- Git

### Running MultiSig Deployer Locally

```bash
# Clone repository
git clone https://github.com/0xFannie/multisig-deployer.git
cd multisig-deployer

# Install dependencies
npm install

# Configure environment variables
cp .env.example .env.local
# Edit .env.local with your configuration

# Start development server
npm run dev

# Visit http://localhost:3000
```

### Running Tests

```bash
# Run smart contract tests
npx hardhat test

# View test coverage
npx hardhat coverage
```

---

## 📚 Technical Architecture

### MultiSig Wallet Deployer

**Frontend Stack:**
- Next.js 14 - React Framework
- TypeScript - Type Safety
- Tailwind CSS - Styling Framework
- Wagmi v2 - Web3 React Hooks
- Viem - Ethereum Interaction Library

**Smart Contracts:**
- Solidity 0.8.19
- Hardhat - Development Environment
- OpenZeppelin - Security Libraries

**Supported Networks:**
- Layer 1 Mainnets: Ethereum, Polygon PoS, BNB Chain, Avalanche, Fantom
- Layer 2: Arbitrum One, Optimism, Base
- zkEVM: zkSync Era, Scroll, Polygon zkEVM, Linea
- Testnets: Sepolia, Goerli

---

## 👤 Author

**0xfannie.eth**

- 🔗 GitHub: [@0xFannie](https://github.com/0xFannie)
- 🌐 Website: [xifangzhang.work](https://xifangzhang.work)
- 💼 Public Wallets:
  - **0xfannie.eth** (EVM): `0x36C1ad1E9eB589E20fF739FAD024a7ff3113Ba27`
  - **Catalizer.eth** (EVM): `0xF9147fb1c9799fA61bC9a41B28FFf2EE80654fd5`
  - **fannie.sol** (Solana): `4SUKuF4jt2ya6No5okHGvk5tsezAZaf3bVHvCf1pNqrC`

---

## 🤝 Contributing

We welcome contributions of all kinds!

### How to Contribute

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribution Guidelines

- Follow existing code style
- Add appropriate tests
- Update relevant documentation
- Ensure all tests pass

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

---

## 🔗 Related Links

### Tool Projects
- [MultiSig Deployer](https://github.com/0xFannie/multisig-deployer) - Multi-signature Wallet Management Tool
- [Solana Private Key Recovery](https://address-recovery.joysteps.io/) - Solana Private Key Export Tool (Third-party Integration)

### Official Website
- [Chain Tools](https://chain-tools.com) - Main Site

---

## 💬 Contact

- GitHub Issues: [Submit Issue](https://github.com/0xFannie/chain-tools/issues)
- Twitter: [@0xFannie](https://twitter.com/0xFannie)
- Website: [xifangzhang.work](https://xifangzhang.work)

---

## 🙏 Acknowledgments

Thanks to all developers and users who have contributed to this project!

Special Thanks to:
- OpenZeppelin - Smart Contract Security Libraries
- Wagmi Team - Excellent React Hooks Library
- Next.js Team - Powerful React Framework

---

## ⚠️ Disclaimer

Please note:
- Test thoroughly before use
- This tool provides no warranties of any kind
- Users assume all risks of use
- Keep your private keys and mnemonics secure
- Recommend testing on testnet first

---

<div align="center">

**0xfannie.eth Made with ❤️ for Web3 Community**

[⬆ Back to Top](#chain-tools---区块链工具集合--blockchain-tools-collection)

</div>
