# Capstone: Real Estate Marketplace

The capstone will build upon the knowledge you have gained in the course in order to build a decentralized housing product. 

## Installing

A step by step series of examples that tell you have to get a development environment running.

Install required npm packages
>npm install

Change directories into the contracts folder:
>cd eth-contracts

Launch Ganache - used GUI

Launch Truffle 
>truffle develop

Compile the smart contracts:
>compile

Migrate smart contracts to the locally running blockchain
>migrate --reset --network rinkeby

Test the smart contracts:
>You must be in the eth-contracts directory and ganache-cli must be running to successfully run these tests.
```shell script
truffle test test/TestERC721Mintable.js
truffle test test/TestSquareVerifier.js 
truffle test test/TestSolnSquareVerifier.js

# To run all tests use the following command
truffle test
```
 Zokrates Setup

>Install and instantiate a Zokrates zkSnarks development environment using Docker. Completes the Zokrates proof in square.code by adding the variable names in square.code.
When running Zokrates, follow examples given in the course.

## Contract Details
- SolnSquareVerifier Contract Address: 0x48F1290EfF08e79f5Dc944F9a319a19D396358CB
https://rinkeby.etherscan.io/address/0x48F1290EfF08e79f5Dc944F9a319a19D396358CB

- Verifier Contract Address: 0x906E23aedF2B4175426240387c362339E500c1A9
https://rinkeby.etherscan.io/address/0x906E23aedF2B4175426240387c362339E500c1A9

- Contract Owner: 0x7dD86Ef978A086F6635B21363515F09BC9E2800c



## Minting new tokens on MyEtherWallet(MEW)

Make sure you log into MEW with the address that created the contract(contract owner). 
Choose the interact with contract option and enter the following contract details:

* Contract Address: 0x48F1290EfF08e79f5Dc944F9a319a19D396358CB

* Contract ABI: See Section More Details

## Selling Tokens on OpenSea

 **Tokens Original Owner (Minter)**
 
0x7dD86Ef978A086F6635B21363515F09BC9E2800c
 **Tokens Buyer**
 
 0xeAB5f21096708513CBAe4B97Ef0fe9eDdced1194
 **Transaction Hashes for 5 Selling Operations**
 
0xe0d4dee05f9648f35d1ec2578dc22aec933dce5d8b4d54b9785c52b91610956c

0x8ea97073789cdfe1483c814a7cd3adbf756cf8b5bb35b02bc4d3ebd360d66768

0x3584d002681e7b350cf25bee34d90a70259034dc52886a0597b70eeec4e22fb4

0x63b16b050588208fe7c34b447ba54724947106b83ba87cee75ad7e1053681c83

0x45793a6103a160bf0a72d198ad81f2eea289fd5fdf2a18a0452bce5796496195

 **Storefront Links for Unsold Tokens**
https://testnets.opensea.io/assets/0x48f1290eff08e79f5dc944f9a319a19d396358cb/6


https://testnets.opensea.io/assets/0x48f1290eff08e79f5dc944f9a319a19d396358cb/7

https://testnets.opensea.io/assets/0x48f1290eff08e79f5dc944f9a319a19d396358cb/8

https://testnets.opensea.io/assets/0x48f1290eff08e79f5dc944f9a319a19d396358cb/9

https://testnets.opensea.io/assets/0x48f1290eff08e79f5dc944f9a319a19d396358cb/10

## Project Resources

