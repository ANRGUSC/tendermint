## SwarmDAG: A Partition Tolerant Distributed Ledger Protocol for Swarm Robotics

Blockade uses iproute2 and tc to control the network partitions and connections.

First install requirements:

    sudo pip3 install requirements.txt

Pre-generate tendermint configs for nodes by running this locally. This will 
create a build/ folder with subfolders for each node. Modify the starting IP 
address depending on your docker's bridge IP.

    tendermint testnet --v 10 --o ./build --populate-persistent-peers --starting-ip-address 172.17.0.2

Blockade supports Docker links which are now deprecated so you may need to 
install an older verison of Docker if you want to use this. 