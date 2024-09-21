# Contributing to LITRBULL Smart Contract

Thank you for your interest in contributing to the LITRBULL smart contract for the TON blockchain! This document outlines the contribution process and guidelines to ensure a smooth workflow for everyone involved.

## Getting Started

1. **Fork the repository**  
   Create your own fork of the repository by clicking the "Fork" button at the top-right corner of the project page.

2. **Clone the repository**  
   Once you've forked the repository, clone your fork locally:
   ```
   git clone https://github.com/your-username/litr-contract.git
   ```
   Navigate to the project directory:
   ```
   cd litr-contract
   ```

3. **Install dependencies**  
   Make sure you have the necessary tools to work with the TON blockchain. This may include:
   - [ton-cli](https://github.com/tonlabs/tonos-cli)
   - [func](https://github.com/ton-blockchain/ton/tree/master/crypto/func)
   - [fift](https://github.com/ton-blockchain/ton/tree/master/crypto/fift)

4. **Create a new branch**  
   Before you start making changes, create a new branch:
   ```
   git checkout -b your-feature-branch
   ```

## Writing and Testing Smart Contracts

- Smart contracts for TON are written in **FunC** or **Fift**. Please adhere to the following conventions:
  - Ensure proper formatting and readability of the contract code.
  - Use comments to explain the logic behind complex functions.
  - Follow TON best practices for security and efficiency.

### Testing

- **Unit Testing**: It is critical to test all changes in the smart contract. Use `ton-cli` to run local tests for your contract.
  - Write tests to validate the functionality and edge cases of the contract.
  - If applicable, ensure integration tests pass for any interaction between smart contracts.

Example command to deploy and test the contract:
```
tonos-cli deploy <smart-contract.tvc> <parameters.json> --sign <path-to-keyfile>
```

### Gas Optimization

- TON is a gas-efficient blockchain, so please keep gas consumption in mind when developing contracts.
- Use tools like [FunC optimizer](https://github.com/tonlabs/TON-Compiler) to check gas usage and optimize accordingly.

## Submitting Changes

1. **Commit your changes**  
   After making changes and running all tests, commit them:
   ```
   git add .
   git commit -m "Description of changes"
   ```

2. **Push to your fork**  
   Push your changes to your fork:
   ```
   git push origin your-feature-branch
   ```

3. **Open a Pull Request**  
   Go to the original repository and open a pull request from your branch. Describe your changes in detail and reference any issues your PR addresses.

## Code Review Process

- The project maintainers will review your pull request and provide feedback if needed.
- Ensure all discussions in the PR are resolved and requested changes are made before your contribution can be merged.

## License

By contributing to this project, you agree that your contributions will be licensed under the MIT License.

## Need Help?

If you have any questions or need assistance, feel free to ask in our [Telegram community](https://t.me/litrbull) or open an issue in this repository.
