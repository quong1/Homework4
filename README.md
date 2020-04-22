# Homework4
Make the contract at the end of: https://coursetro.com/posts/code/102/Solidity-Mappings-&-Structs-Tutorial
Compatible with solidity 0.5 or higher.

## Dependencies:
Install these prerequisites:
- NPM: https://nodejs.org
- Truffle: https://github.com/trufflesuite/truffle
- Ganache: http://truffleframework.com/ganache/

## Step 1:Clone the projects:
git clone https://github.com/quong1/Homework4.git


## Step 2: Install dependencies
On the root folder:
```
$ npm install
```

## Step 3: Start Ganache
Open the Ganache GUI client 

## Step 4: Compile & Deploy Smart Contract
```
truffle compile 
truffle develop migrate --reset
truffle develop
```

Inside the develop, compile the contract using
```

migrate --reset --all
```

## Step 5: Testing function

- Function setInstructor:
```
Courses.deployed().then(function(func){return func.setInstructor("0xAe2CF87569ABc0ACf0733d854e0705840fB5C783",34,"Alpha","Beta");})
```
Output:

- Function getInstructor:
```
Courses.deployed().then(function(func){return func.getInstructor("0xAe2CF87569ABc0ACf0733d854e0705840fB5C783");})
```
Output:
- Function getInsturctors:
```
Courses.deployed().then(function(func){return func.getInstructors();})
```
Output:

-Function countInstuctors:
```
Courses.deployed().then(function(func){return func.countInstructors();})
```
Output:


