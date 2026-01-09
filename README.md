This is a very simple web application which reads block data from the ethereum blockchain (testnet) using web3.js.  

Web3.js is a library which provides an interface to the EVM (Ethereum Virtual Machine) through an ethereum node.

This node will run locally for this application.  To do this, we connect to the ethereum blockchain (testnet, in this case), using the Geth (Go / Ethereum) client.

Running Geth locally will sync the specified network (mainnet, testnet, etc...) to your machine. This will act as web3.js's portal into the chosen ethereum blockchain. This functionality is automated from within the "npm start" script.

## Setup
Install geth
https://geth.ethereum.org/install/

Install application dependencies:
```sh
npm install
npm start
```

NOTE:
Within your terminal, you should notice the local app-server AND the geth client running concurrently.  If this is your first time syncing to the ethereum blockchain, you may need to wait until the sync is complete before you will receive accurate blockchain data from within the application.

Navigate to http://localhost:3000/