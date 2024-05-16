# Functions and Errors
assert, require, and revert – as new error handling constructs. With the throw statement made absolute, developers can now more effectively 
manage errors and optimize gas usage in their code.

## Description
Good day, Im Marc and we are here again for another project assessment in metacrafters. So here's the assessment that we need to do its all about functions and errors
of require, assert and revert.

## Getting Started
// SPDX-License-Identifier: MIT pragma solidity ^0.8.0;

/*REQUIREMENTS: For this project, write a smart contract that implements the require(), assert() and revert() statements.

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract ErrorHandlingExample {
    uint256 public value;

   
    function setValue(uint256 _value) public {
       
        require(_value > 0, "Value must be greater than zero");
        
        value = _value;
    }

   
    function checkInvariant() public view {
       
        assert(value != 0);
    }

  
    function triggerRevert() public pure {
        
        revert("This function always reverts");
    }
}

## Executing Program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/. 
Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension 
(e.g., HelloWorld.sol). Then copy the code given in the assessment.

## Author
Marc Danniel Mariazeta 61902476@ntc.edu.ph
