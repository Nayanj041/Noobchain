# NoobChain - A Simple Blockchain in Java

NoobChain is a basic blockchain implementation in Java that includes transaction handling, proof-of-work mining, and wallet functionality using cryptographic signatures.

## Features
- **Blockchain Structure**: Implements a chain of blocks with cryptographic hashes.
- **Proof-of-Work**: Blocks are mined using a difficulty-based mechanism.
- **Transactions**: Supports transactions with digital signatures.
- **Wallet System**: Generates key pairs and maintains balances.
- **Validation**: Ensures blockchain integrity with verification mechanisms.

## Project Structure
```
/noobchain
│── Block.java             # Defines the block structure
│── NoobChain.java         # Main blockchain logic and execution
│── StringUtil.java        # Utility functions (SHA-256, Merkle root, etc.)
│── Transaction.java       # Transaction processing
│── TransactionInput.java  # Handles transaction inputs
│── TransactionOutput.java # Handles transaction outputs
│── Wallet.java            # Generates and manages user wallets
```

## How It Works
1. **Genesis Block**: The first block is manually created and mined.
2. **Mining Blocks**: Each block is added after solving a cryptographic puzzle.
3. **Transactions**: Wallets sign transactions, ensuring secure transfers.
4. **Validation**: The blockchain verifies integrity at each step.

## Installation & Usage
### Prerequisites
- Java 8 or later
- Bouncy Castle Security Provider (for cryptography)

### Running the Project
1. **Compile the project**:
   ```sh
   javac noobchain/*.java
   ```
2. **Run the blockchain simulation**:
   ```sh
   java noobchain.NoobChain
   ```

## Example Output
```
Creating and Mining Genesis block...
WalletA's balance is: 100.0
WalletA is Attempting to send funds (40) to WalletB...
Transaction Successfully added to Block
WalletA's balance is: 60.0
WalletB's balance is: 40.0
Blockchain is valid
```

## Future Improvements
- Implement a peer-to-peer network.
- Add persistent storage for blockchain data.
- Optimize transaction handling and mining efficiency.

## License
This project is for educational purposes. Feel free to use and modify it.
