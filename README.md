# Ethereum Stack

💎 Ethereum infrastructure, contracts and streaming ETL

## Setup

Get started below.

### Prerequisites

Make sure your development environment has the necessary prerequisites.

1. [Node.js (v16.x)](https://nodejs.org/en/download/) – we use [nvm](https://github.com/nvm-sh/nvm) to manage Node.js versions.

2. [VSCode](https://code.visualstudio.com/) – you could also use another editor, but this helps us guarantee linter/formatter features.

### Install

Clone the repository, checkout a new branch from develop, and install all dependencies.

```zsh
git clone https://github.com/consensusnetworks/ethereum-stack.git
cd ethereum-stack
git checkout -b feature/hodl-contract develop
npm install
```

## 💻 Development

### Hardhat

Compile the contracts in [contracts/](contracts/).

```zsh
npm run task:compile
```

Test the contracts with the tests in [scripts/hardhat/test/](scripts/hardhat/test/).

```zsh
npm run test:contracts
```

Deploy [contracts/Sample.sol](contracts/Sample.sol) with [scripts/hardhat/deploy/sample.ts](scripts/hardhat/deploy/sample.ts).

```zsh
npm run deploy:sample
```

Clean [build/artifacts/](build/artifacts/) and [build/cache/](build/cache/)). (Note, this is useful if you change the Hardhat configuration.)

```zsh
npm run task:clean
```

Start a local Ethereum node.

```zsh
npm run node:local
```

Print all local accounts.

```zsh
npm run task:accounts
```
