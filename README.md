# Guide Xen-X1-Blockchain

`sudo apt update -y`

`sudo apt install -y golang wget git make tmux`

`sudo git clone --branch x1 https://github.com/FairCrypto/go-x1 && cd go-x1 && make x1 && cp build/x1 /usr/local/bin`

# Run node

`tmux new -s xen`

`x1 --testnet --syncmode snap`

 (ctrl +b , d)

# Create Account key

`x1 account new`

# Create a new validator key

`x1 validator new`

# Backup

/root/.x1/keystore/


Click:
`https://explorer.x1-testnet.xen.network/address/0xFC00FACE00000000000000000000000000000000/write-contract#address-tabs`

-> Connection Wallet

Number no 4 Create Validator (Paste cái Public key Validator) Value XN: 100000
-> Click Write

Search ID for me

`https://pwa-explorer.x1-testnet.xen.network/staking`

# Start node: change ID và Public key 

`./build/x1 --testnet  --validator.id 19 --validator.pubkey 0xc004569...1e74943bb4 --xenblocks-endpoint ws://xenblocks.io:6668 --gcmode full --syncmode snap`

Guide Dev: https://github.com/JozefJarosciak/X1/blob/main/Validator-Instructions_Testnet.mdp
