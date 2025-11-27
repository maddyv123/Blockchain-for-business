# EX.NO-1
# CREATING A PRIVATE DATE: BLOCKCHAIN
# AIM
To create a Private Blockchain and to add nodes, create accounts, transfer Ether into it by creating
and deploying Smart contract.
# PROCEDURE
Step 1: 
The user provides their public key to the system. The system stores this key as the user’s identity.

Step 2: 
When the user wants to log in, the system creates a random challenge (nonce) and sends it to the user.

Step 3: 
The user signs the challenge using their private key and sends the signature back to the system.

Step 4: 
The system verifies the signature using the stored public key.
If valid, the user is successfully authenticated.
## program:
# Genesis file privateblock.json
```
{
  "config": {
    "chainId":100306,
    "homesteadBlock": 0,
    "eip150Block": 0,
    "eip155Block": 0,
    "eip158Block": 0,
    "byzantiumBlock": 0,
    "constantinopleBlock": 0,
    "petersburgBlock": 0,
    "istanbulBlock": 0,
    "berlinBlock": 0,
    "clique": {
      "period": 5,
      "epoch": 30000
    }
  },
  "difficulty": "0x1",
  "gasLimit": "0x7a1200",
  "extradata": "0x00000000000000000000000000000000000000000000000000000000000000009615a04324c5ad1b1DB9032306e361efed18734E0000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
  "alloc": {
    "9615a04324c5ad1b1DB9032306e361efed18734E": {
      "balance": "3000000000000000000"
    },
    "8Ed3DcdF69AE9809b31849A1CAD30517f1e57458": {
      "balance": "3000000000000000000"
    }
  }
}
```
# Smart Contract New.sol
```
//SPDX-License-Identifier MIT
pragma solidity ^0.8.19;
contract New{
string name;
function setName(string memory _name) public {
name= _name;
}
function getName() public view returns (string memory){
return name;
}
}
```
# OUTPUT:
# Deploying Transaction in Remix
7
# Contract Creation Output in Command Prompt
<img width="1919" height="1015" alt="Screenshot 2025-10-09 132412" src="https://github.com/user-attachments/assets/32f84ad8-5797-4bf1-89a2-cfb58ee96caf" />

# RESULT: 
Thus, the Private Blockchain is created, nodes are added with accounts, and Ether is transferred
into it by creating and deploying Smart contract successfully.
