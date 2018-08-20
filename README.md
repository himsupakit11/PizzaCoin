<p align="center"><a href="#" target="_blank" rel="noopener noreferrer"><img width="100" src="https://raw.githubusercontent.com/totiz/LiveDashboard/dev/images/Pizza_Hackathon_Logo.png" alt="Vue logo"></a></p>

<h2 align="center">Pizza Coin</h2>

Pizza Coin is a demonstration of Voting system on Blockchain, utilizing <a href="https://www.ethereum.org/">Ehtereum</a> Blockchain with <a href="https://solidity.readthedocs.io/">Smart contracts</a>. Developed for the 1st Thailand's blockchain hackathon named <a href="https://www.facebook.com/events/205814763443058/">Pizza Hackathon 2018</a>.

Pizza Coin is <a href="https://en.wikipedia.org/wiki/ERC-20">ERC20</a> compatible with voting mechanism, allowing player to participate in creating / joining team and voting. Authorized staff can perform "kick player", "kick team", "freeze and transfer tokens" and "start / stop voting".

Each player and each staff has the same amount of PZC for voting. Specifically, a player can give a vote to any teams that he/she is not associated with whereas a staff is freely to give a vote to any teams. Each voter is able to vote to any favourite teams according to his/her own voting token balance.

### Pizza Coin consists of two parts
<p align="center">
  <a href="#" target="_blank">
    <img width="260px" src="https://raw.githubusercontent.com/totiz/LiveDashboard/dev/images/ethereum-smart-contract.jpeg">
  </a> 
  <a href="#" target="_blank">
    <img width="260px" src="https://raw.githubusercontent.com/totiz/LiveDashboard/dev/images/DApp.png">
  </a>
</p>

## Smart Contract
<img src="https://raw.githubusercontent.com/totiz/LiveDashboard/dev/images/Smart-contract-screenshot-PizzaCoin.png">
description: Pizza Coin Contract

#### To install Truffle Framework
<a href="https://truffleframework.com/docs/truffle/getting-started/installation">follow this link</a>

#### To install Node.JS packages required by Truffle
```
npm install
```

#### To set up 'mnemonic.secret' file
```
echo "'your-secret-mnemonic'" > mnemonic.secret  // Your secret mnemonic must be marked with single quotes
```

#### To compile PizzaCoin contract and its dependencies
```
truffle compile
```

#### To deploy PizzaCoin contract and its dependencies
```
truffle migrate --network ropsten  // Deploy to Ropsten testnet via Infura
```

```
truffle migrate --network rinkeby  // Deploy to Rinkeby testnet via Infura
```

```
truffle migrate --network rinkeby_localsync  // Deploy to Rinkeby testnet via local Geth node
```

```
truffle migrate --network ganache  // Deploy to Ganache local test environment
```

#### To install Node.JS packages required by lazy-web3-wrapper functions
```
cd run
npm install
```

#### To execute Node.JS based lazy-web3-wrapper functions (for demo)
```
cd run
node main.js
```

## DApp ( Decentralized Application )
<img src="https://raw.githubusercontent.com/totiz/LiveDashboard/dev/images/DApp-screenshot-teams.jpg">
description: TBD

#### Run Team Dashboard
- cd DApp
- npm install
- npm run serve

#### Run Live Feed
- cd live-feed
- npm install
- npm run serve

#### Run Live Feed Api server
- cd live-feed
- TBD

#### Configure
## store/system.js
- **network**: Ethereum network 'mainnet', 'ropsten', 'rinkeby', 'kovan' or etc.
- **etherscanPrefix**: Etherscan url, you need to configure according to network.
- **ethereumNode**: Public or Private Ethereum node, in case of user don't have Web3 provider like 'Metmask'. **Web socker** is need for Leader Board that checking real time incoming votes. exp: 'wss://rinkeby.infura.io/_ws'
- **pizzaCoinAddr**: Deployed Pizza Coin Contract Address
- **pizzaCoinStaffAddr**: Deployed Pizza Coin Staff Address
- **pizzaCoinTeamAddr**: Deployed Pizza Coin Team Address
- **pizzaCoinPlayerAddr**: Deployed Pizza Coin Player Address

** For **pizzaCoinAddr**, **pizzaCoinStaffAddr**, **pizzaCoinTeamAddr** and **pizzaCoinPlayerAddr** please consult in Pizza-Coin directory.


# Contributors

## Coders
- <a href="https://github.com/serial-coder">Bright</a> (Smart Contract)
- <a href="https://github.com/teerapat1739">Game</a> (DApp Team)
- <a href="https://github.com/zent-bank">Bank</a> (DApp Leader board)

## Advisors
- <a href="https://github.com/totiz?tab=repositories">Tot Nattapon </a>
- <a href="https://nuuneoi.com/">Nuuneoi</a>
