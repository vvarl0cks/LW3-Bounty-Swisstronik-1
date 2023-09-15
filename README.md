# LearnWeb3DAO <> Swisstronik Challenge #1      

💰 Bounty: https://learnweb3.io/bounties/swisstronik-challenge-1/   
📚 Guide: https://swisstronik.gitbook.io/swisstronik-docs/build-on-swisstronik/contract-deployment-hardhat   

# Deploy    

```bash
npx hardhat run scripts/deploy.js --network swisstronik
Swisstronik contract deployed to 0x946a8074384561fE4A2345B633a8773348902D29
Deployment completed successfully.
```   

⛓ `Deployed Contract:` https://explorer-evm.testnet.swisstronik.com/address/0x946a8074384561fE4A2345B633a8773348902D29   

# Interact with contract transaction   

```shell
gitpod /workspace/LW3-Bounty-Swisstronik-1 (main) $ npx hardhat run scripts/setMessage.js --network swisstronik
Transaction Receipt:  {
  hash: '0xf71f9f7a285a77a4aa9e5a72b67d4aac351e8c75ca0f9c7234de14c4a1181ad6',
  type: 2,
  accessList: [],
  blockHash: null,
  blockNumber: null,
  transactionIndex: null,
  confirmations: 0,
  from: '0x2565ff82169a62Ea1D1210D17F05E69d689534d1',
  gasPrice: BigNumber { value: "8" },
  maxPriorityFeePerGas: BigNumber { value: "0" },
  maxFeePerGas: BigNumber { value: "8" },
  gasLimit: BigNumber { value: "27595" },
  to: '0x946a8074384561fE4A2345B633a8773348902D29',
  value: BigNumber { value: "0" },
  nonce: 6,
  data: '0x15ecd84bc9e94cf355913aff7cee6f5918c9b35fdce128afd3c30ff919e1ba133267d10f806d2cc485e60ffee9c73231e765befc24bcba537de093ab585fe394e6d249a1b9de977a84739fc5df5051e8b7718d866e72b9d30e579cbbeb04dd7bf70c0d8c74c923de75b5f33e9f83289145388398fa82174b5fa2fdcf5badb70d6d0ee4aa1c4b56c82fab819e5f0b705383485e5e2f7a88b5f472ec360864a9b3de4e41da62a627f479eb279643c9da71c367cd',
  r: '0x3fe46960edc13bcb97f88ad851d1daf44986387410c94ec9995500484b57ce51',
  s: '0x10bc76bc761bc903b9bc1f9312c2026503e71907313c5e5f98c840f9193c14e8',
  v: 1,
  creates: null,
  chainId: 1291,
  wait: [Function (anonymous)]
}
```   

# Interact with contract call   

```shell
gitpod /workspace/LW3-Bounty-Swisstronik-1 (main) $ npx hardhat run scripts/getMessage.js --network swisstronik
Decoded response: Hello Swisstronik!!
```    

<img src="https://i.postimg.cc/fLDJ0t3s/decoded.png"/>   

# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```   
