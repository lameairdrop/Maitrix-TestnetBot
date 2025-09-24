
# Maitrix Testnet Bot 🤖

An automated bot for interacting with the Maitrix Testnet ecosystem, handling faucet claims, token minting, and staking operations

**GitHub Repository**: https://github.com/lameairdrop/Maitrix-Testnet-Bot

## 🚀 Features

- **Multi-Faucet Claims**: Automatically claim from 6 different Maitrix faucets
- **Token Minting**: Convert ATH → AUSD, VIRTUAL → VUSD, AI16Z → AZUSD
- **Staking Operations**: Stake multiple tokens (AUSD, VUSD, AZUSD, LVLUSD, USDe, USD1)
- **Auto-Retry System**: Built-in retry logic for failed transactions
- **Gas Optimization**: Automatic gas estimation and price checking
- **24/7 Operation**: Continuous cycle with 24-hour intervals

## 📋 Requirements

- Node.js (v16 or higher)
- Sepolia ETH for gas fees
- Wallet with private key

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/lameairdrop/Maitrix-Testnet-Bot.git
   cd Maitrix-Testnet-Bot
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure environment**:
   - Create a `.env` file in the root directory
   - Add your configuration:
     ```
     RPC_URL=https://sepolia-rollup.arbitrum.io/rpc
     PRIVATE_KEY=0xYourPrivateKeyHere
     ```

4. **Run the bot**:
   ```bash
   node main.js
   ```

## ⚙️ Supported Operations

### 🔹 Faucet Claims
- ATH Faucet
- USDe Faucet  
- LVL Faucet
- Virtual Faucet
- USD1 Faucet (with code verification)
- AI16Z Faucet (with code verification)

### 🔹 Minting Operations
- ATH → AUSD (50 ATH required)
- VIRTUAL → VUSD (2 VIRTUAL required)
- AI16Z → AZUSD (5 AI16Z required)

### 🔹 Staking Operations
- AUSD Staking
- VUSD Staking
- AZUSD Staking
- LVLUSD Staking
- USDe Staking
- USD1 Staking

## ⚠️ Important Notes

- **Testnet Only**: Designed for Arbitrum Sepolia testnet only
- **Gas Fees**: Ensure wallet has sufficient SEPOLIA ETH for transaction fees
- **Token Requirements**: Some minting operations require specific token balances
- **24-Hour Cycles**: Bot runs on 24-hour intervals for faucet cooldowns
- **Use at Your Own Risk**: Always understand what transactions are being executed

## 📝 File Structure

```
Maitrix-Testnet-Bot/
├── main.js          # Main bot script
├── .env             # Environment variables (create manually)
├── package.json     # Dependencies
└── README.md        # This file
```

## 🔧 Configuration Options

- `RPC_URL`: Arbitrum Sepolia RPC endpoint
- `PRIVATE_KEY`: Your wallet private key (keep this secure!)

## ❓ Support

For issues and questions, please check the GitHub repository issues section.

## ⏰ Operation Cycle

The bot runs continuously with:
1. Faucet claims from all 6 sources
2. Minting operations (if tokens available)
3. Staking operations
4. 24-hour wait period before next cycle
```

