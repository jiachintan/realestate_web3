# Real Estate NFT DApp

## Technology Stack & Tools

- Solidity (Writing Smart Contracts & Tests)
- Javascript (React & Testing)
- [Hardhat](https://hardhat.org/) (Development Framework)
- [Ethers.js](https://docs.ethers.io/v5/) (Blockchain Interaction)
- [React.js](https://reactjs.org/) (Frontend Framework)

## Requirements For Initial Setup
- Install [NodeJS](https://nodejs.org/en/)

## Setting Up
### 1. Clone/Download the Repository

### 2. Install Dependencies:
`$ npm install`

### 3. Run tests
`$ npx hardhat test`

### 4. Start Hardhat node
`$ npx hardhat node`

### 5. Run deployment script
In a separate terminal execute:
`$ npx hardhat run ./scripts/deploy.js --network localhost`

### 7. Start frontend
`$ npm run start`

### 2025-12-18
Deploy to github pages
1. Update package.json by 
Add Homepage
Add Scripts: Add predeploy and deploy to the scripts section.
2. Install the Deployment Dependency
npm install gh-pages --save-dev
3. Deploy to GitHub Pages
npm run deploy
4. Final GitHub Settings
Under Build and deployment > Branch, ensure it is set to gh-pages and the folder is /(root)