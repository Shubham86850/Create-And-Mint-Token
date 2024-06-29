# Create-And-Mint-Token


<h2> Overview: </h2>


"Create and Mint Token" is a basic ERC20 token smart contract designed for easy implementation and interaction. It provides functionality for minting, transferring, approving, transferring from allowance, and burning tokens, with a straightforward interface suitable for learning and basic applications.

<h2> Description: </h2> 

"Create and Mint Token" is a Solidity-based implementation of the ERC20 standard, providing a streamlined approach to token management. The contract allows the owner to mint new tokens, and users can transfer tokens, approve allowances, transfer tokens on behalf of others, and burn tokens. The goal of this project is to offer a simple and clear example of ERC20 token operations, making it ideal for educational purposes and basic token-based applications.

<h2> Getting Started: </h2>

<h3> Installing </h3>

<h4> Using Remix IDE </h4> 

**Open Remix IDE:** 

Navigate to Remix IDE.

**Create the Smart Contract:**

Create a new file named "Create And Mint Token.sol".

Copy and paste the provided smart contract code into the file.

**Compile the Contract:**

Select the appropriate Solidity compiler version (0.8.0 or higher).

Compile the SimpleToken contract.

<h2> Executing Program </h2>

<h4> Deploying the Contract </h4>

**Deploy:**

In the "Deploy & Run Transactions" tab, select SimpleToken from the contract dropdown.

Click "Deploy".

Confirm the deployment transaction.

<h4> Interacting with the Contract </h4>

**Mint Tokens:**

Function: mint(address to, uint256 amount)

**Transfer Tokens:**

Function: transfer(address to, uint256 amount)

**Approve Allowance:**

Function: approve(address spender, uint256 amount)

**Transfer From Allowance:**

Function: transferFrom(address from, address to, uint256 amount)

**Burn Tokens:**

Function: burn(uint256 amount)

<h2> Help </h2>

For common problems or issues, ensure the following:

You are using the correct address for each function.

The owner is the only one calling the **mint** function.

Sufficient allowance is approved for **transferFrom**.

<h2> Authors </h2>

<h4> Shubham </h4>

**Github :** [Shubham86850](https://github.com/Shubham86850)


<h2> License </h2>

This project is licensed under the MIT License.








