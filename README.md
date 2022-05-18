# nisa-DAO


development steps
1. write smart contracts (testing each contract)
2. write deployment scripts (testing each script)
3. write scripts that interact (testing each script)


stack
1. hardhat development env
2. solidity
3. typescript
4. testing language here


startup steps
1. open directory and run `yarn add --dev hardhat` to install hardhat dev env
2. run `yarn hardhat` and select 'empty hardhat.config.js'
3. create 'contracts' directory in root
4. add openzeppelin package for easy contract import `yarn add --dev @openzeppelin/contracts`
5. adjust solidity compiler version in hardhat.config.js

contracts directory
1. governance_standard directory (contains governance models)
    - GovernerContract.sol (contains governance voting logic)
    - TimeLock.sol (contains owner of Box.sol)
2. Box.sol (@openzeppelin/contracts Ownable.sol)
3. GovernanceToken.sol (@openzepplin/contracts ERC20Votes.sol )