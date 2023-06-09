# NFT Contract

This contract is an ERC721 Non-Fungible Token (NFT) contract. It allows users to mint NFTs, and to transfer and sell them to other users.

## Constants

- `MAX_TOKENS`: The maximum number of NFTs that can be minted.
- `TOKENS_RESERVED`: The number of NFTs that are reserved for the contract owner.
  price: The price of an NFT in ETH.
- `MAX_MINT_PER_TX`: The maximum number of NFTs that can be minted in a single transaction.
- `MAX_MINT_PER_WALLET`: The maximum number of NFTs that can be minted by a single wallet.

## Variables

- `isSaleActive`: A boolean that indicates whether the sale of NFTs is active.
- `totalSupply`: The total number of NFTs that have been minted.
- `mintedPerWallet`: A mapping that tracks the number of NFTs that have been minted by each wallet.
- `baseUri`: The base URI for the NFTs.
- `baseExtension`: The extension for the NFT metadata files.
  Functions
- `mint(uint256 \_numTokens)`: Mints \_numTokens NFTs to the caller.
- `toggleSale()`: Toggles the sale state of the contract.
- `setBaseUri(string memory \_baseUri)`: Sets the base URI for the NFTs.
- `setPrice(uint256 \_price)`: Sets the price of an NFT.
- `withdrawAll()`: Withdraws all of the funds from the contract to the owner.
- `tokenURI(uint256 tokenId)`: Returns the URI for the NFT with the specified ID.

## Events

- `Mint`: Fired when an NFT is minted.
- `SaleToggled`: Fired when the sale state of the contract is toggled.
- `BaseUriSet`: Fired when the base URI for the NFTs is set.
- `PriceSet`: Fired when the price of an NFT is set.
- `Withdrawal`: Fired when funds are withdrawn from the contract.
- `TokenURI`: Fired when the URI for an NFT is requested.#
