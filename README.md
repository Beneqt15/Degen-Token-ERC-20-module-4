# Degen-Token-ERC-20-module-4
# GamingCoin ERC20 Token

GamingCoin is an ERC20 token designed for use in a gaming ecosystem. It allows players to purchase in-game items, earn experience points, and progress through different player ranks.

## Contract Deployment

To deploy the `GamingCoin` contract, you'll need to have a compatible Ethereum client and a tool like Remix, Truffle, or Hardhat.

1. Install the required dependencies, including the OpenZeppelin contracts.
2. Copy the `GamingCoin` contract code into your project.
3. Compile the contract.
4. Deploy the contract to the desired Ethereum network (e.g., mainnet, testnet, or local development network).

Note: During deployment, the contract constructor will set the initial item prices and the token name ("Gaming Coin") and symbol ("GCN").

## Contract Functionality

### Token Minting

The `mintTokens` function allows the contract owner to mint new tokens and distribute them to a specified address. Only the contract owner can call this function.

```solidity
function mintTokens(address _to, uint256 _amount) external onlyOwner { ... }
