# My First Decentralized Application (dApp)

This is a simple Ethereum-based decentralized application (dApp) that interacts with a smart contract to store and retrieve a "mood." The application demonstrates how to integrate the Ethereum blockchain with a front-end interface using `ethers.js`.

---

## Features

- **Set Mood**: Allows users to input and store a mood on the blockchain.
- **Get Mood**: Retrieves the currently stored mood from the blockchain.
- **Blockchain Integration**: Interacts with an Ethereum smart contract deployed on the Sepolia test network.

---

## Prerequisites

To run this project, ensure you have the following:

1. **MetaMask**:
   - Installed as a browser extension.
   - Connected to the Sepolia test network.
   - Test ETH in your wallet to pay for transactions.

2. **Node.js**:
   - Installed on your system.
   - Includes `npm` for package management.

3. **Smart Contract**:
   - Deployed at the address: `0xf1b501122be7736fdaf9e553abe722afc8f410e0`.

---

## Installation

Follow these steps to set up and run the project locally:

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd aish-themagician-web3_
   ```

2. **Install Dependencies**:
   ```bash
   npm install
   ```

3. **Start the Development Server**:
   ```bash
   npm start
   ```

4. **Access the dApp**:
   Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

---

## Usage

1. Open the application in your browser.
2. Ensure MetaMask is unlocked and connected to the Sepolia test network.
3. Use the input field to enter a mood and click **Set Mood** to store it on the blockchain.
4. Click **Get Mood** to retrieve the stored mood.

---

## File Structure

```
└── aish-themagician-web3_/
    ├── README.md              # Project documentation
    ├── index.html             # Main front-end interface
    ├── package.json           # Project metadata and scripts
    └── package-lock.json      # Dependency lock file
```

---

## Technologies Used

- **Ethereum Blockchain**
- **Smart Contracts** (ABI interaction)
- **Ethers.js**
- **MetaMask** for wallet integration
- **Lite Server** for local development

---

## Smart Contract Details

- **Address**: `0xf1b501122be7736fdaf9e553abe722afc8f410e0`
- **Network**: Sepolia Test Network
- **ABI**:
  ```json
  [
    {
      "inputs": [
        { "internalType": "string", "name": "_mood", "type": "string" }
      ],
      "name": "setMood",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "getMood",
      "outputs": [
        { "internalType": "string", "name": "", "type": "string" }
      ],
      "stateMutability": "view",
      "type": "function"
    }
  ]
  ```

---

## Troubleshooting

- **MetaMask Not Connecting**: Ensure the wallet is unlocked and set to the Sepolia network.
- **Error in Transactions**: Check if you have sufficient test ETH in your wallet.
- **Server Not Running**: Verify that `npm install` and `npm start` completed without errors.

---

## Future Improvements

1. **UI Enhancements**:
   - Display retrieved mood in the interface instead of the console.
   - Add user feedback for transaction success or failure.

2. **Validation**:
   - Ensure mood input is not empty.

3. **Error Handling**:
   - Gracefully handle blockchain interaction failures.

---

## License

This project is licensed under the ISC License.

---

## Author

Aishwarya Maan Srivastava
