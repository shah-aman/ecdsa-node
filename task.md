ECDSA Node
The best way to deeply understand blockchain is to put yourself into development mode. What would it be like to build your own blockchain? Let's start by applying our knowledge of hashes and digital signatures to our very first project: ECDSA Node.

In this project you'll have a simple react front-end which will communicate with a single server. This server will be responsible for transferring balances between accounts. Since it's a single server, it is centralized, so we'll need to trust that the server operator is not malicious for this exercise (more on this later!).

🏁 Your Goal: ECDSA
This project begins with a client that is allowed to transfer any funds from any account to another account. That's not very secure. By applying digital signatures we can require that only the user with the appropriate private key can create a signature that will allow them to move funds from one account to the other. Then, the server can verify the signature to move funds from one account to another.

Incorporate Public Key Cryptography so transfers can only be completed with a valid signature
The person sending the transaction should have to verify that they own the private key corresponding to the address that is sending funds

🤔 While you're working through this project consider the security implications of your implementation decisions. What if someone intercepted a valid signature, would they be able to replay that transfer by sending it back to the server?

Tips
Helpful Resources

We're going to be incorporating the concepts we learned from this week into the final project. Here are a few resources you'll find helpful when working on this project:

Public Key Exercises in the Digital Signatures lesson (Recover Keys, Sign Message, Hash Messages)
The Ethereum Cryptography library - specifically random private key generation
