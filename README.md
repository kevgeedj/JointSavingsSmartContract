# Joint Savings Account

## Overview

Experience decentralized and secure interactions with our Ethereum smart contract application. Built on Solidity, the industry-standard programming language for blockchain, our application ensures trust through transparent, tamper-proof transactions. This Joint Savings smart contract application allows two users to manage a joint savings account, enabling them to deposit and withdraw funds. The solidity smart contract uses management functions to implement the financial features.

## What's inside

* Solidity `JointSavings` smart contract.

* A folder named `Execution_Results` that contains all images with the execution results. These images confirm that the deposit and withdrawal transactions, which are designed to test the `JointSavings` functionality in the Remix VM (London), works as expected.

## Compile and Deploy the Contract in Remix VM London
1. Compile the smart contract.

![](Execution_Results/(1) Joint Savings - Compile.png)

2. In the “Deploy & Run Transactions” pane, “Remix VM (London)” is selected as the environment.

3. Deployed my smart contract, and then confirmed that it successfully deployed.


## Interact with the Deployed Smart Contract

Now that the contract is deployed, it’s time to test its functionality.

To interact with my deployed smart contract, I have completed the following steps:

1. Used the `setAccounts` function to define the authorized Ethereum addresses that will be able to withdraw funds from the contract.



2. Tested the deposit functionality of the smart contract by sending the following amounts of ether. After each transaction, I have used the `contractBalance` function to verify that the funds were added to my contract:

* Transaction 1 - Send **1 ether** as wei.


* Transaction 2 - Send **10 ether** as wei.


* Transaction 3 - Send **5 ether.**


3. All funds have been successfully deposited into my contract. I have tested the contract’s withdrawal functionality by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`. After each transaction, I have used the `contractBalance` function to verify that the funds were withdrawn from my contract. I have also, use the `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.

* Withdrawal 1 - **5 ether** into `accountOne`
* `contractBalance`, `lastToWithdraw` and `lastWithdrawAmount` logs are shown. 


We can see that there is 11 ETH in wei left in the balance, last to withdraw is account 1, and withdraw amount was 5 ETH in wei.

* Withdrawal 2 - **10 ether** into `accountTwo`
* `contractBalance`, `lastToWithdraw` and `lastWithdrawAmount` logs are shown. 


We can see that there is 1 ETH in wei left in the balance, last to withdraw is account 2, and withdraw amount was 10 ETH in wei.
