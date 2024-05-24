# lodestar-cheat-sheet
- https://chainsafe.github.io/lodestar/

<br><br>

# Install

<br><br>

## Quickstart scripts
- Will run the Consensus clients and the etherem client
```shell
sudo apt install gnome-terminal
git clone https://github.com/ChainSafe/lodestar-quickstart.git

# Non Silent
./setup.sh --dataDir sepolia-data --elClient nethermind --network sepolia --withTerminal "gnome-terminal --disable-factory --" --dockerWithSudo

# Silent
./setup.sh --dataDir sepolia-data --elClient nethermind --network sepolia --detached --dockerWithSudo
```
