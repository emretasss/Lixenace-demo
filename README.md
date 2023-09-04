
## Features

- 🔔 **Notifications** : Notifications popup for every event
- 🔥 **Responsive Design** : Design also suited for small and medium devices.
- 🤏 **Optimized Performance** :  Performance optimized using [lighthouse](https://developers.google.com/web/tools/lighthouse).

## Built With

`FRONTEND`
- ReactJS
- TailwindCSS
- react-router
- Ethers
 
`BACKEND`
- Hardhat
- Ethers
- Chai


<!-- GETTING STARTED -->
## Getting Started

Follow these steps to setup this project locally.

### Installation

_Below are the instructions to setup this project and get started with._

1. Clone the repo
   ```sh
   git clone https://github.com/emretasss/Cryptoace-demo.git
   ```
2. Install NPM packages for `client` and `smart_contracts` folder
   ```sh
   npm install
   ```
3. Generate an API url for contracts and add your url to `hardhat.config.js` file using [Alchemy.io](https://www.alchemy.com/)
   ```js
   // hardhat.config.js file in smart_contracts
    ropsten: {
      url: {/* Your own url of contracts */},
    },
   ```
4. Add your metamask account's private key in `.env` file of smart_contract dir 
   ```sh
   PRIVATE_KEY=Metamask account private key 
   ```
5. Compile the smart_contracts using 
   ```sh
   npx hardhat run scripts/deploy.js --network ropsten
   ```
   This will compile contracts and provide the addresses of deployed contracts.
6. Create `.env` file in `client` folder and enter the contract addresses as shown below. 
   ```sh
   // add your addresses to .env
   VITE_TRANSACTION_CONTRACT=
   VITE_ACE_TOKEN_CONTRACT=
   VITE_TOKEN_SALE_CONTRACT=
   VITE_LOTTERY_CONTRACT=
   ``` 

7. Run the application by running following command in client folder
   ```sh
   npm run dev
   ```
<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

A few open-source resources that helped in the development of this project.

* [Rad Lines](https://msurguy.github.io/rad-lines/)
* [Remix Etherium](https://remix.ethereum.org/)
* [Shapefest](https://www.shapefest.com/)
* [3dIcons](https://3dicons.co/)

:star: Like the project? Star this repo — It motivates a lot!
