# Homework4
Make the contract at the end of: https://coursetro.com/posts/code/102/Solidity-Mappings-&-Structs-Tutorial
Compatible with solidity 0.5 or higher.

## Dependencies:
Install these prerequisites:
- NPM: https://nodejs.org
- Truffle: https://github.com/trufflesuite/truffle
- Ganache: http://truffleframework.com/ganache/

## Step 1: Clone the projects:
```
git clone https://github.com/quong1/Homework4.git
```

## Step 2: Install dependencies
On the root folder:
```
$ npm install
```

## Step 3: Start Ganache
Open the Ganache GUI client 

## Step 4: Compile & Deploy Smart Contract
- Based on the code given at https://coursetro.com/posts/code/102/Solidity-Mappings-&-Structs-Tutorial. I make some changes for it to be able to run on solidity ^0.5.0 in Courses. sol.
- I also create a second migration Javascript file named 2_migration.js for truffle to compile.
- Compile and deploy smart contract using:
```
truffle compile 
truffle develop migrate --reset
truffle develop
```

- Inside truffle develop, compile the contract using
```
migrate --reset --all
```

## Step 6: Testing function

- Function setInstructor:
```
Courses.deployed().then(function(func){return func.setInstructor("0xAe2CF87569ABc0ACf0733d854e0705840fB5C783",34,"Alpha","Beta");})
```
Output:
![Image](https://github.com/quong1/Homework4/blob/master/homework4/Output%20screenshots/Screenshot%20(101).png)

- Function getInstructor:
```
Courses.deployed().then(function(func){return func.getInstructor("0xAe2CF87569ABc0ACf0733d854e0705840fB5C783");})
```
Output:
![Image](https://github.com/quong1/Homework4/blob/master/homework4/Output%20screenshots/Screenshot%20(102).png)
- Function getInsturctors:
```
Courses.deployed().then(function(func){return func.getInstructors();})
```
Output:
![Image](https://github.com/quong1/Homework4/blob/master/homework4/Output%20screenshots/Screenshot%20(103).png)
- Function countInstuctors:
```
Courses.deployed().then(function(func){return func.countInstructors();})
```
Output:
![Image](https://github.com/quong1/Homework4/blob/master/homework4/Output%20screenshots/Screenshot%20(104).png)

