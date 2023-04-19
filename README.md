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

Any advise for common problems or issues.
command to run if program contains helper info


## Authors

Contributors names and contact info

ex. Dominique Pizzie
ex. [@DomPizzie](https://twitter.com/dompizzie)


## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details