* [Remix - Solidity IDE](https://remix.ethereum.org/)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Truffle Framework](https://truffleframework.com/)
* [Ganache - One Click Blockchain](https://truffleframework.com/ganache)
* [Open Zeppelin ](https://openzeppelin.org/)
* [Interactive zero knowledge 3-colorability demonstration](http://web.mit.edu/~ezyang/Public/graph/svg.html)
* [Docker](https://docs.docker.com/install/)
* [ZoKrates](https://github.com/Zokrates/ZoKrates)

## More Details

### Deployment Output
```shell script
 Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.



Migrations dry-run (simulation)
===============================
> Network name:    'rinkeby-fork'
> Network id:      4
> Block gas limit: 10000000 (0x989680)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > block number:        7803460
   > block timestamp:     1609279238
   > account:             0x7dD86Ef978A086F6635B21363515F09BC9E2800c
   > balance:             27.374197168894445729
   > gas used:            208305 (0x32db1)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00208305 ETH

   -------------------------------------
   > Total cost:          0.00208305 ETH


2_deploy_contracts.js
=====================

   Deploying 'verifier'
   --------------------
   > block number:        7803462
   > block timestamp:     1609279247
   > account:             0x7dD86Ef978A086F6635B21363515F09BC9E2800c
   > balance:             27.363397798894445729
   > gas used:            1052574 (0x100f9e)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.01052574 ETH


   Deploying 'SolnSquareVerifier'
   ------------------------------
   > block number:        7803463
   > block timestamp:     1609279539
   > account:             0x7dD86Ef978A086F6635B21363515F09BC9E2800c
   > balance:             27.328469308894445729
   > gas used:            3492849 (0x354bf1)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.03492849 ETH

   -------------------------------------
   > Total cost:          0.04545423 ETH


Summary
=======
> Total deployments:   3
> Final cost:          0.04753728 ETH





Starting migrations...
======================
> Network name:    'rinkeby'
> Network id:      4
> Block gas limit: 10000000 (0x989680)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0x57876ae9c33b598a6efcfbab4036fac74f272448d4a761de5750572d783c28ab
   > Blocks: 2            Seconds: 20
   > contract address:    0xE84239A68205Ff47cf07a64D77629866F865d3bC
   > block number:        7803483
   > block timestamp:     1609279586
   > account:             0x7dD86Ef978A086F6635B21363515F09BC9E2800c
   > balance:             27.374047168894445729
   > gas used:            223305 (0x36849)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.00223305 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00223305 ETH


2_deploy_contracts.js
=====================

   Deploying 'verifier'
   --------------------
   > transaction hash:    0x67c804e530b3ed60d1d9bb625e1f42a7e1f4a818ca8001faa9d0bde22e3412e0
   > Blocks: 4            Seconds: 56
   > contract address:    0x906E23aedF2B4175426240387c362339E500c1A9
   > block number:        7803490
   > block timestamp:     1609279691
   > account:             0x7dD86Ef978A086F6635B21363515F09BC9E2800c
   > balance:             27.363097798894445729
   > gas used:            1052574 (0x100f9e)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.01052574 ETH


   Deploying 'SolnSquareVerifier'
   ------------------------------
   > transaction hash:    0x6d7f5a41755d575c859f5a94ac4986d592671e803685909a7926b41fa917a45b
   > Blocks: 1            Seconds: 8
   > contract address:    0x48F1290EfF08e79f5Dc944F9a319a19D396358CB
   > block number:        7803491
   > block timestamp:     1609279706
   > account:             0x7dD86Ef978A086F6635B21363515F09BC9E2800c
   > balance:             27.326369308894445729
   > gas used:            3672849 (0x380b11)
   > gas price:           10 gwei
   > value sent:          0 ETH
   > total cost:          0.03672849 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.04725423 ETH


Summary
=======
> Total deployments:   3
> Final cost:          0.04948728 ETH
```

### Contract ABI
```shell script
"abi": [
    {
      "constant": true,
      "inputs": [
        {
          "name": "_address",
          "type": "address"
        }
      ],
      "name": "isValidAddress",
      "outputs": [
        {
          "name": "",
          "type": "bool"
        }
      ],
      "payable": false,
      "stateMutability": "pure",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "interfaceId",
          "type": "bytes4"
        }
      ],
      "name": "supportsInterface",
      "outputs": [
        {
          "name": "",
          "type": "bool"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "getApproved",
      "outputs": [
        {
          "name": "",
          "type": "address"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "to",
          "type": "address"
        },
        {
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "approve",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [],
      "name": "getSymbol",
      "outputs": [
        {
          "name": "",
          "type": "string"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "paused",
          "type": "bool"
        }
      ],
      "name": "setPaused",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [],
      "name": "getName",
      "outputs": [
        {
          "name": "",
          "type": "string"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [],
      "name": "totalSupply",
      "outputs": [
        {
          "name": "",
          "type": "uint256"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "from",
          "type": "address"
        },
        {
          "name": "to",
          "type": "address"
        },
        {
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "transferFrom",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "_myid",
          "type": "bytes32"
        },
        {
          "name": "_result",
          "type": "string"
        }
      ],
      "name": "__callback",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "owner",
          "type": "address"
        },
        {
          "name": "index",
          "type": "uint256"
        }
      ],
      "name": "tokenOfOwnerByIndex",
      "outputs": [
        {
          "name": "",
          "type": "uint256"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "_myid",
          "type": "bytes32"
        },
        {
          "name": "_result",
          "type": "string"
        },
        {
          "name": "_proof",
          "type": "bytes"
        }
      ],
      "name": "__callback",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "to",
          "type": "address"
        },
        {
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "mint",
      "outputs": [
        {
          "name": "",
          "type": "bool"
        }
      ],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "from",
          "type": "address"
        },
        {
          "name": "to",
          "type": "address"
        },
        {
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "safeTransferFrom",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [],
      "name": "getContractOwner",
      "outputs": [
        {
          "name": "",
          "type": "address"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [],
      "name": "squareVerifier",
      "outputs": [
        {
          "name": "",
          "type": "address"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "index",
          "type": "uint256"
        }
      ],
      "name": "tokenByIndex",
      "outputs": [
        {
          "name": "",
          "type": "uint256"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "ownerOf",
      "outputs": [
        {
          "name": "",
          "type": "address"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "owner",
          "type": "address"
        }
      ],
      "name": "balanceOf",
      "outputs": [
        {
          "name": "",
          "type": "uint256"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "to",
          "type": "address"
        },
        {
          "name": "approved",
          "type": "bool"
        }
      ],
      "name": "setApprovalForAll",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "from",
          "type": "address"
        },
        {
          "name": "to",
          "type": "address"
        },
        {
          "name": "tokenId",
          "type": "uint256"
        },
        {
          "name": "_data",
          "type": "bytes"
        }
      ],
      "name": "safeTransferFrom",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [],
      "name": "getBaseTokenURI",
      "outputs": [
        {
          "name": "",
          "type": "string"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "tokenURI",
      "outputs": [
        {
          "name": "",
          "type": "string"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": true,
      "inputs": [
        {
          "name": "owner",
          "type": "address"
        },
        {
          "name": "operator",
          "type": "address"
        }
      ],
      "name": "isApprovedForAll",
      "outputs": [
        {
          "name": "",
          "type": "bool"
        }
      ],
      "payable": false,
      "stateMutability": "view",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "newOwner",
          "type": "address"
        }
      ],
      "name": "transferOwnership",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        {
          "name": "verifierAddress",
          "type": "address"
        }
      ],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "constructor"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "name": "_index",
          "type": "uint256"
        },
        {
          "indexed": false,
          "name": "_address",
          "type": "address"
        }
      ],
      "name": "SolutionAdded",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "name": "owner",
          "type": "address"
        },
        {
          "indexed": true,
          "name": "uri",
          "type": "string"
        }
      ],
      "name": "NewTokenMinted",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "name": "from",
          "type": "address"
        },
        {
          "indexed": true,
          "name": "to",
          "type": "address"
        },
        {
          "indexed": true,
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "Transfer",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "name": "owner",
          "type": "address"
        },
        {
          "indexed": true,
          "name": "approved",
          "type": "address"
        },
        {
          "indexed": true,
          "name": "tokenId",
          "type": "uint256"
        }
      ],
      "name": "Approval",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": true,
          "name": "owner",
          "type": "address"
        },
        {
          "indexed": true,
          "name": "operator",
          "type": "address"
        },
        {
          "indexed": false,
          "name": "approved",
          "type": "bool"
        }
      ],
      "name": "ApprovalForAll",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "name": "pauser",
          "type": "address"
        }
      ],
      "name": "Paused",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "name": "unpauser",
          "type": "address"
        }
      ],
      "name": "Unpaused",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        {
          "indexed": false,
          "name": "newOwner",
          "type": "address"
        }
      ],
      "name": "OwnershipTransferred",
      "type": "event"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "Id",
          "type": "uint256"
        },
        {
          "name": "owner",
          "type": "address"
        }
      ],
      "name": "addSolution",
      "outputs": [],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "constant": false,
      "inputs": [
        {
          "name": "Id",
          "type": "uint256"
        },
        {
          "name": "a",
          "type": "uint256[2]"
        },
        {
          "name": "b",
          "type": "uint256[2][2]"
        },
        {
          "name": "c",
          "type": "uint256[2]"
        },
        {
          "name": "input",
          "type": "uint256[1]"
        }
      ],
      "name": "mintTokens",
      "outputs": [
        {
          "name": "result",
          "type": "bool"
        }
      ],
      "payable": false,
      "stateMutability": "nonpayable",
      "type": "function"
    }
  ],
```