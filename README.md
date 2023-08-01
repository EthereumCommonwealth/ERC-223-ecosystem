# Call to action: we are building safer ecosystem for Ethereum tokens

The repo is created to coordinate the efforts of pushing ERC-223 adoption. We believe that Ethereum needs secure token standards and ERC-20 is not the best candidate for this role.

ERC-20 is designed in a way that it's direct transactions can not be handled by the recipient - which means there is no way to handle user mistakes or any transaction errors. Error handling is a critical part for a secure digital asset standard and ERC-223 solves this problem.

## Why ERC-223?

ERC-223 is to make token simple and transaction execution straightforward. There is already one asset in the Ethereum network that meets all security requirements and has existed since the very foundation of the network - ether, the native currency of Ethereum chain. ERC-223 makes tokens behave similar to ethere.

We can compare existing tokens and crypto assets. There are three types of transactions:

- Push transactions (sender initiates the transfer, recipient is notified)
- Pull transactions (recipient initiates the transfer if allowed)
- Unhandled transactions (recipient initiates the transfer without notifying the recipient)

| Transaction type  | ERC-223    |  ERC-20    |
| ------------- | ------------- | ------------- |
| Push tx       | +             | -             |
| Pull tx       | -             | +             |
| Unhandled     | -             | +             |
