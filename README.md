# Call to action: we are building safer ecosystem for Ethereum tokens

The repo is created to coordinate the efforts of pushing ERC-223 adoption. We believe that Ethereum needs secure token standards and ERC-20 is not the best candidate for this role.

ERC-20 is designed in a way that it's direct transactions can not be handled by the recipient - which means there is no way to handle user mistakes or any transaction errors. Error handling is a critical part for a secure digital asset standard and ERC-223 solves this problem.

## Why ERC-223?

ERC-223 is to make token simple and transaction execution straightforward. There is already one asset in the Ethereum network that meets all security requirements and has existed since the very foundation of the network - ether, the native currency of Ethereum chain. ERC-223 makes tokens behave similar to ethere.

We can compare existing tokens and crypto assets. There are three types of transactions:

- Push transactions (sender initiates the transfer, recipient is notified)
- Pull transactions (recipient initiates the transfer if allowed)
- Unhandled transactions (recipient initiates the transfer without notifying the recipient)

It should be noted that if your standard implements one way of transaction handling (either push or pull transactions) then there is no reason to support another. Credit cards are good example of pull transactions - they do work, but definitely not in trustless decentralized systems. Pull transactions are not suitable for a class of decentralized assets like tokens and these are potentially risky. Unhandled transactions are straight up insecure.

A good, **secure** token standard must implement push transactions and remove pull & unhandled transactions for the safety of users in a decentralized trustless environment.

| Transaction type  | [ERC-223](https://eips.ethereum.org/EIPS/eip-223)   |  Ether    | [ERC-20](https://eips.ethereum.org/EIPS/eip-20)             | [ERC-721 (NFT)](https://eips.ethereum.org/EIPS/eip-721) | [ERC-777](https://eips.ethereum.org/EIPS/eip-777) | [ERC-1155](https://eips.ethereum.org/EIPS/eip-1155) | [ERC-1363](https://eips.ethereum.org/EIPS/eip-1363) | [EOS C++ token](https://github.com/EOSIO/eosio.contracts/blob/master/contracts/eosio.token/src/eosio.token.cpp) |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Push tx       | +             | +             | - | + | + | + | + | + |
| Pull tx   (risky)    | -             | -             | + | + | + | + | + | - |
| Unhandled  (insecure)   | -             | -             | + | - | + | + | + | - |

There are classes of assets that behave properly and are not prone to the problems of ERC-20 standard: most notably native currencies (ether, EOS and EOS tokens). Our goal is to make Ethereum tokens similarly secure.
