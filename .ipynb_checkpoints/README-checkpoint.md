# Solidity_Contracts

This project uses the programming language Solidity to write a smart contract to split profits between three employees and returns the remainder to the HR account if it is not divisible by three.  It utilitizes Ganache as a local host network to run a simulated Ethereum blockchain and MetaMask a cryptocurrency wallet to interact with the Ethereum blockchain to track transactions and balances.

## Technologies
This use project uses Solidity v.0.5.5 to write the contracts within Remix, an interactive Ethereum IDE.  Ganache is used to run the blockchain and Metamask is used to interact with the Blockchain. The operating system is Windows 10. 

## Libraries Uses
    Solidity 0.5.0 - this is the main language used to code the smart contract
    
## Installation Guide
Remix IDE is accessible through your preferred web browser and does not require an installation.
To install Ganache, download Ganache from https://www.trufflesuite.com/ganache for your current operating system.  Following the download, run the installer. After Ganache is successfully installed, it is time to set up a network to run the blockchain.  Create a name for the test network under WORKSPACE NAME.  
* Set the server settings to:
* HOSTNAME = 127.0.0.1 
* PORT NUMBER = 8545 
* AUTOMINE = ON

After the server is set up, set up the ACCOUNTS & KEYS:
* ACCOUNT DEFAULT BALANCE = 100
* TOTAL ACCOUNTS TO GENERATE = 10
* AUTOGENERATE HD MNDMONIC = YOUR MNEMONIC PHRASE(PASSWORD)

Next install the Metamask browser extension: 
* Download Metamask for your brower and run the install
* Hit the get started button, and import the wallet to run your blockchain
* Use the 12 word mnemonic that you used for your local wallet and click all done to see the balances in your accouont.

To import an account to Metamask:
* click the circle at the top right and copy the address from your Ganache accounts into the new account address input.  

## Examples
![](./Images/contract_deploy.JPG)
![](./Images/blocktransaction.JPG) 
![](./Images/account_transaction.JPG) 

## Usage

To use this contract: 
First make sure that Metamask is connected to the LocalHost 8545 Network. 
Then complile the contract using the "Compile AssociateProfitSplitter.sol". Next, goto the next icon below to begin deployment. Make sure that the environment is InjectedWeb3.  Click the dropdown menu next to "DEPLOY" and input the three account numbers that you are going to use to receieve the transaction.  PLace a number in the value column next to wei and click the transact button.  Use Metamask to confirm the gas fee and make sure that the contact is deployed.  Once the contract is deployed, click on the drop down menu next to that contract and click the deposit button.  Use Metamask to confirm the transaction and check the accounts via MetaMask to confirm the updated balances.  

## Contributors
Ryan Dibeler

ryandibeler@gmail.com

## License
MIT License

Copyright (c) [2021] [Ryan Dibeler]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
