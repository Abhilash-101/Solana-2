# Creation of SPL token & Candy machine UI Setup

This will walk you through the steps to set up the user interface (UI) for your Candy Machine, allowing users to mint NFTs using the SPL token you've created. The UI will use the SPL token as the payment method, and users will be able to mint NFTs by connecting their Phantom wallet.

## Prerequisites
1.  - A  Candy Machine with critical informations in its `config.json` file, including pricing, quantity, symbol, seller fee, SPL token account, SPL token, go-live date, and creator details.
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
 - `splTokenAccount`: ""
   - `splToken`: ""
## Conclusion

By following these steps, you'll have successfully set up a Candy Machine UI that allows users to mint NFTs using the SPL token you've created. Users can connect their Phantom wallets and use the SPL token as payment to mint NFTs from your Candy Machine. Remember to thoroughly test the setup before deploying it for public use.
