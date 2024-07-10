# Stabull Finance Token

## Overview

The Stabull Finance Token (STABUL) is a non-upgradeable, non-pausable, and non-restrictable ERC677 compatible token with burning and minting capabilities. This token is designed to function across multiple chains, including Ethereum and Polygon.

### Token Specifications

- **Name:** Stabull Finance
- **Symbol:** STABUL
- **Decimals:** 18
- **Total Supply:** 10 million
- **Chains:** Ethereum, Polygon

## Features

1. **Minting and Burning:**
   - The contract allows certain addresses to mint and burn tokens.
   - Minting and burning access can be granted and revoked by the contract owner.

2. **Role Management:**
   - The contract uses `EnumerableSet` to manage the list of addresses that have minting and burning permissions.
   - Emits events when minting and burning access is granted or revoked.

3. **ERC677 Compatibility:**
   - Implements the ERC677 token standard, allowing tokens to be transferred and called in a single transaction.

4. **OpenZeppelin Integration:**
   - Utilizes OpenZeppelin's ERC20Burnable and other utility libraries for secure and efficient token operations.

## Usage

The Stabull Finance Token (STABUL) is primarily used to distribute rewards to holders of liquidity provider (LP) tokens of the Stabull DEX platform. Users who add liquidity to the Stabull DEX will receive LP tokens, which they can stake to earn STABUL tokens as rewards. This incentivizes users to provide liquidity and ensures the stability and liquidity of the Stabull DEX platform.

### Example Workflow

1. **Provide Liquidity:**
   - Users add liquidity to the Stabull DEX platform.
   - In return, they receive LP tokens representing their share of the liquidity pool.

2. **Stake LP Tokens:**
   - Users can stake their LP tokens on the Stabull platform.
   - By staking LP tokens, users are eligible to earn STABUL tokens as rewards.

3. **Earn STABUL Tokens:**
   - Staked LP tokens accrue rewards over time in the form of STABUL tokens.
   - Users can claim their STABUL tokens as rewards for providing liquidity to the platform.

## Installation

To install and test the contract using Foundry, follow these steps:

1. **Install Foundry:**

   Follow the instructions on the [Foundry GitHub repository](https://github.com/gakonst/foundry) to install Foundry.

2. **Clone the Repository:**

   ```sh
   git clone https://github.com/your-repo/stabull-finance.git
   cd stabull-finance
