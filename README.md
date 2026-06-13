# Healthcare E-Vault

A decentralized healthcare record management system built on Ethereum blockchain that enables secure storage, sharing, and access control of medical records using IPFS and smart contracts.

## Features

* Secure storage of medical record references using IPFS
* Blockchain-based ownership and access control
* Upload and manage healthcare documents
* Grant and revoke access to healthcare records
* Transparent and tamper-resistant data management
* Decentralized architecture for enhanced security

## Technology Stack

* **Blockchain:** Ethereum
* **Smart Contracts:** Solidity
* **Development Framework:** Hardhat
* **Frontend:** React.js
* **Wallet Integration:** MetaMask
* **Storage:** IPFS

## Project Structure

```text
Healthcare_E_Vault/
├── client/              # React frontend
├── contracts/           # Solidity smart contracts
├── medical_chat/        # Backend/chat module
├── scripts/             # Deployment scripts
├── test/                # Smart contract tests
├── hardhat.config.js    # Hardhat configuration
└── README.md
```

## Prerequisites

Before running the project, ensure you have:

* Node.js (v16 or later)
* npm
* Hardhat
* MetaMask Browser Extension

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd Healthcare_E_Vault
```

### Install Dependencies

```bash
npm install
```

## Running the Project

### Start Local Blockchain

```bash
npx hardhat node
```

### Deploy Smart Contract

Open a new terminal and run:

```bash
npx hardhat run scripts/deploy.js --network localhost
```

### Start Frontend

```bash
cd client
npm install
npm start
```

The application will be available on:

```text
http://localhost:3000
```

## Smart Contract Functionalities

### Upload Medical Records

```javascript
await uploadInstance.add(userAddress, "ipfs://medical-record");
```

### View Records

```javascript
await uploadInstance.display(userAddress);
```

### Remove Records

```javascript
await uploadInstance.removeFile(index);
```

### Grant Access

```javascript
await uploadInstance.allow(otherUserAddress);
```

### Revoke Access

```javascript
await uploadInstance.disallow(otherUserAddress);
```

## Security Benefits

* Decentralized record ownership
* Immutable transaction history
* User-controlled permissions
* Reduced risk of centralized data breaches
* Transparent access management

## Future Enhancements

* Role-based access for doctors and hospitals
* Multi-signature approvals
* Encrypted medical records
* Patient consent management
* Audit logs and analytics

## License

This project is licensed under the MIT License.
