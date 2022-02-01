Steps to setup own Cardano Node on windows:

1. https://developers.cardano.org/docs/get-started/cardano-components/

2.  download cardano executable file 

3. create a batch file with the following commands: eg. run-node.bat.

cardano-node run --topology "configuration\cardano\mainnet-topology.json" --database-path "db" --socket-path "\\.\pipe\cardano" --host-addr 192.168.0.1 --port 3000 --config "configuration\cardano\mainnet-config.json"

4. create a database folder with the path. eg db.

5. run CMD as an Administrator to run "run-node.bat" file.

Query Cardano Node

1. Use the cardano-cli 

2. set up environment variable "CARDANO_NODE_SOCKET_PATH" 

3. Type sysdm.cpl in console --> environment variables 

4. set path "CARDANO_NODE_SOCKET_PATH" and value : "\\.\pipe\cardano"

5. Open another console window type command in root folder: "cardano-cli query tip" --mainnet 

