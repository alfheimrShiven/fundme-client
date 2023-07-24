# fund-me-client
# Requirements

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - You'll know you've installed it right if you can run:
    - `git --version`
- [Metamask](https://metamask.io/)
  - This is a browser extension that lets you interact with the blockchain.

# Quickstart

1. Clone the repo

```
git clone https://github.com/alfheimrShiven/fundme-client.git
cd html-fund-me-fcc
```

2. Run the file.

You can usually just double click the file to "run it in the browser". Or you can right click the file in your VSCode and run "open with live server".

# Execute a transaction

1.  Start the Anvil blockchain and Deploy the [crowd-sourcing-smart-contract](https://github.com/alfheimrShiven/crowd-sourcing-smart-contract.git):

Note: You'll need to open up a second terminal

```
git clone https://github.com/alfheimrShiven/crowd-sourcing-smart-contract.git
cd crowd-sourcing-smart-contract
make build
make anvil
```

Then, in a second terminal
```
make deploy
```

This will start a local Anvil blockchain and deploy a sample contract.

2. Update your `constants.js` with the new contract address.

In your `constants.js` file, update the variable `contractAddress` with the address of the deployed "FundMe" contract. You'll see it near the top of the hardhat output.

3. Connect your [metamask](https://metamask.io/) to your local Anvil blockchain.

> **PLEASE USE A METAMASK ACCOUNT THAT ISNT ASSOCIATED WITH ANY REAL MONEY.**
> I usually use a few different browser profiles to separate my metamasks easily.

In the output of the above command, take one of the private key accounts and [import it into your metamask.](https://metamask.zendesk.com/hc/en-us/articles/360015489331-How-to-import-an-Account)

Additionally, add your local Anvil network with chainid 31337 to your metamask.

4. Finally, refresh the front end, input an amount in the text box, and hit `fund` button after connecting

# Thank you!

If you appreciated this, feel free to follow me!

[![Patrick Collins Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/shiven_alfheimr)
[![Patrick Collins Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shivends/)

