# Solana Project - 2 Creation of SPL token and setting up the Candy machine UI.

This guide will assist you in configuring the user interface (UI) for your Candy Machine, enabling users to create NFTs utilizing the SPL token you have established. The UI will employ the SPL token as the payment mechanism, and users will have the capability to create NFTs by linking their Phantom wallet.

## Prerequisites
1. A  Candy Machine with critical informations in its `config.json` file, including pricing, quantity, symbol, seller fee, SPL token account, SPL token, go-live date, and creator details.
2. A Phantom wallet to act as the minting wallet.

## Steps

### 1. Set Up the SPL Token

Make sure you have one. If you don't, create one. Note down the SPL token's address. 

### 2. Update Candy Machine Configuration

Open your Candy Machine's `config.json` file and update the following fields:

- `splTokenAccount`: Update this field with the SPL token account address you've created.
- `splToken`: Update this field with the SPL token address.

### 3. Set Up the UI

Use the tutorial "Quick Node: Set Up a Minting Site" to set up the UI. This UI will allow users to connect their Phantom wallets and mint NFTs using the SPL token as payment.

### 4. Modify Minting Logic

In the minting logic, make the necessary adjustments to mint NFTs to the Phantom wallet address instead of the `fromWallet`. Alternatively, adjust the transfer function to send the minted NFTs to your Phantom wallet.

### 5. Testing

Test the entire setup by transferring or minting your SPL token to one of your Phantom accounts. Then, use the UI you've created to mint NFTs. The users should be able to mint NFTs by paying in the SPL token you've set up.

### By User Abhilash-101
my candy machine details
 - `splTokenAccount`: "CmYjWgk18KvpBeRpRvxdiowdq5Eko14MBZEnDf6LFwes"
   - `splToken`: "BRchm6kw2mQVFPsx9dtN8xfjpqMy7j9LhCs5jz3w9Tc9"
## Conclusion

By adhering to these instructions, you will have effectively established a user interface for a Candy Machine that permits individuals to create NFTs utilizing the SPL token you've developed. Users can link their Phantom wallets and employ the SPL token as payment to generate NFTs from your Candy Machine. It is crucial to extensively examine the configuration prior to making it accessible for public utilization.
