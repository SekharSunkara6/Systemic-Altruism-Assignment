# Bonding Curve Token

This smart contract is a Bonding Curve Token, which is a token (BCT) that follows a **specific mathematical formula** for determining its price.

The contract's primary purpose is to implement a bonding curve mechanism, a mathematical formula that determines the price of the token in question.

It implements the ERC20 standard for tokens and the Ownable standard from the OpenZeppelin library, which allows the contract to have an owner with specific privileges. The contract has several functions, including **buy**, **sell**, **withdraw**, and **getCurrentPrice**.

The **buy** function allows users to purchase tokens with Ether and the sell function allows them to sell tokens at a 10% loss.

The **withdraw** function allows the owner to withdraw any lost Ether and the getCurrentPrice function returns the current price of the token based on the bonding curve formula.

## Scripts

This repository includes the following scripts in the `package.json` file:

### Test

`npm run test`

This command runs the test suite for the contract using the Hardhat testing framework. It will execute the command `npx hardhat test`, which will run all the tests in the project. The tests are used to check that the contract behaves as expected and to ensure that any changes made to the contract don't break existing functionality.

### Test with coverage

`npm run test:coverage`

This command runs the test suite and generates a coverage report for the contract. It will execute the command `npx hardhat coverage`, which will run all the tests in the project and also generate a coverage report. A coverage report shows how much of the contract's code is being executed by the test suite.

### Compile

```
npm run compile
```

This command compiles the contract using the Hardhat compiler. It will execute the command `npx hardhat compile`, which will compile the contract code, and generate the bytecode and ABI needed to deploy the contract on the Ethereum blockchain.

### Lint TypeScript

```
npm run lint:ts
```

This command runs the ESLint linter on all TypeScript files in the project. It will execute the command `npx eslint '**/*.ts'`, which will check all TypeScript files in the project against a set of linting rules and report any errors or warnings.

### Lint TypeScript and fix issues

```
npm run lint:ts-fix
```

This command runs the ESLint linter on all TypeScript files in the project and automatically fix any issues it finds.

### Lint Solidity

```
npm run lint:sol
```

This command runs the Prettier and Solhint linters on all the Solidity files in the project. It will execute the command `npx prettier '**/*.{json,sol,md}' --check && npx solhint 'contracts/**/*.sol'`, which will check all the solidity files in the project against a set of linting rules and report any errors or warnings.

### Lint Solidity and fix issues

```
npm run lint:sol-fix
```

This command runs the Prettier and Solhint linters on all the Solidity files in the project and automatically fix any issues it finds.

### Lint all

```
npm run lint
```

This command runs both TypeScript and Solidity linters in the project.

### Lint all and fix issues

```
npm run lint:fix
```

This command runs both TypeScript and Solidity linters in the project and automatically fix any issues it finds.

