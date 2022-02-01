Steps to setup own Cardano Node on windows:

1. https://developers.cardano.org/docs/get-started/cardano-components/

2.  download cardano executable file 

3. create a batch file with the following commands: eg. run-node.bat.

cardano-node run --topology "configuration\cardano\testnet-topology.json" --database-path "db" --socket-path "\\.\pipe\cardano" --host-addr 192.168.0.1 --port 3000 --config "configuration\cardano\testnet-config.json"

4. create a database folder with the path. eg db.

5. run CMD as an Administrator to run "run-node.bat" file.



![img](https://user-images.githubusercontent.com/90293555/151898424-98144d63-365b-4bec-872c-73e37c275d5b.jpg)



![img1](https://user-images.githubusercontent.com/90293555/151898471-3a4363d4-bfbe-4434-bc10-aa96ef178c1e.jpg)

Query Cardano Node:


1. Use the cardano-cli 

2. set up environment variable "CARDANO_NODE_SOCKET_PATH" 

3. Type sysdm.cpl in console --> environment variables 

4. set path "CARDANO_NODE_SOCKET_PATH" and value : "\\.\pipe\cardano"

5. Open another console window type command in root folder: "cardano-cli query tip" --testnet 


![img2](https://user-images.githubusercontent.com/90293555/151898509-4eb659ec-bc87-40ec-b6ba-0a548de65eac.jpg)



