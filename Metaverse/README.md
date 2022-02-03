
DEPLOYED DECENTRALAND LAND SMART CONTRACT USING HARDHAT AND RUN CATALYST NODE USING UBUNTU v20.4


Description:

Decentraland is a 3D virtual world platform. Users may buy virtual plots of land in the platform as NFTs via the MANA cryptocurrency, which uses the Ethereum blockchain.


![image](https://user-images.githubusercontent.com/90293555/152284601-0a6a689b-70de-4aff-8093-9fccb71b8f7a.png)


#  Hardhat Project

![image](https://user-images.githubusercontent.com/90293555/152399521-fb2aefef-62d1-4ceb-948d-bffcc3d188b9.png)


This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, a sample script that deploys that contract, and an example of a task implementation, which simply lists the available accounts.

Try running some of the following tasks:

```shell
npx hardhat accounts
npx hardhat compile
npx hardhat clean
npx hardhat test
npx hardhat node
node scripts/sample-script.js
npx hardhat help
```
Setup Hardhat Project

1. npm install --save-dev hardhat

2. npx hardhat

3. Create Deploy.js to deploy contract 

4. Add .env that include Ropsten test "PUBLIC_KEY" "PRIVATE_KEY" 

![image](https://user-images.githubusercontent.com/90293555/152399599-e944c940-0da4-4b36-9829-0e53404f1854.png)


    "API_URL" - this using infura API @ https://infura.io/

5. Update Harhat.config file with .env const. and the Solidity version 

    to match the contracts pragma.

6. npm install "dotenv" and "@nomiclabs/hardhat-ethers" 

    "openzeppelin-zos" "ethers"

7. update config file with multiple compilers to match contract files.

error: 
    Please replace LANDRegistry for one of these options wherever you are trying to read its artifact:

    contracts/estate/EstateStorage.sol:LANDRegistry
    contracts/land/LANDRegistry.sol:LANDRegistry

    SOLVED: adjust the contract name in the Estate contract

    Error HH606: The project cannot be compiled, see reasons below.

    The Solidity version pragma statement in these files doesn't match any of the configured compilers in your config. Change the pragma or configure additional compiler versions in your hardhat config.

    SOLVED: add multiple compilers


8. RUN:  npx hardhat run scripts/deploy.js --network ropsten

    error: ProviderError: max code size exceeded











------------------------------------------------------------------------------------------------------------------



#  Truffle Project



Steps:

![image](https://user-images.githubusercontent.com/90293555/152398534-893a90c7-9616-4aff-a644-5f30ed66f297.png)


truffle init

npm install @truffle/hdwallet-provider

npm babel-register

npm install babel-polyfill

npm install erc821


npm install dotenv


npm install openzeppelin-zos


update config file with package 


update config file with compiler versions


update config file https://ropsten.infura.io/v3/a5810a1d99f246608d85248e4c20594d"

![image](https://user-images.githubusercontent.com/90293555/152398583-3bd6db03-cff6-43d3-9eed-85d9798145b7.png)


run Ganache : ganache-cli

![image](https://user-images.githubusercontent.com/90293555/152398444-97e55f53-b410-4042-b9c2-da3fe9e30814.png)


truffle compile


truffle migrate 





 Deploying 'LANDRegistry'
   ------------------------

Error:  *** Deployment Failed ***

"LANDRegistry" ran out of gas (using a value you set in your network config or deployment parameters.)
   * Block limit:  6721975 (0x6691b7)
   * Gas sent:     20000000000 (0x4a817c800)
-----------------------------------------------------------------------------------------------------------------------






#  Catalyst Node Project

![image](https://user-images.githubusercontent.com/90293555/152284559-e2292c4d-1ce6-48de-8680-274ca7a50039.png)

Setting up a Catalyst Node on Ubuntu 20.4 using virtualbox

![image](https://user-images.githubusercontent.com/90293555/152399464-7a546ee3-e409-4fa7-a15e-246c34af435b.png)



1. Install Docker

2. Install Docker-Compose

3. Add $USER to Docker Group

4. Verify Docker Install

5. Verify Docker-Compose Install

6. Stop Apache2

7. Install Git

8. Create Directory for Catalyst Source Code

9. Download Catalyst-Owner from Decentraland's Github

11. Edit Environment File .env

12. Create Storage Folder

13. Bridge the connection for the virtual machine 

error : 

![img](https://user-images.githubusercontent.com/90293555/152281203-7d45ae1b-2867-48af-ad98-f4f82c32773b.jpg)

SOLVED:

run mv .env-advanced.example .env-advanced in catalyst-owner  folder and then run mkdir storage

![img2](https://user-images.githubusercontent.com/90293555/152281600-9be61717-2a66-40d3-93bc-f2b71af3635a.jpg)

Final message to confirm that the server is functioning:

// Catalyst server is up and running at http://localhost


![img3](https://user-images.githubusercontent.com/90293555/152281785-51106824-b01b-49f2-b0b5-b5cabdcb5756.jpg)


![img4](https://user-images.githubusercontent.com/90293555/152284083-3f07befb-8fe9-4f8a-b416-fd5931f79107.jpg)


credit : https://www.reddit.com/r/decentraland/comments/m0xujc/decentralizing_decentraland_content_setting_up_a/
