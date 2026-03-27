# EtherSender.sol
Base - Smart Contract Deployed by Remix EtherSender.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract EtherSender {
    function sendEther(address payable _to) public payable {
        _to.transfer(msg.value);
    }
}
