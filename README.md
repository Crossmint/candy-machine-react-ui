[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FCrossMint%2Fcandy-machine-react-ui&env=REACT_APP_CANDY_MACHINE_ID,REACT_APP_SOLANA_NETWORK,REACT_APP_SOLANA_RPC_HOST,REACT_APP_CROSSMINT_ID&project-name=candy-machine-ui&repo-name=candy-machine-react-ui)

# candy-machine-react-ui

Create your NFT minting site for Solana Candy Machine, in less than 5 minutes.

This repository contains a minimal UI front-end in React, for creating NFT drop sites for Solana Candy Machines. 

It also includes the option to accept credit cards via Crossmint (which takes under 5 min to set up as well).

<img width="544" alt="Example image" src="https://user-images.githubusercontent.com/93743232/155666012-2e0d3788-531f-435b-8466-4af89df816f7.png">


## Set up

Make sure you have `yarn` and `git` installed. Then run:

```
git clone https://github.com/CrossMint/candy-machine-react-ui.git
cd candy-machine-react-ui
yarn
```

## Configure

Copy the .env.template file into a file named .env

Then, uncomment either the "development" or "production" lines, depending on whether you are running a devnet candy machine or a production one.

Finally, in `<YOUR CANDY MACHINE PROGRAM ID>`, enter the candy machine ID you obtained when uploading your assets. [More info](https://docs.metaplex.com/candy-machine-v2/creating-candy-machine)

## Accept credit card payments

Accepting credit card payments allows you to sell to more customers who don't yet have a wallet, or are using their phones. With crossmint, accepting credit cards is free for you (seller), and you'll still receive all the funds instantly in SOL. [Learn more](https://www.crossmint.io)

To accept credit card payments using crossmint:
1. Register your NFT drop in https://www.crossmint.io/developers/onboarding (takes 2-3 min)
2. Once you receive a client ID, enter it in your .env file as `REACT_APP_CROSSMINT_ID`
3. Then, in Home.tsx., edit the `<CrossMintButton>` properties for your collection name, description and photo

You can now accept credit card payments -- and you'll get all the money from purchases in SOL, instantaneously when someone purchases!

## Develop

Run `yarn dev` to start a local server

Then make any UI changes into the `Home.tsx` file

Also be sure to update the title and description of your site in `index.html`

## Deploy with Vercel

We recommend you deploy to Vercel, as it's free, scalable and very easy to use.

To do so:

1. Create an account at vercel.com
2. Install the vercel command line
3. Run `vercel` on your project folder (generally the recommended configuration works)
4. Go to the vercel console and configure the domain for your drop

Or just click this button:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FCrossMint%2Fcandy-machine-react-ui&env=REACT_APP_CANDY_MACHINE_ID,REACT_APP_SOLANA_NETWORK,REACT_APP_SOLANA_RPC_HOST,REACT_APP_CROSSMINT_ID&project-name=candy-machine-ui&repo-name=candy-machine-react-ui)
