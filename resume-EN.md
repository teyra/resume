# Web3 front-end engineer

## Personal information

- **Name**: toby yan

- **Contact**: tobyyan865@gmail.com

- **GitHub**: https://github.com/teyra

- **Work experience**: 7 years

## Professional skills

### Web3 technology stack

- Proficient in Ethereum ecosystem and related tools (web3.js, ethers.js, Hardhat)

- Familiar with mainstream smart contract interaction modes (ERC-20, ERC-721, ERC-1155)

- Master solidity smart contract

- Experience in DApp development such as DeFi, GameFi, NFT

- Familiar with wallet integration such as WalletConnect, MetaMask

- Understand decentralized storage/indexing solutions such as IPFS and The Graph

- Understand the contract interaction process of Uniswap V2/V3 and be able to implement basic token exchange functions

- Use Uniswap SDK or official API to obtain token price and liquidity data
- Use Etherscan verifies the contract and analyzes the reasons for transaction failure

### Front-end technology

- Proficient in React.js/Next.js, Vue.js, vite framework and ecology;

- Familiar with TypeScript and modern JavaScript (ES6+)

- Proficient in using TailwindCSS, Styled-components and other CSS solutions
- Experience in using Wagmi RainbowKit front-end library
- Experience in audio and video development, proficient in WebRTC, WebCodecs and SRS streaming media servers, with audio and video encoding and decoding and performance optimization capabilities
- Full-stack development capabilities, proficient in Node.js, Nest.js and MongoDB

## Project experience

### Parallel World Game

[Project link](https://github.com/teyra/parallel-world-game)

#### Project description

Parallel World Game is a Web3 based The decentralized application (DApp) based on Chainlink technology integrates wallet connection, user authentication, smart contract interaction, and gamification functions (such as card drawing games). The project realizes the interaction between on-chain and off-chain data through Chainlink Functions, and supports NFT casting through ERC-721 contracts to reward users. The backend service is built on Nest.js and provides API services for JWT authentication and card drawing score records.

#### Technology stack

- **Front-end**: React.js, Next.js, TypeScript, TailwindCSS, Wagmi, RainbowKit, Axios

- **Back-end**: Nest.js, JWT, Passport.js, Swagger, TypeScript, MongoDB

- **Smart contracts**: Solidity, ERC-721, Chainlink Functions, Hardhat

- **Toolchain**: Ethers.js, dotenv, bcrypt

#### Function implementation

##### Front-end

- Implement wallet connection function, support mainstream wallets such as MetaMask, use wagmi and RainbowKit to provide wallet signature and disconnection functions.

- Develop a card drawing game module, support users to participate in card drawing after logging in through the wallet, randomly generate cards and calculate points.

- Use axios to encapsulate HTTP request module, support common methods such as GET, POST, PUT, DELETE, and integrate request and response interceptors.
- Provide user-friendly prompt information, such as wallet not connected, signature failed, card draw times exhausted, etc.
- Use the readContract method to read on-chain data (such as user score and NFT casting status) from the contract.
- Use the writeContract method to call the mintNFT method of the contract to cast NFT according to the user score.

##### Backend

- Use `@nestjs/jwt` to implement the user login function based on wallet signature and generate a short-term valid JWT Token.
- Implement JWT authentication through `passport-jwt` to protect restricted interfaces and ensure that only authenticated users can access.
- Design and implement a card draw score record module to support users to submit scores and query history records.
- Use MongoDB to persist user data and score records.
- Integrate `@nestjs/swagger` to automatically generate interface documents, support online debugging and rapid development.

##### Smart Contract

- Write a custom ERC-721 contract to support the casting and distribution of NFTs.
- Use Chainlink Functions to implement the interaction between on-chain and off-chain data, and query user score data in real time.
- Provide `mintNFT` method to dynamically mint NFTs based on user scores and issue them to users.

#### Achievements

- Successfully launched a fully functional Web3 DApp that supports wallet connection, smart contract interaction, and gamification functions.
- Provides complete backend services to support user login authentication and card draw score recording functions.
- The contract side implements on-chain and off-chain data interaction, and mints NFTs to reward users through the ERC-721 standard.
- The project architecture is clear and easy to expand, laying a good foundation for subsequent function development.

### Dragon Yield - Decentralized Yield Aggregation Platform

[Project Link](https://github.com/teyra/dragon-yield)

#### Project Description

Dragon Yield is a decentralized yield aggregation platform based on Web3 technology, aiming to provide users with efficient and secure staking, exchange and yield management functions. The project integrates mainstream DeFi protocols such as Uniswap and Chainlink, supports staking and exchange of multiple tokens, and improves user experience through real-time data updates and user-friendly interface.

#### Project Responsibilities

##### Core Function Development

- Implement token staking and unstaking functions, support staking of multiple tokens

- Integrate Chainlink Data Feeds to obtain token prices in real time and calculate exchange ratios

- Use Uniswap Router to implement token exchange functions, support users to quickly switch between different tokens

##### Front-end Development

- Use Next.js and React to build a high-performance front-end interface

- Integrate RainbowKit and wagmi to achieve wallet connection and user identity management

- Use TailwindCSS to optimize interface design and improve user experience

##### Smart Contract Interaction

- Use @wagmi/core and viem to interact with smart contracts to complete staking, unstaking and reward collection functions

- Integrate Uniswap SDK and call Router contract to complete token exchange
- Realize real-time display of the total locked volume (TVL) of the staking pool and user income

##### Data Management

- Use @tanstack/react-query Manage asynchronous data requests and optimize data loading performance
- Integrate urql to query Uniswap's trading pairs and liquidity data through GraphQL

##### Optimization and debugging

- Use eslint and typescript to improve code quality and ensure project maintainability
- Provide multi-wallet support through RainbowKit, compatible with mainstream wallets such as MetaMask and WalletConnect

## Technology stack

| Category | Technical tools |
| ------------ | ------------------------------------- |
| Front-end framework | Next.js, React |
| Style tools | TailwindCSS |
| Web3 tools | RainbowKit, wagmi, @uniswap/sdk, viem |
| Data management | @tanstack/react-query, urql |
| Smart contract interaction | Chainlink Data Feeds, Uniswap Router |
| Development tools | TypeScript, ESLint |

#### Project highlights

##### Real-time price updates

- Integrate Chainlink Data Feeds to get real-time ETH/USD and other token prices
- Ensure the accuracy of the exchange ratio

##### Multi-function staking system

- Support users to stake multiple tokens
- Real-time display of staking balance, cumulative income and total locked volume (TVL)
- Provide reward token distribution function, users can collect income at any time

##### Decentralized token exchange

- Use Uniswap Router to realize token exchange
- Support fast switching of multiple token pairs
- Dynamically calculate the exchange ratio to ensure that users get the best exchange price

##### User-friendly interface

- Use RainbowKit to provide multi-wallet support
- The interface design is simple and intuitive, supporting real-time data updates and interactions

##### High scalability

- Use GraphQL to query Uniswap data and support the expansion of more DeFi protocols in the future
- Modular design facilitates subsequent function iteration and maintenance

## Education background

Undergraduate | Hunan University of Arts and Sciences | Communication Engineering | 2015-2019

- Blockchain related courses: Cryptography Basics, Distributed Systems

## Certificates and Achievements

- [Blockchain Fundamentals Certification] - [chainlink] - [2025]

- [Hackathon Award or other achievements]

## Open Source Contributions

- typegoose: Optimize Schema validation logic (PR #827)

## Other information

- Community Certification: Chainlink Builders Program 2025

- Language proficiency: English technical document reading and writing (TOEFL 105), can participate in English technical conferences
