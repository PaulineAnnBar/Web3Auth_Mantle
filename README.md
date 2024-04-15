# Web3Auth PnP Modal React Quick Start
This guide is designed to help you quickly integrate a basic instance of Web3Auth Plug and Play (PnP) Modal in your React application with Mantle chain configuration. You can refer to the full documentation here: https://web3auth.io/docs/sdk/pnp/web/modal

### Step 1:  Set up your project

Clone the PnP Modal React Quick Start Application for a quick setup:
```npx degit Web3Auth/web3auth-pnp-examples/web-modal-sdk/quick-starts/react-modal-quick-start w3a-quick-start```

### Step 2: Install & Run

```
cd w3a-quick-start
npm install
npm run start
```

### Step 3: Install the web3Auth package
```
npm install --save @web3auth/modal
```

### Step 4:  Get your Client ID from the Web3Auth Dashboard

You will need to get the clientID from Web3Auth dashboard here 👉 https://dashboard.web3auth.io
Once this is done, you set up a new project from the project dashboard and paste the client ID into the `App.tsx`file as below :
![Screenshot 2024-04-15 at 14 42 38](https://github.com/PaulineAnnBar/Web3Auth_Mantle/assets/101885938/efe2acc1-6730-4444-b0a0-a86d248f0a05)


### Step 6 : Configuration for the Mantle chain
````
const chainConfig = {
  chainId: "0x1388", 
  rpcTarget: "https://rpc.mantle.xyz",
  chainNamespace: CHAIN_NAMESPACES.EIP155,
  displayName: "Mantle Mainnet",
  blockExplorerUrl: "https://explorer.mantle.xyz/",
  //we will add the etherscan link when implementation done
  ticker: "MNT",
  tickerName: "Mantle",
  logo: "https://cryptologos.cc/logos/mantle-mnt-logo.svg?v=031",
}


