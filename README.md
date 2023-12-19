# Minting Tokens and NFTs

This project contains three sections:
1. Token: SPL token used to mint
2. NFT: NFT minted using sugar cli
3. UI: This is the candy machine ui used for interactions with the NFT contract.


### Executing program
1. Token Program: cd into the token folder and run: `npm run generate`. This will generate an SPL token. Please remember to use your wallet public key in the .env file.
2. NFT: To run this cd into the nft folder and use the splToken address and splTokenAccount generated from token program. Then, use sugar-cli to mint. You can follow the following steps:
    1. `sugar validate`
    2. `sugar upload`
    3. `sugar deploy`
    4. `sugar verify`
    5. `sugar mint`
If you run into any problems, please delete the cache.json and re-run
3. UI: Once the above steps are done, cd into the UI folder and configure your .env file with the following:
`   REACT_APP_CANDY_MACHINE_ID=CANDY_MACHINE_IF_FROM_STEP_2
    REACT_APP_SOLANA_NETWORK=devnet
    REACT_APP_SOLANA_RPC_HOST=https://api.devnet.solana.com/
    SKIP_PREFLIGHT_CHECK=true
`
Then, run `npm run start`
## Authors

Rohan Dhar


## License

This project is licensed under the MIT License - see the LICENSE.md file for details