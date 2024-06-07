# Together Contract

This Solidity program is a simple token contract that demonstrates the basic syntax and functionality of the Solidity programming language. The purpose of this program is to serve as a starting point for those who are new to Solidity and want to get a feel for how it works.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract implements a token system with minting and burning functionalities. It includes the following features:

- **Token Name**: EcoToken
- **Token Abbreviation**: ET
- **Total Supply**: Tracks the total number of tokens in existence.

This program serves as a simple and straightforward introduction to Solidity programming and can be used as a stepping stone for more complex projects in the future.

## Getting Started

### Executing the Program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at [Remix Ethereum IDE](https://remix.ethereum.org/).

1. **Create a New File**:
   - Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar.
   - Save the file with a `.sol` extension (e.g., `Together.sol`).
   - Copy and paste the following code into the file:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;

contract Together {
    string public TokenName = "EcoToken";
    string public TokenAbbrv = "ET";
    uint public TotalSupply;

    mapping(address => uint) public balanceof;

    function mint(address Address, uint Value) public {
        TotalSupply += Value;
        uint balance;
        balance += Value;
        balanceof[Address] = balance;
        balance += Value;
    }

    function burn(address Address, uint Value) public {
        if (balanceof[Address] > Value) {
            TotalSupply -= Value;
            balanceof[Address] -= Value;
        }
    }
}
```

2. **Compile the Code**:
   - Click on the "Solidity Compiler" tab in the left-hand sidebar.
   - Make sure the "Compiler" option is set to "0.8.17" (or another compatible version).
   - Click on the "Compile Together.sol" button.

3. **Deploy the Contract**:
   - Once the code is compiled, click on the "Deploy & Run Transactions" tab in the left-hand sidebar.
   - Select the "Together" contract from the dropdown menu.
   - Click on the "Deploy" button.

4. **Interact with the Contract**:
   - Once the contract is deployed, you can interact with it by calling the `mint` and `burn` functions.
   - To mint tokens, input the address and value, then click on the "mint" button.
   - To burn tokens, input the address and value, then click on the "burn" button.

## Author

Divanshi
[DivanshiChauhan](https://github.com/DivanshiChauhan)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
