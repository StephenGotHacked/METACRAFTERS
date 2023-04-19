# ETH Proof: Beginner Course(Final Assessment Project)

Eth Proof: Beginner Course Project is creating a simple but useful program for NFTs, Minting and Burning of tokens

## Description

An in-depth paragraph about your project and overview of use.

## Getting Started

### Executing program

* How to run the program
* Step-by-step bullets

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

## Authors

Creator: Stephen David Q. Condino 

Email: 8215348@ntc.edu.ph

Facebook: https://www.facebook.com/profile.php?id=100010312052822

Contact Number: 09651272083


## License

This project is licensed under the MIT License - see the LICENSE.md file for details
