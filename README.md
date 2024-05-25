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

## Kill
```(base)  ✘   ~/Projects/lodestar-quickstart   main  sudo docker ps              
CONTAINER ID   IMAGE                          COMMAND                  CREATED          STATUS              PORTS     NAMES
470c3ccbd1e3   chainsafe/lodestar:latest      "node ./packages/cli…"   48 minutes ago   Up 11 minutes                 sepolia-lodestar
a7cf575343e3   nethermind/nethermind:latest   "./nethermind --conf…"   48 minutes ago   Up About a minute             sepolia-nethermind
(base)    ~/Projects/lodestar-quickstart   main  sudo docker stop 470c3ccbd1e3
470c3ccbd1e3
(base)   ~/Projects/lodestar-quickstart   main  sudo docker stop a7cf575343e3 
a7cf575343e3
(base)    ~/Projects/lodestar-quickstart   main  sudo docker ps                
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
(base)    ~/Projects/lodestar-quickstart   main  
                                                    
```
