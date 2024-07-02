
# Remix Default Workspace

The Remix default workspace is present in the following situations:
1. When Remix is loaded for the very first time.
2. When a new workspace is created using the 'Default' template.
3. When no files exist in the File Explorer.

This workspace contains three directories:

1. **contracts**: This directory holds three contracts of increasing complexity.
2. **scripts**: This folder contains four TypeScript files to deploy a contract, explained below.
3. **tests**: This folder includes one Solidity test file for the 'Ballot' contract and one JavaScript test file for the 'Storage' contract.

## Scripts

The 'scripts' folder includes four TypeScript files that assist in deploying the 'Storage' contract using the 'web3.js' and 'ethers.js' libraries.

To deploy a different contract, update the contract name from 'Storage' to the desired contract and provide the necessary constructor arguments in the `deploy_with_ethers.ts` or `deploy_with_web3.ts` files.

## Tests

The 'tests' folder contains a Mocha-Chai unit test script for the 'Storage' contract.

To run a script, right-click on the file name in the file explorer and select 'Run'. Ensure that the Solidity file is already compiled. The script output will appear in the Remix terminal.

**Note:** The require/import functionality is supported in a limited manner for Remix-supported modules. Currently, Remix supports the following modules: `ethers`, `web3`, `swarmgw`, `chai`, `multihashes`, `remix`, and `hardhat` (only for the `hardhat.ethers` object/plugin). If you attempt to require an unsupported module, an error message will be displayed: `<module_name> module require is not supported by Remix IDE`.
