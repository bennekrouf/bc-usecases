
I was wondering what could be some use cases for development projects in the blockchain. After some research here is a starting list.

# Easy

## Hello world

[Code](https://github.com/alto-io/hello-crypto)

- Connect to eth via web3
    (if not web3/metamask instance is detected fallback to truffle - local peer instance)
- get account ID and balance (in js BigNumber)
- store the contract (a simple ERC20 token that sets a balance and do a transfer to the sender - see [OpenZeppelin](https://openzeppelin.com/) contracts)
    - get the essential artifact of the contract and instantiate it with truffle
    - set the provider of the contract (web3 instance)
    - invoke the contract to get the balance
    - return the balance

## Simple storage

[Code](https://github.com/ethers-io/tutorial-simplestore)

Store information in a smart contracts and allow modify this information
- Connect to an existing contract in the bc using ethers-cli
- Allow setting and getting a value from the deployed/instanciated contract


## Multi-send

[Code](https://github.com/miguelmota/eth-send)

Allow sending ethers to multiple addresses


## Ether wallet


Create a smart contracts that allows sending and receiving ethers in a wallet

[Code](https://github.com/MyEtherWallet/etherwallet)


## Polling system

Allow people to create a new poll with different choices and a voting period, users to select one choice. And the system compute the winner after the voting period expire.

[Implementation example](https://github.com/doriancrutcher/blockvotetutorial2)


# Medium complexity


## Time lock wallet
Special wallet that keeps crypto locked for a certain amount of time.

[Example](https://github.com/mattdf/TimeLock)

## To-do list app

A smart contract on the blockchain that allows you to add, remove items of a to-do list stored on the blockchain.

[Example](https://github.com/dappuniversity/eth-todo-list)

## Voting system

Only identify users by their address and keep privacy. Control that one person only put one vote. Also control that a person is elligible for voting.

[Example](https://github.com/sanattaori/techdot)




## Savings and lending application

An an that allow borrowing and lending cryptos.


[Code](https://github.com/mradkov/p2p-lending)


## Decentralized cryptocurrency exchange

Create smarts contracts that enable the trading of any ethereum assets (crypto, tokens..etc). Then create a frontend client to allow interacting with these smart contracts using web3

[Example of implementation](https://github.com/gitbitex/gitbitex-spot)



# Advanced use cases

## Blockchain wallet

A wallet allows signing a transaction with the user's private key.

[Example](https://github.com/dappuniversity/eth_wallet)


## Digital asset marketplace (DAM)

A DAM is a trusted intermediary between issuers and investors of digital assets. Provide tools to facilite transactions between users.

[Example 1](https://github.com/dappuniversity/nft)
[Example 2](https://github.com/dappuniversity/marketplace)


## Peer to peer carpooling

To avoid privacy issues with data, create a system that allows ride-sharing and car hire occuring on the blockchain and not in a specific agency.

[POC in python](https://github.com/jakubrog/car-sharing-blockchain)


## Skill verification system

Create a system where users are rewared for anonymously verify a skill that someone claims. The user can attach a proof of this claim.

[Example](https://github.com/jaygpt/Skillcheck)


## Fake product identification system

Use immutability (non destructive) strength of blockchain to keep track of product tracability, allow transfer of ownership of a product over decades from now.

[Example using java](https://github.com/kylelobo/AuthentiFi)