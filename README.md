# Concordium Hackathon 

## Task 1: Concordium Blockchain Development Env

### Mainnet address: 

### Install Rust
Install Rust using the following command:

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

install wasm32-unknown-unknown target

```bash
rustup target add wasm32-unknown-unknown
```


### Install Cargo-Concordium
 -Download the latest release from [here](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#cargo-concordium-testnet)

 -Move the binary to ~/.cargo/bin

 -run cargo concordium --help to verify the installation




### Install Concordium Client

    -Download the latest release from [here](https://developer.concordium.software/en/mainnet/net/installation/downloads-testnet.html#concordium-node-and-client-download-testnet)
    
    -Move the binary to ~/.cargo/bin
    
    -run concordium-client --help to verify the installation

    -connect to the public node with the following command:
        
        ```bash
        concordium-client consensus status --grpc-port 10000 --grpc-ip node.testnet.concordium.com
        ```

### Setup a Testnet Account and get testnet CCD

- Used the Concordium Wallet for Web in chrome Browser to create a new account and get testnet CCD
- Created a new account on testnet IP and got 2000 CCD


### Export Wallet keys and import them into the Concordium Client

- Exported the keys from the wallet and imported them into the client using the following command:

```bash
concordium-client config account import 3jqux4HT14VgEWfBQzTDexGK4q2q2pmpMRDZYDvxKJks5pkupt.export --name Gunwant
```

