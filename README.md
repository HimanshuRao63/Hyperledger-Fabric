# Hyperledger-Fabric

## 1. Install Golang  
```bash
sudo apt install golang-go
```
Installs Golang, which is necessary for running Hyperledger Fabric binaries.

**Screenshot **: 

![Screenshot 2025-04-13 130047](https://github.com/user-attachments/assets/34277b4b-807e-407e-a0a1-15625793b47d)


---

## 2. Check Docker Version  
```bash
docker --version
```
Verifies that Docker is installed and running correctly.

**Screenshot **: 

![Screenshot 2025-04-13 161049](https://github.com/user-attachments/assets/893cb8a2-050b-434c-9350-4c76be8bb23c)
_

---

## 3. Check Docker Compose Version  
```bash
docker compose version
```
Verifies the installation of Docker Compose.

**Screenshot **:

![Screenshot 2025-04-13 161201](https://github.com/user-attachments/assets/d6bc63c1-dd15-46f3-a902-04e4dc1d3f41)


---

## 4. List Files in Current Directory  
```bash
ls
```
Shows the list of files and folders in the current directory.

---

## 5. Clone the Fabric Samples Repository and Move into the Cloned Folder  
```bash
git clone https://github.com/fabric-samples.git; cd fabric-samples
```
Downloads the official Hyperledger Fabric sample code from GitHub.  
Enters the cloned folder where Fabric examples are available.

**Screenshot **: 

![Screenshot 2025-04-13 161348](https://github.com/user-attachments/assets/997a447c-38f7-44c0-b18b-5bb380382f24)


---

## 6. Download Fabric Binaries  
```bash
curl -sSL https://bit.ly/2ysbOFE | bash -s
```
Downloads necessary Fabric binaries and Docker images like peer, orderer, and cryptogen.

**Screenshot **:

![Screenshot 2025-04-13 163554](https://github.com/user-attachments/assets/603a1a43-1e3f-44fb-bc62-f5e0691a3e10)
![Screenshot 2025-04-13 171636](https://github.com/user-attachments/assets/a2642bf3-6a0f-4a9f-9df1-ad7fc2f5d3a5)
![Screenshot 2025-04-13 171730](https://github.com/user-attachments/assets/b9f5863c-e5e5-4ebf-8135-b972c148974c)
![Screenshot 2025-04-13 171749](https://github.com/user-attachments/assets/7cdb4657-5e46-47dc-97be-b61009d92d27)


---

## 7. Enter the Test Network Directory  
```bash
cd test-network
```
Navigates to the directory that contains scripts for running a sample Fabric network.

**Screenshot **:

![Screenshot 2025-04-13 163740](https://github.com/user-attachments/assets/948647e5-a691-4031-ba2f-efdccd197549)


---

## 8. View the Network Script  
```bash
./network.sh
```
Shows the options available with the `network.sh` script.

**Screenshot **: 

![Screenshot 2025-04-13 172111](https://github.com/user-attachments/assets/bf6836bf-87e9-4daa-a4cb-a4ea6eafa4c4)
![Screenshot 2025-04-13 172147](https://github.com/user-attachments/assets/f2e9338e-956e-4685-b909-a7f8d02d7225)


---

## 9. Start the Fabric Network  
```bash
./network.sh up
```
Starts the network by launching peer, orderer, and CA containers, and generates the required cryptographic materials.

**Screenshot **: 
![Screenshot 2025-04-13 172259](https://github.com/user-attachments/assets/94373585-61e5-4cf1-912e-324a7814864c)

---

## 10. Create a Channel  
```bash
./network.sh createChannel
```
Creates a default channel (usually named `mychannel`) and joins the peers to it.

**Screenshot **: 
![Screenshot 2025-04-13 172952](https://github.com/user-attachments/assets/debbfd28-95fa-407c-ac39-0439d20b8bed)
![Screenshot 2025-04-13 173050](https://github.com/user-attachments/assets/371e77a4-b7c4-45c2-b98d-d0fc88c83ac0)


---

## 11. Shut Down the Network  
```bash
./network.sh down
```
Stops all containers and deletes the crypto material and artifacts created during the setup.

**Screenshot **: 
![Screenshot 2025-04-13 173229](https://github.com/user-attachments/assets/2db9a0b7-3949-4f55-b777-0e457bbc97e0)

---

