# ETH Proof: Beginner Course(Final Assessment Project)

Eth Proof: Beginner Course Project is creating a simple but useful program for NFTs, Minting and Burning of tokens

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract have two different function that will shown how Minting and Burning of tokens is been processes. This program serves as a simple Minting and Burning Token's to Solidity programming, and can be used as a stepping stone for more complex projects in the future.

## Getting Started

### Executing program

* To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

**STEP BY STEP HOW TO RUN THIS CODE**
* You can easily get a copy address from Remix: Etherium IDE built in wallet address in **_Deploy & Run Transactions_** you will see copy button from account and you can easily get a address

> if you click the **_TokenName_** and **_TokenAbbrv_** it will show the declared value because that's a type of State variables 

> if you **_TotalSupply_** and **_Balances_** without minting a value it will show a default value **0** 

* After you have the address please input the address and value for Minting and click **_Transact_** you can check it in **_TotalSupply_** and **_Balances_** if it success run you can check your Terminal also.

* If you have a Value in Balances and TotalSupply now you can use the Burning section, a burning function have a condition which is Burning section will run if the value of TotalSupply and Balances is Greater than or Equal in the value of Burning Value

* Every Mint or Burn of your value will easily update it

```javascript
//SPDX-License-Identifier: MIT
  pragma solidity ^0.8.18;
        
        contract Metacrafters{

            string public TokenName = "Coindino";
            string public TokenAbbrv = "COD";
            uint public TotalSupply;

                    mapping (address => uint) public Balances;

                function Minting (address Address, uint Value)public{
                        TotalSupply += Value;
                        Balances[Address] += Value;
                }

                function Burning (address Address, uint Value)public{
                       while(Balances[Address] >= Value){
                                TotalSupply -= Value;
                                Balances[Address] -= Value;
                            break;
                       }
                }
         }
```

## Help

Be aware and alert for some errors: 

* You will notice if your code have an error check on the upper right side of your screen you will your mini-minimize entire code there that have a red lines, blue lines mean you are in that lines and red lines means error.

* You will see a Red Exclamation Mark in that line so you will notice that there some errors

* Check your File name if its red

* Don't forget to count and check some valuable symbols
* **_{  }_** , **_[ ]_** , **_( )_** , **_;_**


## Authors

Creator: Stephen David Q. Condino 

Email: 8215348@ntc.edu.ph

Facebook: https://www.facebook.com/profile.php?id=100010312052822

Contact Number: 09651272083


## License

This project is licensed under the MIT License - see the LICENSE.md file for details
