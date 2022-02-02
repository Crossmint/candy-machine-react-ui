# candy-machine-react-ui

This repository contains a minimal UI front-end in React, for creating NFT drop sites for Solana Candy Machines. With this repo, your customers will be able to mint Solana Candy Machine NFTs.

It is forked off the official Solana Metaplex repository, but contains improvements to make for a better development experience.

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

## Develop

Run `yarn dev` to start a local server

Then make any UI changes into the Home.tsx file
