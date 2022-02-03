CARDANO BLOCKCHAIN

Description

Cardano is a public blockchain platform. It is open-source and decentralized, with consensus achieved using proof of stake. 
It can facilitate peer-to-peer transactions with its internal cryptocurrency, ADA

Steps to setup own Cardano Node Mainnet and Testnet on windows:

1. https://developers.cardano.org/docs/get-started/cardano-components/

2.  download cardano executable file 

3. create a batch file with the following commands: eg. run-node.bat.

cardano-node run --topology "configuration\cardano\mainnet-topology.json" --database-path "db" --socket-path "\\.\pipe\cardano" --host-addr 192.168.0.1 --port 3000 --config "configuration\cardano\mainnet-config.json"

4. create a database folder with the path. eg db.

5. run CMD as an Administrator to run "run-node.bat" file.


MAINNET
![img](https://user-images.githubusercontent.com/90293555/151898424-98144d63-365b-4bec-872c-73e37c275d5b.jpg)

![img1](https://user-images.githubusercontent.com/90293555/151898471-3a4363d4-bfbe-4434-bc10-aa96ef178c1e.jpg)

TESTNET:

![img6](https://user-images.githubusercontent.com/90293555/152064205-f4fdefe2-8bfd-495b-9b78-19edce7b760c.jpg)




Query Cardano Node:


1. Use the cardano-cli 

2. set up environment variable "CARDANO_NODE_SOCKET_PATH" 

3. Type sysdm.cpl in console --> environment variables 

4. set path "CARDANO_NODE_SOCKET_PATH" and value : "\\.\pipe\cardano" or "\\.\pipe\cardano-node-testnet"

5. Open another console window type command in root folder: "cardano-cli query tip" --mainnet / cardano-cli query tip --testnet-magic 1097911063

MAINNET:

![img2](https://user-images.githubusercontent.com/90293555/151898509-4eb659ec-bc87-40ec-b6ba-0a548de65eac.jpg)

![img](https://user-images.githubusercontent.com/90293555/151906674-277ad509-defd-412f-a797-ec29bc0eb20d.jpg)

TESTNET: 

![img7](https://user-images.githubusercontent.com/90293555/152064361-b6ea59f8-dc85-45eb-8a19-9aa6e405f9ac.jpg)

![img8](https://user-images.githubusercontent.com/90293555/152064317-3ddb8167-6016-4e2d-97bc-a47d3dbfe082.jpg)


1. download windows zip from: https://github.com/input-output-hk/cardano-wallet/releases

2. create a Wallet folder and extract files 

3. create batch file for running wallet : cardano-wallet serve --listen-address 127.0.0.1 --port 8090 --node-socket "\\.\pipe\cardano" --mainnet --database "wallets"  //run-wallet.bat / or   create batch file for running wallet : cardano-wallet serve --listen-address 127.0.0.1 --port 8090 --node-socket "\\.\pipe\cardano" --testnet --database "wallets"  //run-wallet.bat 

4. create database folder to match --database

5.  Open another console window type command in root folder for Wallet: run-wallet

image:

![img3](https://user-images.githubusercontent.com/90293555/151906597-6bc486aa-a444-4269-850b-fc673e3cdb68.jpg)

6. Create wallet : WALLET_NAME, recovery-phrase, Passphrase

7. Generate recovery phrase 
cardano-wallet recovery-phrase generate

 "favorite correct plunge ketchup travel borrow laugh illegal sure magnet thank ankle confirm example fix social chair shop tooth canal tenant success fine panel"

 8. Enter "cardano-wallet wallet create from-recovery-phrase AlWallet"

 9. Enter recovery phrase

 10. Enter passphrase
 
 
 ![img9](https://user-images.githubusercontent.com/90293555/152074787-ff6a2119-ff33-4670-9095-4d914f0e6a84.jpg)


![img4](https://user-images.githubusercontent.com/90293555/151906614-b1d2cd69-969b-471f-b5a3-55635af27008.jpg)

![img5](https://user-images.githubusercontent.com/90293555/151906623-bf31d378-1268-48ad-93e1-32d57405689c.jpg)

 
