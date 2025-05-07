# Web3 前端工程师

## 个人信息

- **姓名**: toby yan
- **联系方式**: tobyyan865@gmail.com
- **GitHub**: https://github.com/teyra
- **工作经验**: 7 年

## 专业技能

### Web3 技术栈

- 精通 Ethereum 生态及相关工具 (web3.js, ethers.js, Hardhat)
- 熟悉主流智能合约交互模式 (ERC-20, ERC-721, ERC-1155)
- 掌握 solidity smart contract
- 有 DeFi,GameFi, NFT 等 DApp 开发经验
- 熟悉 WalletConnect, MetaMask 等钱包集成
- 了解 IPFS, The Graph 等去中心化存储/索引方案
- 了解 Uniswap V2/V3 的合约交互流程，能实现基础代币兑换功能
- 使用 Uniswap SDK 或官方 API 获取代币价格和流动性数据
- 使用 Etherscan 验证合约并分析交易失败原因

### 前端技术

- 精通 React.js/Next.js,Vue.js,vite 框架及生态;
- 熟悉 TypeScript 和现代 JavaScript (ES6+)
- 熟练使用 TailwindCSS, Styled-components 等 CSS 方案
- 有 Wagmi RainbowKit 前端库使用经验
- 有音视频开发经验，精通 WebRTC、WebCodecs 和 SRS 流媒体服务器，具备音视频编解码和性能优化能力
- 全栈开发能力，熟练掌握 Node.js、Nest.js 和 MongoDB

## 项目经验

### Parallel World Game

