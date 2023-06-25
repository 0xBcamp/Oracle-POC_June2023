# Oracle POC

## Description

This is a POC for an EVM based blockchain oracle implementation. The oracle is implemented as a smart contract that can be deployed on any EVM based blockchain. The oracle is able to fetch data from a remote server and store it on the blockchain. The oracle can also be queried to fetch the data from the blockchain network itself. My main goal here is to implement a simple POC that only supports two operations at the current stage:

-   Fetch data from a remote server and use it within the smart contract
-   Automate the process of fetching data from the remote server and using it within the smart contract

---

## Pseudo Code

[//]: # "write a description for the pseudo code of the oracle service, the backend and the smart contract"

### **Architecture**

<details>
<summary>Oracle Service Overview</summary>

1.  Fetch data from remote server using a NodeJS backend
2.  Store/use data on blockchain after calling the backend service and getting the data from the exyternal server/s
3.  Query/stream data from blockchain by smart contract events to the backend service to check for conditions and automate the process of fetching data from the remote server/s or writing data to the blockchain

</details>

<details>
<summary>Backend</summary>

1. A NodeJS backend that is responsible for fetching data
2. The backend will utilize the 'ethersjs' library to interact with the blockchain and the smart contract
3. Smart contracts will be able to communicate with the backend using the 'ethersjs' library by capturing events emitted by the smart contract

</details>

<details>
<summary>Smart Contracts</summary>

1. A smart contract will be responsible for communicating with the backend
2. The smart contract will be able to fetch data from the backend and use it on the blockchain network
3. The smart contract will be able to emit events that can be used by the backend to automate the process of fetching data or writing data to the blockchain

</details>
