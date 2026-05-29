# erc20-token-
My First ERC20 Token Smart Contract
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract MyToken is ERC20 {
    constructor() ERC20("Buahlil", "BHL") {
        // Mint 10.000.000 token ke wallet kamu (18 decimals = standar ERC20)
        _mint(msg.sender, 10000000 * 10 ** decimals());
    }
}
