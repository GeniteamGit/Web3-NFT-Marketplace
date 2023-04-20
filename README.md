## NFT Marketplace with Staking and Minting 🔥
<img src="src/assets/images/logo.jpg" width="100" height="100">

#### Description
Demo NFT marketplace based on one of the most popular blockchian Etherium
with most advance features of Staking and minting of NFTs

### Tech Stack
<ul>
    <li>ReactJS</li>
    <li>Web3.0 JS</li>
    <li>Etherium</li>
    <li>Solidity</li>
    <li>Metamask</li>
</ul>

### Features List
<ul>
    <li>Metamask 👜</li>
    <li>Etherium Chain ⛓️</li>
    <li>Minting🍦</li>
    <li>NFT Staking🎆</li>
    <li>Marketplace 🏪</li>
    <li>Offers🫴</li>
    <li>Activity 🎭</li>
    <li>Custom Coins 🪙</li>
    <li>Characters & Skins🤹‍♂️🤹‍♀️</li>
</ul>


### Directory Structure

. <br>
├── public <br>
├── src/ <br>
│   ├── assets/ <br>
│   │   ├── data <br>
│   │   └── images <br>
│   ├── components/ <br>
│   │   ├── Footer/ <br>
│   │   │   ├── footer.css <br>
│   │   │   └── Footer.jsx <br>
│   │   ├── Header/ <br>
│   │   │   ├── header.css <br>
│   │   │   └── Header.jsx <br>
│   │   ├── Layout/ <br>
│   │   │   └── Layout.jsx <br>
│   │   └── ui <br>
│   ├── config/ <br>
│   │   └── constants.json <br>
│   ├── pages/ <br>
│   │   ├── Market <br>
│   │   ├── CharacterDetails.jsx <br>
│   │   ├── Contact.jsx <br>
│   │   ├── Create.jsx <br>
│   │   ├── Favourite.jsx <br>
│   │   ├── Home.jsx <br>
│   │   ├── Listing-Active.jsx <br>
│   │   ├── Listing-Inactive.jsx <br>
│   │   ├── Market.jsx <br>
│   │   ├── Mint.jsx <br>
│   │   ├── MyCollection.jsx <br>
│   │   ├── Offers-Made.jsx <br>
│   │   ├── Offers-Received.jsx <br>
│   │   ├── Profile.jsx <br>
│   │   ├── SkinDetails.jsx <br>
│   │   ├── Staking.jsx <br>
│   │   ├── StakingDetails.jsx <br>
│   │   └── Wallet.jsx <br>
│   ├── routes/ <br>
│   │   └── Routers.jsx <br>
│   ├── styles/ <br>
│   │   ├── create-item.css <br>
│   │   ├── market.css <br>
│   │   ├── nft-details.css <br>
│   │   ├── overlay.css <br>
│   │   └── wallet.css <br>
│   ├── util/ <br>
│   │   └── UtilityMethods.jsx <br>
│   ├── App.css <br>
│   ├── App.js <br>
│   ├── index.css <br>
│   └── index.js <br>
├── .gitignore <br>
└── package.json <br>

### Installation
how to install and run this project <br>
```shell
 npm i --legacy-peer-deps
 ```
### Prerequesties
To run this project you need smart contracts deployed
to the etherium blockchain and their idl files
on the config folder.
Also need an active metamask account with some balance in it.

Also please check the config-overrides.js file and change the
```baseUrl``` to your local server address
<br>
```shell
npm run start
```


### Basic Configurations
Go to the config folder and update the Constants.json file with your firebase configs.<br>
```json
    {
  "secretKey": "xxxxxxxxxxxxxx",
  "dbListings": "listings",
  "dbOffers": "offers",
  "dbNfts": "nfts",
  "dbActivity": "activity",
  "transactionLimit": 1,
  "firebaseConfig": {
    "apiKey": "xxxxxxxxxxxxxxxxxxxxxxxx",
    "authDomain": "xxxxxxxxxxxxxxxxx.firebaseapp.com",
    "projectId": "xxxxxxxxxxxxxxxxx",
    "storageBucket": "xxxxxxxxxxxxxxxxx.appspot.com",
    "messagingSenderId": "xxxxxxxxxxxxxxx",
    "appId": "xxxxxxxxxxxxxxxxx:xxxxxxxxxxxxxxxxx"
  }
}
```
and update the jsons with your smart contract addresses and idl files in index.js
like this
```javascript
import marketplace from "./Marketplace.json";
import characters from "./Characters.json";
import skins from "./Skins.json";
import coin from "./Coin.json";
import staking from "./Staking";
import minting from "./NftMinting.json";
import config from "./Constants.json";
export {
    marketplace,
    characters,
    skins,
    coin,
    staking,
    minting,
    config
}
```
Thanks