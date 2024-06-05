# BankAccount-A-Multi-Signature-Ethereum-Wallet
This full-stack project demonstrates a multi-signature (multi-sig) wallet implemented as a smart contract on the Ethereum blockchain. Multi-sig wallets enhance security by requiring multiple owner approvals for transactions, making them ideal for shared finances or organizational funds.

Key Features
⦁	Multi-Signature Security: Transactions require approval from a specified number of owners.
⦁	Deposit: Allows users to deposit Ether (ETH) into the shared account.
⦁	Withdrawal Request: Owners can initiate withdrawal requests.
⦁	Approval Process: Other owners can approve or reject withdrawal requests.
⦁	Withdrawal: Approved withdrawals transfer funds to the requester's address.
⦁	Account Management: Create accounts with multiple owners, view account balances, and review transaction history.

Technical Overview
Blockchain: Ethereum (Chosen for its mature ecosystem and established smart contract capabilities)
Smart Contracts:
Language: Solidity (>=0.7.0 <=0.9.0)
Core Functions:
createAccount(address[] otherOwners): Creates a multi-sig account.
deposit(uint256 accountId): Deposits ETH into the specified account.
requestWithdrawl(uint256 accountId, uint256 amount): Initiates a withdrawal request.
approveWithdrawl(uint256 accountId, uint256 withdrawId): Approves a withdrawal request.
withdraw(uint256 accountId, uint256 withdrawId): Executes an approved withdrawal.
(other functions for account management and viewing)
Frontend:
HTML: base.html (Provides the basic structure and UI elements)
JavaScript: script.js (Interacts with the smart contract using ethers.js library)
User Interface: Includes input fields for account creation, buttons for interacting with the contract, and areas to display accounts and events.

Getting Started

Prerequisites:
MetaMask: Install and configure the MetaMask browser extension to interact with the Ethereum blockchain.
Node.js and npm: Ensure Node.js and npm are installed on your system.

Installation:
Bash
git clone https://your-github-repo.git
cd bankaccount
Use code with caution.
content_copy
Configuration:
Open script.js and update the address variable with the deployed smart contract address.
Running the Project:
Open base.html in your web browser.
Connect your MetaMask wallet to the DApp.
Interacting with the DApp:
Use the provided UI to create accounts, deposit ETH, request withdrawals, approve withdrawals, and view account details.

Project Moto
This project aims to provide a user-friendly, yet secure, way to manage shared funds on the Ethereum blockchain, leveraging the transparency and immutability of blockchain technology.
