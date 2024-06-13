# ETHAssessment

This repository houses a Solidity smart contract for the token called MyToken. It features the ability to mint and burn tokens, and maintains records of the total supply and individual balances. This contract acts as a base for managing tokens on the Ethereum blockchain.

### Process

**Contract Initialization**

The contract starts with the name "MyToken" and launches a token on the Ethereum blockchain. It establishes initial values for public variables like ```tokenName```, ```tokenAbbrv```, and ```totalSupply```. Additionally, a mapping called ```balances``` is set up to link addresses with their respective token balances.

**Minting Tokens**

The ```mint``` function allows the creation of new tokens to be assigned to a specific address. When invoked, it requires two parameters: ```_address``` (the recipient's address) and ```_value``` (the number of tokens to mint). The function increases the total supply by ```_value``` and adds ```_value``` to the ```_address``` balance in the ```balances``` mapping.

**Burning Tokens**

The ```burn``` function enables the removal of tokens from circulation, thereby reducing an address's balance. It takes two parameters: ```_address``` (the token owner's address) and ```_value``` (the number of tokens to burn). The function first verifies that ```_address``` has a balance that is equal or more than ```_value```. If so, the total supply is reduced by ```_value```, and ```_value``` is deducted from the ```_address``` balance in the ```balances``` mapping. Otherwise, the function does not run.

## Authors

Contributors names and contact info

Louella Amor Ramos 
Email: louellaaramos2714@gmail.com