[项目链接](https://github.com/teyra/parallel-world-game)

#### 项目描述

Parallel World Game 是一个基于 Web3 技术的去中心化应用（DApp），集成了钱包连接、用户鉴权、智能合约交互以及游戏化功能（如抽卡游戏）。项目通过 Chainlink Functions 实现了链上与链下数据的交互，支持通过 ERC-721 合约铸造 NFT 奖励用户。后端服务基于 Nest.js 构建，提供了 JWT 鉴权和抽卡得分记录的 API 服务。

#### 技术栈

- **前端**: React.js、Next.js、TypeScript、TailwindCSS、Wagmi、RainbowKit、Axios
- **后端**: Nest.js、JWT、Passport.js、Swagger、TypeScript、MongoDB
- **智能合约**: Solidity、ERC-721、Chainlink Functions、Hardhat
- **工具链**: Ethers.js、dotenv、bcrypt

#### 实现功能

##### 前端

- 实现钱包连接功能，支持 MetaMask 等主流钱包，使用 wagmi 和 RainbowKit 提供钱包签名和断开连接功能。
- 开发抽卡游戏模块，支持用户通过钱包登录后参与抽卡，随机生成卡片并计算点数。
- 使用 axios 封装 HTTP 请求模块，支持 GET、POST、PUT、DELETE 等常用方法，并集成请求和响应拦截器。
- 提供用户友好的提示信息，如钱包未连接、签名失败、抽卡次数用尽等。
- 使用 readContract 方法从合约中读取链上数据（如用户得分和 NFT 铸造状态）。
- 使用 writeContract 方法调用合约的 mintNFT 方法，根据用户得分铸造 NFT。

##### 后端

- 使用 `@nestjs/jwt` 实现基于钱包签名的用户登录功能，生成短期有效的 JWT Token。
- 通过 `passport-jwt` 实现 JWT 鉴权，保护受限接口，确保只有经过身份验证的用户才能访问。
- 设计并实现抽卡得分记录模块，支持用户提交得分并查询历史记录。
- 使用 MongoDB 持久化存储用户数据和得分记录。
- 集成 `@nestjs/swagger`，自动生成接口文档，支持在线调试和快速开发。

##### 智能合约

- 编写自定义 ERC-721 合约，支持 NFT 的铸造和分发。
- 使用 Chainlink Functions 实现链上与链下数据的交互，实时查询用户得分数据。
- 提供 `mintNFT` 方法，根据用户得分情况动态铸造 NFT 并颁发给用户。

#### 成果

- 成功上线了一个功能完善的 Web3 DApp，支持钱包连接、智能合约交互和游戏化功能。
- 提供了完整的后端服务，支持用户登录鉴权和抽卡得分记录功能。
- 合约端实现了链上与链下数据交互，并通过 ERC-721 标准铸造 NFT 奖励用户。
- 项目架构清晰，易于扩展，为后续功能开发奠定了良好的基础。

### Dragon Yield - 去中心化收益聚合平台

[项目链接](https://github.com/teyra/dragon-yield)

#### 项目描述

Dragon Yield 是一个基于 Web3 技术的去中心化收益聚合平台，旨在为用户提供高效、安全的质押、兑换和收益管理功能。项目集成了 Uniswap 和 Chainlink 等主流 DeFi 协议，支持多种代币的质押与兑换，并通过实时数据更新和用户友好的界面提升用户体验。

#### 项目职责

##### 核心功能开发

- 实现代币质押与解押功能，支持多种代币的质押
- 集成 Chainlink Data Feeds，实时获取代币价格并计算兑换比例
- 使用 Uniswap Router 实现代币兑换功能，支持用户在不同代币之间快速切换

##### 前端开发

- 使用 Next.js 和 React 构建高性能的前端界面
- 集成 RainbowKit 和 wagmi，实现钱包连接和用户身份管理
- 使用 TailwindCSS 优化界面设计，提升用户体验

##### 智能合约交互

- 使用 @wagmi/core 和 viem 与智能合约交互，完成质押、解押和奖励领取功能
- 集成 Uniswap SDK，调用 Router 合约完成代币兑换
- 实现质押池的总锁仓量（TVL）和用户收益的实时展示

##### 数据管理

- 使用 @tanstack/react-query 管理异步数据请求，优化数据加载性能
- 集成 urql，通过 GraphQL 查询 Uniswap 的交易对和流动性数据

##### 优化与调试

- 使用 eslint 和 typescript 提高代码质量，确保项目的可维护性
- 通过 RainbowKit 提供多钱包支持，兼容 MetaMask、WalletConnect 等主流钱包

## 技术栈

| 类别         | 技术工具                              |
| ------------ | ------------------------------------- |
| 前端框架     | Next.js、React                        |
| 样式工具     | TailwindCSS                           |
| Web3 工具    | RainbowKit、wagmi、@uniswap/sdk、viem |
| 数据管理     | @tanstack/react-query、urql           |
| 智能合约交互 | Chainlink Data Feeds、Uniswap Router  |
| 开发工具     | TypeScript、ESLint                    |

#### 项目亮点

##### 实时价格更新

- 集成 Chainlink Data Feeds，实时获取 ETH/USD 和其他代币价格
- 确保兑换比例的准确性

##### 多功能质押系统

- 支持用户质押多种代币
- 实时显示质押余额、累计收益和总锁仓量（TVL）
- 提供奖励代币分发功能，用户可随时领取收益

##### 去中心化代币兑换

- 使用 Uniswap Router 实现代币兑换
- 支持多种代币对的快速切换
- 动态计算兑换比例，确保用户获得最佳兑换价格

##### 用户友好界面

- 使用 RainbowKit 提供多钱包支持
- 界面设计简洁直观，支持实时数据更新和交互

##### 高扩展性

- 使用 GraphQL 查询 Uniswap 数据，支持未来扩展更多 DeFi 协议
- 模块化设计，便于后续功能迭代和维护

## 教育背景

本科 | 湖南文理学院 | 通信工程 | 2015-2019

- 区块链相关课程：密码学基础、分布式系统

## 证书与成就

- [Blockchain Fundamentals Certification] - [chainlink] - [2025]
- [黑客松获奖或其他成就]

## 开源贡献

- typegoose：优化 Schema 验证逻辑（PR #827）

## 其他信息

- 社区认证：Chainlink Builders Program 2025
- 语言能力：英文技术文档读写（TOEFL 105），可参与英文技术会议
