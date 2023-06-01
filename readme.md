# Decentralized Escrow Application

This is an Escrow Dapp built with [Hardhat](https://hardhat.org/).

## Project Layout

There are three top-level folders:

1. `/app` - contains the front-end application
2. `/contracts` - contains the solidity contract
3. `/tests` - contains tests for the solidity contract

## Project brief description

This dApp is a simple application developed as part of the Alchemy University Dev. Bootcamp Solidity module. It allows a Depositor, which can be an individual or an entity, to make a deposit into an Escrow account and define a Beneficiary and an Arbitror.

The deposited amount is securely stored on the blockchain. To unlock or transfer the funds to the Beneficiary, the Arbitror, who acts as an intermediary or trusted third party, can approve the transaction using their wallet.

The dApp is implemented using Hardhat and runs on the local blockchain provided by Hardhat. The front-end interface is built using React.

## Setup - Dependencies and compile

Install dependencies in the top-level directory with `npm install`.

After you have installed hardhat locally, you can use commands to test and compile the contracts, among other things. To learn more about these commands run `npx hardhat help`.

Compile the contracts using `npx hardhat compile`. The artifacts will be placed in the `/app` folder, which will make it available to the front-end. This path configuration can be found in the `hardhat.config.js` file.

## Setup - Run a Local Test Blockchain using hardhat

npx hardhat node

## Setup - Install Depositor, Arbiter and Beneficiary accounts on a Wallet (Metamask)

Import the private keys created by hardhat above

## Front-End

`cd` into the `/app` directory and run `npm install`

To run the front-end application run `npm start` from the `/app` directory. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

Enter the addresses for Arbiter and Beneficiary

Enter the amount to be stored on the Escrow Smart Contract

Make sure to use Deploy using the Depositor address

Then the transaction needs to be approved by the Arbiter. To do so, switch from Depositor to Arbiter and approve.

The page should show "It's been approved!"
