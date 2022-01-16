## Selected Design Patterns

### 1. Inheritance and Interfaces
The Ownable contract is for access contro that provides a mechanism where there is an account (the owner in our case) that can be granted exclusive access to specific functions.
ERC-721 is a Non-Fungible Token (NFT) is used to identify something or someone in a unique way

### 2. Access Control Design Patterns
The use of Ownable to control access to the mintable/burnable NFT collection and the onlyOwner modifier in setBaseURI method

### 3. Optimizing Gas
Tried as much as possible to keep state change out of loops to optimize gas
