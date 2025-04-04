# Dash Mon\[k\]ey
> View the [gitcoin grant](https://explorer.gitcoin.co/#/projects/0x04f949b4b358adc1a89ab3d4179110fc57a095923dbee573cc7f6502c0a5144f) for more details

Dash Mon[k]ey is an onchain tamagotchi that embodies your financial health. Inspired by behavioral science and the 90s craze of virtual pets, this project externalizes your “monkey brain” to help you visualize your habits and correct them — before it’s too late.

## Project Timeline
> current :: [ai blueprints](#ai-blueprints)

This project is highly ambitious and quite complex and such, is being built over multiple hackathons. Please see the specific hackathons / sprints below to adjudge what stage the project currently is in.

### Preliminary Work

Prior to 2025, Dash Mon[k]ey had only been in the conceptual stage. The project was born out of Account Abstraction from the [IndiaStack](https://en.wikipedia.org/wiki/India_Stack), since that feature by the protocol let an application query all financial data of a user, with consent. This was in 2021. However, the project was put on the back burner since IndiaStack existed only in India and the country is not very crypto friendly.

### AI Bootcamp

In Summer of 2024, I participated in an AI Bootcamp where I explored the idea of receipt tracking via OCR, deployed locally. This became the foundations of the pivot in the project. While originally the idea was to use IndiaStack, now, the idea is to require users to submit their receipts and statements and perform OCR on it to store to the database. Of course, everything remains local and nothing of importance is sent over the network. You can see the exploratory repository here — https://github.com/thisispalash/finance-tracker-localhost

In another AI bootcamp in early February 2025, I pitched the project as something I would like to pursue at some point in the future. However, the presentation received an overwhelming response, which made me think that the time to build it out is now! Here is the pitch at the bootcamp,

![![monkey-pitch](https://img.youtube.com/vi/6S_fSh8ldoo/0.jpg)](https://youtu.be/6S_fSh8ldoo?si=94Yi3AjZNUwkvbA2)


### Modular DeFi Hackathon

In February 2025, during ETHDenver, I participated in a side event hackathon by Encode Club, where the feasibility of the copytrading platform was tested. The project even won a couple of prizes! The contract structure and how the actual copytrading would function onchain was discovered, experimented upon, and finalized here. You can see how the contracts function here — https://github.com/thisispalash/monkey-contracts

Another discovery made over the course of this hackathon was that of [Envio HyperIndex](https://docs.envio.dev/docs/HyperIndex/overview). This amazing product is going to solve a lot of technical difficulties with the project, and let my users run the app locally on their machines, thereby enabling absolute privacy! You can see explorations with the product here — https://github.com/thisispalash/monkey-node

Finally, here's the demo video for the project built over the hackathon (ie, the copytading feature),

![![monkey-demo](https://img.youtube.com/vi/MReSUmdkHT0/0.jpg)](https://youtu.be/MReSUmdkHT0?si=O9txnBC9lScr_mTx)

### EthereumSF

In March 2025, I participated in EthereumSF, a week long build event in San Francisco. The hackathon was a failure, and nothing of substance was created, but a discovery of Modular Smart Accounts ([ERC 7579](https://eip.tools/eip/7579)) and Sub Accounts ([ERC 7895](https://eip.tools/eip/7895)) was made. Now the app users can have seamless smart wallets onchain, without having to worry about web3 in the least!

### Trifecta Agents

At the end of March 2025, there was a weekend hackathon on very short notice. Though not a lot was completed, what was figured out was how to enable mobile. The project requires users to take pictures of their receipts, which is unlikely to happen if they are expected to first take pictures of the receipt, send them to their computer, and then upload them. Hence, a mobile application is an absolute must. However, mobile applications cannot be heavy enough to perform on device OCR and receipt images cannot be encrypted or sent over the network. Additionally, web3 does not play well with mobile, so desktop has to be the main device.

So, a compromise is made here with the user being expected to run a docker container on their desktop, through which they can log in on their mobile. You can see some of the explorations here, though you may have to change the branch to see them — https://github.com/thisispalash/monkey-front/tree/1-mobile

### AI Blueprints

This hackathon is by Filecoin and the goal here is to create a decentralized OCR network using Filecoin's properties and features. This hackathon is ongoing, and you can track progress here — https://github.com/thisispalash/encode-ai-blueprints

### Hashgraph Agents

This is an upcoming hackathon where the ElizaOS integration will be built out. The idea here is that Eliza is a complete representation of the user, informed by their financial habits, and their conversations with the agent. Another exploration is to use Eliza as an interface for the project, as opposed to a traditional UI based approach.

### Base Batch

This is another upcoming hackathon where the plan is to build out the integration on Base. This means, logging with Coinbase Wallet, getting a Coinbase Smart Wallet, linking subaccounts, and potentially creating a mechanism to simulate a savings account using USDC.

### Sui Overflow

This is another month long hacakthon where the plan is to utilize Sui and Walrus to test out an alternative to Filecoin for the data layer.

## Repositories

Current repositories, (more soon)

| | Repository | Description |
| --- | :---: | --- |
| landing | [`thisispalash/dashmonkey`](https://github.com/thisispalash/dashmonkey) | The primary entrypoint to the application |
| contracts | [`sliver-labs/monkey-forge`](https://github.com/sliver-labs/monkey-forge) | All contracts |

### Archived Repositories

- [`thisispalash/monkey-front`](https://github.com/thisispalash/monkey-front/tree/1-mobile) Partial frontend built over ETHGlobal Trifecta. Focus was on mobile integration here.
- [`thisispalash/monkey-web`](https://github.com/thisispalash/monkey-web) Potential frontend for the copytrading network. Built during Encode's Modular DeFi Hackathon.
- [`thisispalash/monkey-contracts`](https://github.com/thisispalash/monkey-contracts) Contracts created over Encode's Modular DeFi Hackathon.
- [`thisispalash/monkey-node`](https://github.com/thisispalash/monkey-node) Backend code that every user is expected to run on their machine. Created over Encode's Modular DeFi Hackathon.
- [`thisispalash/finance-tracker-localhost`](https://github.com/thisispalash/finance-tracker-localhost) Explorations with OCR using [`tesseract-ocr`](https://github.com/tesseract-ocr/tesseract)