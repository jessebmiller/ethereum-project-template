# ethereum-project-template

My Ethereum Project Template

## Steps taken to create this repo

```
npm install --save-dev hardhat
npx hardhat
✔ What do you want to do? · Create a sample project
✔ Hardhat project root: · ./ethereum-project-template
✔ Do you want to add a .gitignore? (Y/n) · y
✔ Do you want to install the sample project's dependencies with npm (hardhat @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers ethers)? (Y/n) · y
mv hardhat.config.js hardhat.config.ts
npm install --save-dev ts-node typescript
npm install --save-dev chai @types/node @types/mocha @types/chai
```

Make the required updates

1. Plugins must be loaded with import instead of require.
1. You need to explicitly import the Hardhat config functions, like task.
1. If you are defining tasks, they need to access the Hardhat Runtime Environment explicitly, as a parameter.

Add a basic tsconfig.json

```
npm install ts-standard --save-dev
```

Add `lint` script to `package.json` `ts-standard`
Add `fix` script to `package.json` `ts-standard --fix`

```
npm run fix
```

Fixed problems it couldn't

```
ethereum-project-template/scripts/sample-ts-script.ts:3:1: Missing return type on function. (@typescript-eslint/explicit-function-return-type)
ethereum-project-template/test/basic-test.ts:8:5: 'accounts' is assigned a value but never used. (@typescript-eslint/no-unused-vars)
```


