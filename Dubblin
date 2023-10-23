// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract MyCryptoToken {

    // public variables here
    string public tokenName = "Dubblin";
    string public tokenAbr = "DBLN";
    uint public tokenSupply;

    // mapping variable here
    mapping (address => uint) public balance;

    // mint function
    function mint(address _address, uint _value) public {
      tokenSupply += _value;
      balance[_address] += _value;
    }

    // burn function
    function burn(address _address, uint _value) public {
       if (balance[_address] >= _value) {
          tokenSupply -= _value;
         balance[_address] -= _value;
      } 
    }
}
