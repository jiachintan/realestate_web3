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

### 2025-12-17
Deploy to github pages
1. Update package.json by 
`Add Homepage
`Add Scripts: Add predeploy and deploy to the scripts section.
2. Install the Deployment Dependency
`npm install gh-pages --save-dev
3. Deploy to GitHub Pages
`npm run deploy
4. Final GitHub Settings
`Under Build and deployment > Branch, ensure it is set to gh-pages and the folder is /(root)

### 2025-12-18
`Deploy smart contract 
1. Environment Configuration (.env)
`Store Alchemy RPC URL and MetaMask Private Key.
2. Hardhat Settings (hardhat.config.js)
`Imported dotenv to load the credentials.
`Configured the networks object with the Sepolia url and accounts.
`Added the specific Chain ID for Sepolia (11155111).
3. Deployment Script Logic (scripts/deploy.js)
`Updated the deployment script to use a single Sepolia account for all roles and replaced local metadata with public IPFS links to ensure the app works correctly on a live testnet.
4. Frontend Integration (src/config.json)
`Updated the frontend configuration by copying the unique "Real Estate" and "Escrow" addresses from the deployment terminal into the Sepolia section of the JSON config to ensure the website connects to the new contracts.
5. Deployment Command
`npx hardhat compile
`npx hardhat run scripts/deploy.js --network sepolia
`npm run deploy