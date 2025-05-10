# Minecraft Server [![Discord](https://img.shields.io/discord/1225272078752813178?label=Discord)](https://discord.gg/m6vCCX6Hvr) [![YouTube](https://img.shields.io/youtube/channel/subscribers/UCwSd8pbURlMBAIxqq8EaELw?style=flat-square&label=Subscribers)](https://www.youtube.com/@ismaeltechI?sub_confirmation=1)
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
> openjdk version "21" 2025-10-19 LTS
> OpenJDK Runtime Environment Corretto-21.0.0.35.1 (build 21+35-LTS)
> OpenJDK 64-Bit Server VM Corretto-21.0.0.35.1 (build 21+35-LTS, mixed mode, sharing)
## Download Paper
```bash
wget https://api.papermc.io/v2/projects/paper/versions/1.21/builds/130/downloads/paper-1.21-130.jar
```
> Note: make sure to rename the file downloaded to "paper.jar"
## Startup
```bash
java -Xmx16G -Xms4G -jar paper.jar --nogui
```
> Servers that Has 8 Ram & 2 CPU cores
```bash
java -Xmx8G -Xms4G -jar paper.jar --nogui
```
## Closing The Server
```bash
stop
```

## Optional Settings:
GitHub will use 8 gb rams and 2 cores in cpu as default so you have to change it.
> to change follow these steps:
go back to the repository page and then find the code with green color button then go to the codespaces section, under the on current branch, find your codespace with uncommitted changes phase, click 3 dots button then stop the codespace, after that the website will refresh and click again that 3 dots, click into change machine type, change to 4-core then update codespace then well done.
