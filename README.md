# Decentralized E-Vault

Welcome to the Decentralized E-Vault! This repository contains the source code for a decentralized file storage system built using MetaMask, React, Solidity, Pinata, and TailwindCSS. The Decentralized E-Vault allows users to securely store and manage their files on a decentralized network, leveraging the power of Web3 technology.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technology](#technology)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Smart Contract](#smart-contract)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Decentralized E-Vault is designed to provide a secure and decentralized way to store and manage files. By using blockchain technology and IPFS (InterPlanetary File System), it ensures data integrity, security, and accessibility without relying on centralized servers.

## Features
- **Decentralized Storage**: Store files securely on the IPFS network.
- **MetaMask Integration**: Authenticate and interact with the blockchain using MetaMask.
- **User-friendly Interface**: A responsive and intuitive user interface built with React and TailwindCSS.
- **Smart Contracts**: Solidity smart contracts to handle file metadata and ownership.
- **Secure and Transparent**: Ensures data security and transparency through blockchain technology.

## Technology
The Decentralized E-Vault leverages several modern technologies to provide a robust and secure file storage solution:

- **MetaMask**: A browser extension to interact with the Ethereum blockchain.
- **React**: A JavaScript library for building user interfaces.
- **Solidity**: A programming language for writing smart contracts on the Ethereum blockchain.
- **Pinata**: A service to manage and pin files to the IPFS network.
- **TailwindCSS**: A utility-first CSS framework for rapid UI development.
- **Hardhat**: A development environment to compile, deploy, test, and debug Ethereum software.

## Prerequisites
Before you begin, ensure you have met the following requirements:
- [Node.js](https://nodejs.org/en/download/) (v14.x or later)
- [MetaMask](https://metamask.io/) browser extension
- An Ethereum test network (e.g., Ropsten, Rinkeby) account
- Pinata account for IPFS storage

## Installation
To install and run this project locally, follow these steps:

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/decentralized-e-vault.git
    cd decentralized-e-vault
    ```

2. **Install dependencies:**
    ```sh
    npm install
    ```

3. **Configure environment variables:**
    Create a `.env` file in the root directory and add your Pinata API keys and other necessary configurations:
    ```plaintext
    REACT_APP_PINATA_API_KEY=your_pinata_api_key
    REACT_APP_PINATA_SECRET_API_KEY=your_pinata_secret_api_key
    REACT_APP_INFURA_PROJECT_ID=your_infura_project_id
    ```

4. **Deploy the smart contract:**
    Ensure you have MetaMask connected to your preferred Ethereum test network and run the following command:
    ```sh
    npx hardhat run scripts/deploy.js --network rinkeby
    ```

    Note the contract address displayed after deployment.

5. **Update the contract address in the frontend:**
    In the `src/constants/contractAddress.js` file, update the contract address with the one obtained from the previous step.

6. **Start the development server:**
    ```sh
    npm start
    ```

## Usage
1. Open your browser and navigate to `http://localhost:3000`.
2. Connect your MetaMask wallet.
3. Upload files and manage your decentralized storage through the interface.

## Smart Contract
The smart contract for this project is written in Solidity and is responsible for managing file metadata and ownership. The contract is located in the `contracts` directory. You can interact with the contract using the provided frontend or via command-line tools like `hardhat` or `web3.js`.

## Contributing
Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make your changes and commit them (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Thank you for using the Decentralized E-Vault! If you have any questions or need further assistance, please open an issue in this repository.



## Run commands 

```bash
npm start 


npx hardhat node


npx hardhat run --network localhost scripts/deploy.js
```
