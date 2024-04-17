#EVM SUBNET

## Avalanche Subnets: ERC20 Token and Vault Deployment Guide

Welcome to the Avalanche Subnets repository, where you can find guides and tools for deploying ERC20 tokens and a secure vault contract on an Avalanche EVM Subnet using the Remix IDE.

## Overview

This repository contains two Solidity smart contracts:
- `ERC20.sol`: Implements a basic ERC-20 token with functionalities such as transfer, approve, mint, and burn.
- `Vault.sol`: Provides a secure storage mechanism for the ERC-20 tokens, allowing users to deposit and withdraw tokens while managing supply and account balances.

## Getting Started

### Prerequisites

- Install [Remix IDE](https://remix.ethereum.org) on your web browser for Solidity development.
- Ensure you have Metamask installed in your browser to interact with the Ethereum blockchain.
- Familiarity with Ethereum smart contract development is recommended.

### Deployment Steps

#### Set Up Your Environment

1. **Open Remix IDE**:
   - Launch your web browser and navigate to [Remix IDE](https://remix.ethereum.org).

2. **Import Contracts**:
   - Create new files in Remix named `ERC20.sol` and `Vault.sol`.
   - Copy and paste the contents of the respective smart contracts into these files.

3. **Compile Contracts**:
   - Access the "Solidity" tab in Remix.
   - Select a compatible compiler version (e.g., ^0.8.17).
   - Click "Compile" to compile both contracts.

#### Deploy Contracts on Avalanche EVM Subnet

1. **Deploy Your EVM Subnet Using the Avalanche CLI**:
   - Follow the provided instructions in the Avalanche CLI documentation to set up your EVM subnet.

2. **Add Your Subnet to Metamask**:
   - Open Metamask, navigate to Networks, and select 'Custom RPC'.
   - Enter the details of your EVM subnet (RPC URL, Chain ID, Symbol, Block Explorer URL).

3. **Ensure Network Selection in Metamask**:
   - Make sure the newly added subnet is your active network in Metamask.

4. **Connect Remix to Metamask**:
   - Set "Injected Web3" as the environment in Remix to link it with Metamask.

5. **Deploy the ERC20 Token Contract**:
   - Under the "Deploy & Run Transactions" tab, select `ERC20.sol`.
   - Click "Deploy" to deploy the token contract on the subnet.

6. **Deploy the Vault Contract**:
   - Copy the address of the deployed ERC20 token contract.
   - Select `Vault.sol` and input the ERC20 token address as the constructor parameter.
   - Click "Deploy" to deploy the vault.

### Interacting with the Contracts

Once deployed, use Remix to interact with the smart contracts. You can manage tokens through the ERC20 interface and interact with the vault for deposit and withdrawal operations.

## Authors

- Harshgupta0081

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Additional Resources

- [Avalanche Documentation](https://docs.avax.network/)
- [Metamask Documentation](https://docs.metamask.io/)
- [Remix Documentation](https://docs.remix.ethereum.org/)

For troubleshooting and further assistance, refer to the official documentation or community forums. Enjoy building on the Avalanche EVM Subnet! 🚀
