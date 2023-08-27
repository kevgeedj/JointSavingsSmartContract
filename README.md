# Joint Savings Account

## Overview

Experience decentralized and secure interactions with our Ethereum smart contract application. Built on Solidity, the industry-standard programming language for blockchain, our application ensures trust through transparent, tamper-proof transactions. This Joint Savings smart contract application allows two users to manage a joint savings account, enabling them to deposit and withdraw funds. The solidity smart contract uses management functions to implement the financial features.

## What's inside

* Solidity `JointSavings` smart contract.

* A folder named `Execution_Results` that contains all images with the execution results. These images confirm that the deposit and withdrawal transactions, which are designed to test the `JointSavings` functionality in the Remix VM (London), works as expected.

## Compile and Deploy the Contract in Remix VM London
1. Compile the smart contract.

   ![(1) Joint Savings - Compile](https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/82beb854-1706-4cc1-b2b9-a502e917492e)

2. In the “Deploy & Run Transactions” pane, “Remix VM (London)” is selected as the environment.

3. Deployed my smart contract, and then confirmed that it successfully deployed.
 
    <img width="800" alt="(2) Joint Savings - Deployed" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/3b7018ee-2570-40f7-8f74-bf3c98d71ee5">

## Interact with the Deployed Smart Contract

Now that the contract is deployed, it’s time to test its functionality.

To interact with my deployed smart contract, I have completed the following steps:

1. Used the `setAccounts` function to define the authorized Ethereum addresses that will be able to withdraw funds from the contract.

    <img width="800" alt="(3) Joint Savings - Set Account" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/959628b9-877f-43c6-a05a-caf29c373194">

2. Tested the deposit functionality of the smart contract by sending the following amounts of ether. After each transaction, I have used the `contractBalance` function to verify that the funds were added to my contract:

* Transaction 1 - Send **1 ether** as wei.

  <img width="800" alt="(4) Joint Savings - 1 ether" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/44865594-aef7-4859-a298-311e074eed08">

* Transaction 2 - Send **10 ether** as wei.
  
  <img width="800" alt="(5) Joint Savings - 10 ether" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/19926da7-e90a-4b9a-8bd8-7e933e75fce0">


* Transaction 3 - Send **5 ether.**

    <img width="800" alt="(6) Joint Savings - 5 ether" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/ec100caa-d335-4d30-940d-526243c0c97b">


3. All funds have been successfully deposited into my contract. I have tested the contract’s withdrawal functionality by withdrawing 5 ether into `accountOne` and 10 ether into `accountTwo`. After each transaction, I have used the `contractBalance` function to verify that the funds were withdrawn from my contract. I have also, use the `lastToWithdraw` and `lastWithdrawAmount` functions to verify that the address and amount were correct.

* Withdrawal 1 - **5 ether** into `accountOne`
* `contractBalance`, `lastToWithdraw` and `lastWithdrawAmount` logs are shown. 

    <img width="800" alt="(7) Joint Savings - Withdraw 5 Ether" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/83282161-5176-4923-a4cc-5944b96f2347">


We can see that there is 11 ETH in wei left in the balance, last to withdraw is account 1, and withdraw amount was 5 ETH in wei.

* Withdrawal 2 - **10 ether** into `accountTwo`
* `contractBalance`, `lastToWithdraw` and `lastWithdrawAmount` logs are shown. 

    <img width="800" alt="(8) Joint Savings - Withdraw 10 Ether" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/caa9d7b4-f778-451b-bd5c-79cba9578220">

We can see that there is 1 ETH in wei left in the balance, last to withdraw is account 2, and withdraw amount was 10 ETH in wei.

* LastoToWithdraw and LastWithdrawAmount functions are used to verify that the address and amount were correct.

     <img width="800" alt="(9) Joint Savings - LastToWithdraw" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/5664da5a-dd0c-42cd-98ea-444d7faf5e87">
    <img width="800" alt="(10) Joint Savings - LastWithdraw" src="https://github.com/kevgeedj/JointSavingsSmartContract1/assets/128102960/4d897917-0383-4444-8777-fe5427c914c5">
