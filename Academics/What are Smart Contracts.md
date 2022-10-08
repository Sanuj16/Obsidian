# What are Smart Contracts?
## Smart Contract Definition:

A smart contract is a self-executing digital agreement that enables two or more parties to exchange money, property, shares, or anything of value in a transparent, conflict-free way while avoiding the need for a third party.

For ex : You want to buy a deed to a newly available real estate. With the help of smart contracts you can simply give the asked price to the seller and the deed to the real estate is sent to your account automatically.

Smart contract keep in check all the condtions that need to be satisfied. Smart contracts define the rules and penalties and can also automatically enforce those obligations.

Smart contracts remove the need for an intermediary/third-party to negotiate between client and provider. When both sides agree to the terms and conditions set by the contracts, the program automatically executes. The program is verified and enforced by the blockchain network.

## Some of the use cases for Smart Contracts:
1.  Real Estate : A decentralised way to buy/sell/rent estates will cut the total cost.
2.  Healthcare : Receipts and health records could be sent as a proof-of-delivery. Such contracts can also supervise drugs and help manage healthcare supplies.
3.  Government : Smart Contracts could be used in voting system.
4.  NFTs
5.  DeFi Applications

## Some of the key features of Smart Contracts are :
1. Autonomy: Smart contracts discard any middlemen needed to perform any transaction.
2.  Trust: Smart contracts are only performed when certain conditions are met and its also checks whether both parties have held their side of the bargain. Then and only then does the contract perform its total actions.
3.  Backup : Smart contract can be shared over a blockchain.
4.  Savings: The removal of any third party reduces the total cost of the trasaction that needs to be performed.
5.  Accuracy: Smart contracts are scarily accurate as they perform a particular set of instructions provided in its code.

One of the biggest drawback of Smart Contracts is that they are very difficult to reconfigure once they have been deployed. Suppose you have deployed a smart contract on a blockchain and realize that you have written the wrong code, the smart contract will execute no matter what. This can result in many complications.

Now, after a brief introduction of smart contracts, let us see how these contracts are actually implemented. The languages these contracts use are mainly dependent on the blockchain they are implemented on. Mainly on ethereum, smart contracts are written in solidity.

## Following is an example of code written in solidity:

```js
// SPDX-License-Identifier: GPL-3.0

pragma solidity >=0.4.16 <0.9.0;

contract SimpleStorage {

    uint storedData;

    function set(uint x) public {

        storedData = x;

    }

    function get() public view returns (uint) {

        return storedData;

    }

}
```


When a contract is created, its constructor is executed once. Only one contructor can be declared, i.e., oveloading is not supported. Once the constructor is executed, the final code of the contract is stored on the blockchain.

The structure of a contract basically comprise state variables, functions, function modifiers, events, errors, struct types and enum types.

You can further delve into more detailed description of the solidity language in its official page : < docs.soliditylang.org>

## Smart contracts can also be run on various other platforms like:

1.  The bitcoin blockchain : However, the scope of the smart contracts written using Bitcoin's stack based byte-scripting language is very limited. Major changes would need to be made in order for proper functioning of various advanced smart contracts.
2.  NXT : This is an open source blockchain platform that relies entirely on a proof-of-stake consensus protocol. The only smart contracts can be used on this platform are the pre-existing templates.
3.  Ethereum : This is the first blockchain platform for developing smart contracts. It supports advanced and customized smart contracts.
4.  Hyperledger Fabric : This is an enterprise grade platform. Organisations need to join in through membership. Hyperledger Fabric supports multiple languages like Java, Go and Javascript.

 ### Now that we have made ourselves familiar with the basics of smart contracts, you can try to create a basic smart contract on ethereum.

1.  Create an account on ethereum
2.  Go into the contract tab after logging in and paste your contract code. You can also borrow your code from the various tutorials on ethereum.org/token.
3.  Select the contructor function and fill the contructor parameters and deploy your contract.

![[Pasted image 20221003200530.png]]

4.  You can now use this contract by choosing the function which you want to use and  addressing this contract to some other account. The actions would be performed according to the function when certain conditions are met.


---
# References
1. [What Are Smart Contracts? [Ultimate Beginner’s Guide to Smart Contracts]](https://blockgeeks.com/guides/smart-contracts/)
2. [Introduction to Smart Contracts — Solidity 0.8.18 documentation](https://docs.soliditylang.org/en/develop/introduction-to-smart-contracts.html)
3. [(PDF) Survey on Blockchain-Based Smart Contracts: Technical Aspects and Future Research](https://www.researchgate.net/publication/350018207_Survey_on_Blockchain-Based_Smart_Contracts_Technical_Aspects_and_Future_Research)

---
Date: 03-10-2022
Time: 19:56
Status: #note
Tags: #finalyearproject 