# SpookNetwork
> [!IMPORTANT]
> Follow step by step to make a Minecraft Server or you will mess up.

## Installing Java 21
```bash
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install ca-certificates apt-transport-https gnupg wget
```
```bash
wget -O - https://apt.corretto.aws/corretto.key | sudo gpg --dearmor -o /usr/share/keyrings/corretto-keyring.gpg && \
echo "deb [signed-by=/usr/share/keyrings/corretto-keyring.gpg] https://apt.corretto.aws stable main" | sudo tee /etc/apt/sources.list.d/corretto.list
```
```bash
sudo apt-get update
sudo apt-get install -y java-21-amazon-corretto-jdk libxi6 libxtst6 libxrender1
```
## Verifiying installation
```bash
java -version
```
> [!Should Say This]
> openjdk version "21" 2025-10-19 LTS ###Time will be different
> OpenJDK Runtime Environment Corretto-21.0.0.35.1 (build 21+35-LTS)
> OpenJDK 64-Bit Server VM Corretto-21.0.0.35.1 (build 21+35-LTS, mixed mode, sharing)
## Step 1: Download Paper
```bash
wget https://api.papermc.io/v2/projects/paper/versions/1.21/builds/130/downloads/paper-1.21-130.jar
```
> Note: make sure to rename the file downloaded to "paper.jar"
## Step 2: Start Server
```bash
java -Xmx16G -Xms4G -jar paper.jar --nogui
```
## To Close Use
```bash
stop
```
