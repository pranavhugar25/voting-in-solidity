# Blockchain-Based Voting System (Solidity + Remix IDE)

This project is a decentralized voting system built using Solidity and tested on Remix IDE. It allows transparent, secure, and tamper-proof elections on the Ethereum blockchain. The contract ensures one vote per participant and declares the winner only after the voting phase has ended.

---

## Features

- Admin-controlled voting (start and end voting sessions)  
- One vote per wallet address  
- Real-time vote count tracking  
- Automatic winner calculation  
- Immutable and transparent voting process

---

## Technologies Used

- Solidity ^0.8.20  
- Remix IDE  
- MetaMask for interacting with testnets (optional)

---

## How It Works

1. Admin deploys the contract with a list of candidate names.
2. Admin starts the election using `startVoting()`.
3. Each Ethereum address can vote once for their preferred candidate.
4. Admin ends the voting using `endVoting()`.
5. Anyone can call `getWinner()` to see who won based on the highest vote count.

---

## Testing Instructions

1. Open [Remix IDE](https://remix.ethereum.org/) and create a new file named `Voting.sol`.
2. Paste the contract code into the file.
3. Compile it using Solidity version ^0.8.20.
4. Go to the Deploy & Run Transactions tab.
5. Deploy the contract with an input like:
   ```json
   ["Alice", "Bob"]

