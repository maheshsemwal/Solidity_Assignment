# MyToken Smart Contract

This Solidity smart contract implements a basic token system called MyToken. It allows for the creation (minting) and destruction (burning) of tokens, while ensuring that the balance of the address performing the burning operation is sufficient.

## Requirements

1. **Token Details**: The contract stores public variables to hold information about the token, including its name, abbreviation, and total supply.
2. **Balances Mapping**: There's a mapping of addresses to balances to keep track of the token balances of each address.
3. **Mint Function**: A function called `mint` is implemented, which takes an address and a value as parameters. It increases the total supply by the given value and increases the balance of the specified address by the same amount.
4. **Burn Function**: The contract includes a `burn` function, which works in the opposite way to the `mint` function. It takes an address and a value as parameters, and if the balance of the address is sufficient, it decreases the total supply by the specified value and deducts the same amount from the balance of the address.
5. **Safety Checks**: The `burn` function includes conditionals to ensure that the balance of the address performing the burn operation is greater than or equal to the amount being burned.

## Usage

1. **Deployment**: Deploy the contract on a compatible Ethereum Virtual Machine (EVM) blockchain network.
2. **Interacting with the Contract**: Once deployed, users can interact with the contract by calling its `mint` and `burn` functions. These functions allow for the creation and destruction of tokens, respectively.
3. **Token Details**: Users can query the public variables `tokenName`, `tokenAbbvr`, and `totalSupply` to retrieve information about the token.

## License

This smart contract is licensed under the [MIT License](https://opensource.org/licenses/MIT).
