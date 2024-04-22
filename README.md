#### Module 20 Challenge: Joint Savings Account
##### Anvitha Chaluvadi

<p align="center">
<img src = Images/joint-savings.gif width =40% height 30%=/>
</p>

### Background

A fintech startup company has recently hired you. This company is disrupting the finance industry with its own cross-border, Ethereum-compatible blockchain that connects financial institutions. Currently, the team is building smart contracts to automate many of the institutions’ financial processes and features, such as hosting joint savings accounts.

To automate the creation of joint savings accounts, you’ll create a Solidity smart contract that accepts two user addresses. These addresses will be able to control a joint savings account. Your smart contract will use ether management functions to implement a financial institution’s requirements for providing the features of the joint savings account. These features will consist of the ability to deposit and withdraw funds from the account.

### What You're Creating

* The completed Solidity `JointSavings` smart contract.

* A folder named `Execution_Results` that contains at least eight images. These images should confirm that the deposit and withdrawal transactions, which are designed to test the `JointSavings` functionality in the JavaScript VM, worked as expected.

### Joint Accounts Added to the Contract:

* Account 1: 0xd80BDbbe9757b6104F230f1C3f977511E6e8B5a0
* Account 2: 0xa0A630235747d11D58a1CED2d2F8df2114f158e0

<p align="center">
<img src = Images/Joint_Accounts.png width =60% height 30%=/>
</p>

### Execution Results:

**NOTE**: After each transaction, I'll check the contractBalance function to make sure funds were withdrawn. I'll also use lastToWithdraw and lastWithdrawAmount to confirm the address and amount.

#### Deposit 1 ETH - Transaction 1: Send 1 ether as wei

* To deposit 1 ETH, I needed to convert wei into ETH and then assign that number to the 'value' field
    * 1000000000000000000 wei = 1 Ether

    <p align="center">
    <img src = Execution_Results/Deposit_1.png width =90% height 30%=/>
    </p>

* Balance is 1 ETH

#### Deposit 10 ETH - Transaction 2: Send 10 ether as wei

* To deposit 1 ETH, I needed to convert wei into ETH and then assign that number to the 'value' field
    * 10000000000000000000 wei = 10 Ether

    <p align="center">
    <img src = Execution_Results/Deposit_10.png width =90% height 30%=/>
    </p>

* Balance is 11 ETH
    * 1 ETH + 10 ETH = 11 ETH

#### Deposit 5 ETH - Transaction 3: Send 5 ether

* I converted the value from wei to Ether and successfully set it to 5, then deposited it.

    <p align="center">
    <img src = Execution_Results/Deposit_5-pt1.png width =20% height 30%=/>
    </p>

    <p align="center">
    <img src = Execution_Results/Deposit_5-pt2.png width =90% height 30%=/>
    </p>

* Balance is 16 ETH
    * 11 ETH + 5 ETH = 11 ETH

#### Withdraw 5 ETH - Withdrawing 5 ether into accountOne

* To withdraw 5 ETH into accountOne, I had to convert ETH into wei
    * 5 ETH = 5000000000000000000 wei

<p align="center">
<img src = Execution_Results/Withdraw_5.png width =90% height 30%=/>
</p>

* Balance is 11 ETH
    * 16 ETH - 5 ETH = 11 ETH

* 

#### Withdraw 10 ETH - Withdrawing 10 ether into accountTwo

* To withdraw 10 ETH into accountOne, I had to convert ETH into wei
    * 10 ETH = 10000000000000000000 wei

<p align="center">
<img src = Execution_Results/Withdraw_10.png width =90% height 30%=/>
</p> 

* Balance is 1 ETH
    * 11 ETH - 10 ETH = 1 ETH

