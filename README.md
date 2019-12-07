# Decentralized Finance Automation MetaMask Snap

## User Story

Over the weekend I sent my long-time buddy ETH. He shouldn't need to learn about InstaDapp, Smart Wallets, Decentralized Exchanges, Compound, etc.... to leverage his money. That's silly and doesn't scale.

## Technical Requirements

- Application Installation Page
- MetaMask Snap
- Automated Decentralized Finance Transactions
- User Difficulty Mode Selection
- Deadman Switch
- Backup Service for Trust Anchor to Recover Funds (Strech Goal)

## Resources

When you arrive at a fork in the road, take it.

- DeFi Zap https://defizap.com/
- DeFi Recipes https://github.com/dexlab-io/fvm
- Smart Wallet https://medium.com/@ChrisLundkvist/exploring-simpler-ethereum-multisig-contracts-b71020c19037
- Example dApp https://instadapp.io/

## Project Specification

To qualify for any bounties please review the project specification document. If any questions/concerns arise please open an issue or contact @kamescg directly.

### Application

To install the Snap a user will visit a safe, trusted website. When installing the user might select between 3 different choices: Easy, Intermediate and Advanced.

### Metamask Snap

The MetaMask Snap will help everyday users avoid the technical overhead of learning Ethereum and Decentralized Finance to participate. The focus should be on simplicity. The less user actions, after installation, the better. Simple. Elegant.

- Batch signing using application/plugin specific private key.
- Deadman swtich to protect user from losing funds.

### Automated Transaction Signing

This is the technically interesting part. And is very open for interpreation. In other words, to accomplish an automated decentralized finance snap can probably be achieved multiple ways - all with different pros/cons.

# Engineering Topics

## Plugin Architecture

Due to how Snaps are currently built, to accomplish this it might require 3 separate snaps to cater to the unique user preferences.

The preferences should balance the User's risk appetite and also familarity with blockchain terms. In other words, when a User select's a difficulty level, then the user should also be asked "How much are you willing to risk?" and "How familiar are you with Ethereum/blockchain terminology?"

After that everything needs to be very low touchpoint. The less the user has to do now. The better.

No more user actions after this installation is optimal. Simple. Elegant.

## Private Key Approach

The first way to build the Snap might be to do it with only private keys.

This route requires figuring out a clever way to ensure automatic, atomic, and failure resistent transactions. I have a feeling this way will require a lot of upfront work, custom javascript, and clever usage of snaps. The DEXWallet team has convinced me a method for achieving such an approach is ready-ish.

The recipes can be accessed via @Alexintosh - if you're lucky ;)

https://twitter.com/Alexintosh/status/1202111497637380097

## Smart Wallet/Bank Approach

The second method might be to utilize a Smart Wallet.

A Smart Wallet/Bank would alleviate the private key orchestration concerns, and allow for several novel methods to automate a user's decentralized bank.

The smart wallet/bank could be contolled via multiple methods:

- Signatures
- Transactions
- MetaTransactions
- Trust Anchor Protocol w/ Decentralized Public Key Infrastruvture

However.... such an approach introduces an entirely new set of security problems, user experiences issues, possible centralization and other unwanted side-effects. I'm of the opinion those choices will have to be made eventually and we should just do it now.

The benefits of a multiple battled tested smart wallets/banks that can help coordinate multiple cross-chain protocols and compose new decentralized finance features as they emerge seem worth the risk.
