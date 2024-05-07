# NFT Market Hub aka OpenD

OpenD is a decentralized NFT (Non-Fungible Token) market hub where users can discover, buy, sell, and mint NFTs with ease. Built on blockchain technology, OpenD provides a secure and transparent platform for creators and collectors to interact and exchange digital assets.
Please note that this is the clone of [OpenSea](https://opensea.io/) 

## Demo

### 1. Home Page
The home page welcomes users to OpenD and provides an overview of featured NFT collections, trending artworks, and upcoming events. Users can explore various categories and collections or search for specific NFTs.

![Home Page](/src/opend_assets/assets/home-page.png)

### 2. My NFTs
In the My NFTs section, users can view their owned NFTs, track their collections, and manage their digital assets. Users have full control over their NFTs, including the ability to transfer, sell, or showcase them in their virtual galleries.

![My NFTs](/src/opend_assets/assets/my-nfts.png)

### 3. Discover
Discover showcases a curated selection of NFTs from emerging and established artists. Users can browse through different categories, explore trending collections, and discover unique digital artworks. OpenD regularly updates its Discover section to highlight new and noteworthy NFTs.

![Discover](/src/opend_assets/assets/discover.png)

### 4. Minting
Minting allows creators to tokenize their digital creations and transform them into NFTs. By minting NFTs on OpenD, creators can establish ownership, authenticity, and scarcity for their digital assets. The minting process is intuitive and streamlined, making it accessible to creators of all skill levels.

![Minting](/src/opend_assets/assets/minting.png)

### 5. Minted
Minted showcases recently minted NFTs and highlights the latest additions to the OpenD marketplace. Users can discover fresh content, support emerging artists, and stay up-to-date with the latest trends in the NFT space.

![Minted](/src/opend_assets/assets/minted.png)

### 6. Wallet
The Wallet section provides users with a secure and convenient way to manage their digital assets. Users can connect their wallets, view their NFT holdings, and perform transactions directly from the OpenD platform. OpenD supports various blockchain networks and compatible wallet providers.

![Wallet](/src/opend_assets/assets/wallet.png)

----------------------------------------

# To Install and Run the Project

1. start local dfx

```
dfx start --clean
```

2. Run NPM server

```
npm start
```

3. Deploy canisters

to get principal
dfx identity get-principal
```
dfx deploy --argument='("CryptoDunks #123", principal "iii2z-iuk7j-dxzwn-f4sqf-x47s7-ix4tj-e26hn-yxm5j-ynttt-zpi5a-cae", (vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}))'
```


# Creating NFT for Testing

1. Mint an NFT on the command line to get NFT into mapOfNFTs:

```
dfx canister call opend mint '(vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}, "CryptoDunks #123")'
```

2. List the item into mapOfListings:

```
dfx canister call opend listItem '(principal "<REPLACE WITH NFT CANISTER ID>", 2)'
```

3. Get OpenD canister ID:

```
dfx canister id opend
```

4. Transfer NFT to OpenD:

```
dfx canister call <REPLACE WITH NFT CANISTER ID> transferOwnership '(principal "<REPLACE WITH OPEND CANISTER ID>", true)'
```

# Conneting to the Token Canister

1. Copy over the token declarations folder

2. Set the token canister id into the <REPLACE WITH TOKEN CANISTER ID>

```
const dangPrincipal = Principal.fromText("<REPLACE WITH TOKEN CANISTER ID>");
```
