# Deploy an encrypted contract Devnet Seismic 

### Here we will describe commands on how to deploy a smart contract, Devnet Seismic. The commands will go in order, just paste them into the console. Also, for deployment, you will need at least 8 RAM on the server.

### Also, to get started, visit the project's official faucet and get test ETH tokens on the Devnet Seismic network.

#### Link: https://faucet-2.seismicdev.net/

#### Code:

```
sudo apt update
sudo apt upgrade -y
sudo apt install -y curl git build-essential
--------------------------
sudo apt install file -y
--------------------------
sudo apt install unzip -y
--------------------------
curl https://sh.rustup.rs -sSf | sh
source "$HOME/.cargo/env"
rustc --version
--------------------------
sudo apt install -y jq
jq --version
--------------------------
curl -L \
     -H "Accept: application/vnd.github.v3.raw" \
     "https://api.github.com/repos/SeismicSystems/seismic-foundry/contents/sfoundryup/install?ref=seismic" | bash
--------------------------
source ~/.bashrc
--------------------------
sfoundryup      / it can take from 5 to 20 minutes
--------------------------
git clone --recurse-submodules https://github.com/SeismicSystems/try-devnet.git
cd try-devnet/packages/contract/
--------------------------
bash script/deploy.sh
--------------------------
```
#### Next, you will receive a wallet, where you need to deposit the test ETH you received in the first step. Send 0.1 ETH there. Below is an example of what it looks like.

[![Screenshot-7.png](https://i.postimg.cc/prRQBFLM/Screenshot-7.png)](https://postimg.cc/vg26YDn0)

#### wait a few minutes for the tokens to reach this wallet, and then simply press enter. You will see the following image: 

[![Screenshot-8.png](https://i.postimg.cc/28Xv1JhD/Screenshot-8.png)](https://postimg.cc/56LjGss7)

### Done!

### Interaction with an extended contract: 

#### Code:

```
curl -fsSL https://bun.sh/install | bash
--------------------------
source ~/.bashrc
--------------------------
bun --version
--------------------------
cd ../cli/
bun install
--------------------------
bash script/transact.sh  / executing a transaction
```

## DONE! 


#### Additional links Seismic Devnet:
```
Network Name: Seismic devnet

Currency Symbol: ETH

Chain ID: 5124

RPC URL (HTTP): https://node-2.seismicdev.net/rpc

RPC URL (WebSocket): wss://node-2.seismicdev.net/ws

Explorer: https://explorer-2.seismicdev.net

Faucet: https://faucet-2.seismicdev.net

Starter Repo: https://github.com/SeismicSystems/seismic-starter
```
## MY X: https://x.com/o7xabz
