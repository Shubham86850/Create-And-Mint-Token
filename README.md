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


**1. Open Remix IDE:** 

  Navigate to [Remix](https://remix.ethereum.org/) IDE.

**2. Create the Smart Contract:**

  Create a new file named "Crate and Mint.sol".

  Copy and paste the provided smart contract code into the file.

**3. Compile the Contract:**

  Select the appropriate Solidity compiler version (0.8.0 or higher).

  Compile the MyToken contract.

<h2> Executing Program </h2>

<h3> Deploying the Contract </h3>

**Deploy:**

In the "Deploy & Run Transactions" tab, select MyToken from the contract dropdown.

Click "Deploy".

Confirm the deployment transaction.

<h3> Interacting with the Contract </h3>

**Mint Tokens:**

Function: mint(address to, uint256 amount)

Description: Mint new tokens to a specified address.

**Transfer Tokens:**

Function: transfer(address to, uint256 amount)

Description: Transfer tokens to another address.

**Pausing the Contract:**

Function: pause()

Description: Pause the contract (only the owner can call this).

**Unpausing the Contract:**

Function: unpause()

Description: Unpause the contract (only the owner can call this).



<h2> Help </h2>

For common problems or issues, ensure the following:

You are using the correct address for each function.

The owner is the only one calling the **mint** function.

Verify all required imports are included.

Enter the required constructor parameters (name and symbol).

<h2> Authors </h2>

<h4> Shubham </h4>

**Github :** [Shubham86850](https://github.com/Shubham86850)


<h2> License </h2>

This project is licensed under the MIT License.








