# My Token

MyToken is an ERC20 compliant token with additional functionalities for minting, burning, pausing, and unpausing transactions. This smart contract uses OpenZeppelin's standard libraries for security and standardization.


<h2> Overview: </h2>

MyToken is a smart contract built on the Ethereum blockchain using the Solidity programming language. It utilizes OpenZeppelin's libraries for ERC20, Ownable, and Pausable functionalities to provide a secure and feature-rich token implementation.

<h2> Features: </h2> 

**ERC20 Standard:** Implements the standard ERC20 interface.

**Minting:** Allows the contract owner to mint new tokens.

**Burning:** Allows users to burn their own tokens.

**Pausable:** The owner can pause and unpause the contract, restricting token transfers during the paused state.

**Ownership:** The contract includes ownership management, allowing only the owner to execute specific functions.

<h2> Getting Started: </h2>

<h3> Installing </h3>

<h4> Using Remix IDE </h4> 

**Open Remix IDE:** 

Navigate to Remix IDE.

**Create the Smart Contract:**

Create a new file named "My Token.sol".

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








