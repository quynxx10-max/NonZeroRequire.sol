# NonZeroRequire.sol
NonZeroRequire.sol
pragma solidity ^0.8.20;
contract NonZeroRequire {
    uint public value;

    function set(uint x) public {
        require(x != 0, "Zero not allowed");
        value = x;
    }
}
