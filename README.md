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

<pre>// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/access/Ownable.sol";
import "@openzeppelin/contracts/security/Pausable.sol";

contract MyToken is ERC20, Ownable, Pausable {
    constructor(string memory name, string memory symbol) ERC20(name, symbol) Ownable(msg.sender) {}

    event TokensMinted(address indexed to, uint256 amount);
    event TokensBurned(address indexed from, uint256 amount);

    function mint(address to, uint256 amount) external onlyOwner whenNotPaused {
        _mint(to, amount);
        emit TokensMinted(to, amount);
    }

    function burn(uint256 amount) external whenNotPaused {
        _burn(msg.sender, amount);
        emit TokensBurned(msg.sender, amount);
    }

    function pause() external onlyOwner {
        _pause();
    }

    function unpause() external onlyOwner {
        _unpause();
    }

    function transfer(address recipient, uint256 amount) public override whenNotPaused returns (bool) {
        return super.transfer(recipient, amount);
    }

    function transferFrom(address sender, address recipient, uint256 amount) public override whenNotPaused returns (bool) {
        return super.transferFrom(sender, recipient, amount);
    }
}
</pre>

In the "Deploy & Run Transactions" tab, select MyToken from the contract dropdown.

Click "Deploy".

Confirm the deployment transaction.

<h3> Interacting with the Contract </h3>

**Mint Tokens:**

Function: mint(address to, uint256 amount)

Description: Mint new tokens to a specified address.

Example :

<pre>mint("0x5B38Da6a701c568545dCfcB03FcB875f56beddC4", 1000)
</pre>


**Burning Tokens:**

Function: burn(uint256 amount)

Description: Burn a specified amount of your own tokens.

Example :

<pre> burn(200)
</pre>


**Transfer Tokens:**

Function: transfer(address recipient, uint256 amount)

Description: Transfer tokens to another address.

Example :

<pre>transfer("0xAb8483F64d9C6d1EcF9b849Ae677dD3315835Cb2", 500)
</pre>

**Pausing the Contract:**

Function: pause()

Description: Pause the contract (only the owner can call this).

Example :

<pre>pause()
</pre>

**Unpausing the Contract:**

Function: unpause()

Description: Unpause the contract (only the owner can call this).

Example : 

<pre>unpause()
</pre>



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








