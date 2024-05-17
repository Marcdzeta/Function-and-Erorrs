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

contract GradeQuiz {
    address public teacher;
    mapping(address => uint) public Scores;
    event ScoreAssigned(address indexed student, uint score);
    event Error(string message);

    modifier onlyTeacher() {
        require(msg.sender == teacher, "Only the teacher can perform this action.");
        _;
    }

    modifier validScore(uint score) {
        require(score >= 50 && score <= 100, "Score must be between 50 and 100.");
        _;
    }

    constructor() {
        teacher = msg.sender;
        assert(teacher != address(0)); // This should never fail
    }

    function assignScore(address student, uint score) public onlyTeacher validScore(score) {
        if (Scores[student] != 0) {
            emit Error("Score already assigned to this student.");
            revert("Score already assigned to this student.");
        }

        Scores[student] = score;
        emit ScoreAssigned(student, score);
    }

    function getScore(address student) public view returns (uint) {
        uint score = Scores[student];
        require(score != 0, "No score assigned to this student.");
        return score;
    }
}

## Executing Program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/. 
Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension 
(e.g., HelloWorld.sol). Then copy the code given in the assessment.

## Author
Marc Danniel Mariazeta 61902476@ntc.edu.ph
