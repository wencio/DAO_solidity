# DAO Contract

## Description

This Solidity smart contract, named DAO (Decentralized Autonomous Organization), facilitates the management of investor contributions and proposals within a decentralized organization. Key features include:

1. Collecting investors' funds (ether) and allocating shares.
2. Tracking investor contributions and shares.
3. Allowing investors to transfer shares.
4. Creating and voting on investment proposals.
5. Executing successful investment proposals, such as sending funds.

## Contract Details

- **Solidity Version:** ^0.8.0
- **Total Shares:** Tracks the total number of shares issued.
- **Available Funds:** Records the amount of ether available for investment proposals.
- **Contribution End:** Defines the end timestamp for accepting investor contributions.
- **Next Proposal ID:** Maintains the ID for the next investment proposal.
- **Vote Time:** Specifies the duration for voting on proposals.
- **Quorum:** Sets the minimum percentage of votes required for a proposal to be executed.
- **Admin:** Identifies the contract administrator.

## Usage

### Investor Functions

- **Contribute:** Investors can contribute ether during the contribution period.
- **Redeem Shares:** Investors can redeem their shares for ether.
- **Transfer Shares:** Investors can transfer shares to other addresses.

### Admin Functions

- **Create Proposal:** The contract administrator can create investment proposals specifying the name, amount, and recipient address.
- **Vote:** Investors can vote on proposals during the voting period.
- **Execute Proposal:** The contract administrator can execute successful proposals after the voting period, subject to the quorum requirement.
- **Withdraw Ether:** The contract administrator can withdraw ether from the contract.

## Smart Contract Integration

To integrate the DAO contract into your DApp, follow these steps:

1. Deploy the DAO contract on the Ethereum blockchain.
2. Connect your frontend application to the deployed contract using Web3.js or similar libraries.
3. Implement user interfaces for investors to contribute, redeem shares, transfer shares, and vote on proposals.
4. Provide administrative interfaces for creating proposals, executing proposals, and withdrawing ether.
5. Monitor contract events and states to keep users informed about the status of proposals and their shares.

## Sample Application

The `App.js` file provided alongside the contract demonstrates a React-based frontend application that interacts with the DAO contract. It includes functionalities for contributing, redeeming shares, transferring shares, creating proposals, voting on proposals, executing proposals, and withdrawing ether.

For more details on contract methods and events, refer to the contract's ABI (Application Binary Interface) and the Web3 documentation.

## License

This Solidity contract is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Author
