# Decentralized-Finance-Lending-Network

Peer 2 peer lending platform on the Ethereum blockchain network.

# About
This project is a Peer-to-Peer (P2P) lending platform built on the Ethereum blockchain network. This decentralized platform connects borrowers and lenders directly, eliminating the need for traditional financial intermediaries. The use of smart contracts ensures secure, transparent, and efficient transactions.

Key Features:

Decentralization: Built on the Ethereum blockchain to ensure trust and transparency.
Smart Contracts: Automates lending agreements, reducing the risk of fraud.
Fair Interest Rates: Competitive rates for both borrowers and lenders.
No Hidden Fees: Transparent fee structure with no surprises.
Security: Robust security measures to protect user data and funds.
Functionalities:

Borrowing:
Request Funding: Users can create funding requests for their projects.
Funding Details: Provides detailed information about the requested funding.
Withdrawal: Allows borrowers to withdraw funds after successfully reaching the full funding goal.
Repayment Installments: Enables borrowers to repay the loan in installments.
Lending:
Invest in Projects: Users can lend their funds to various projects and credits.
Vote for Contract Revoke/Refund: Lenders can vote to revoke a contract and refund their investments if necessary.
Fraud Detection: Users can mark projects as fraud if they suspect malicious activities.
Technologies Used:

Blockchain: Ethereum
Smart Contracts: Solidity
Frontend: React.js
Backend: Node.js, Express.js
Database: MongoDB
Wallet Integration: MetaMask
Deployment: IPFS, Infura
Testing: Truffle, Mocha
## Chart flow

![Chart flow](https://i.imgur.com/vRq7nAN.png)

### Further development

  - Improve external contract calls.
  - Minimize gas cost.
  - Create more investors protection.

### Requirements
* [Node.js](https://nodejs.org/)
* [Truffle](https://truffleframework.com/)
* [Ganache](https://truffleframework.com/ganache/)
* [MetaMask](https://metamask.io/)
    
### Installation

1. Start Ganache on ``localhost:7545``   

2. Build and migrate smart contracts

```sh
$ cd p2p-lending/smart-contracts
$ truffle compile
$ truffle migrate --reset --network development --verbose-rpc
```

3. Set the ``PeerToPeerLending`` contract newly published address in the [client-app/public/js/contract_interaction.js LINE:3](https://github.com/mradkov/p2p-lending/blob/370bde2a452caff4831d5e91157f733ce9921a99/client-app/public/js/contract_interaction.js#L5) 

4. Install the dependencies and devDependencies and start the server.

```sh
$ cd p2p-lending/client-app
$ npm install --save
$ npm start
```

5. Your app is running on ``http://localhost:1337``



