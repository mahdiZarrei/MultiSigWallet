# MultiSigWallet

![MultiSigWallet image](./pic/MultiSigWallet.jpg)

This project implements a MultiSigWallet smart contract using Hardhat. A MultiSigWallet is a type of cryptocurrency wallet that requires multiple signatures to authorize a transaction. This increases security by ensuring that no single party can unilaterally control the funds.

## Overview

A MultiSigWallet is akin to a bank vault that requires multiple keys to open. In this setup, you can specify how many keys are needed to authorize a transaction. For example, in a 2-of-3 MultiSigWallet, any two out of three designated key holders must sign a transaction for it to be executed. This setup is commonly used by organizations, investment funds, and crypto exchanges to enhance security and distribute control over funds.

## Prerequisites

- Node.js (version 14 or higher)
- npm or yarn
- Hardhat

## Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/username/MultiSigWallet.git
cd MultiSigWallet
npm install
# or
yarn install
```

## Configuration

Create a `.env` file in the root directory and set the following variables:

```plaintext
PRIVATE_KEY=your_private_key
INFURA_PROJECT_ID=your_infura_project_id
```

## Compilation

To compile the smart contracts, run:

```bash
npx hardhat compile
```

## Testing

To run the tests, use:

```bash
npx hardhat test
```

## Deployment

To deploy the contracts to a local network, run:

```bash
npx hardhat run scripts/deploy.js --network localhost
```

For deployment to other networks (e.g., Rinkeby), configure the `hardhat.config.js` file and then execute:

```bash
npx hardhat run scripts/deploy.js --network rinkeby
```

## Usage

After deployment, you can use the MultiSigWallet contract to manage transactions requiring multiple signatures. For more details, refer to the contract documentation.

## Contributing

We welcome contributions! Please open an issue to discuss your changes before submitting a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
