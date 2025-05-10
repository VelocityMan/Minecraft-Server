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
> It's going to ask you to accept the eula, to accept find "eula.txt" and make sure its set to: eula=true

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

## You can add custom domains to your minecraft server by doing these steps:
download this plugin and drag it in your plugins folder
https://github.com/playit-cloud/playit-minecraft-plugin/releases/latest/download/playit-minecraft-plugin.jar

Afterwards stop and start your minecraft server by using the commands listed on Startup.
> when you run this command you will see many messages that are spamming again like:
[gg.playit.minecraft.PlayitKeysSetup] trying to exchange claim code for secret
[gg.playit.minecraft.PlayitKeysSetup] failed to exchange, to claim visit: https://playit.gg/mc/"yourcode"
> click into the link like that to make agent in playit.gg but you have to have an account in playit.gg first
when you done adding agent go to the agent section in playit.gg website, click into the agent you created for minecraft server, scroll down to the bottom and click "add tunnel", when adding tunnel, keep the region is global because it's free, change the tunnel type to "Minecraft java(game)" and then wait for it to create the tunnel, after that in tunnel you will see 2 ip like "africa-champion.gl.joinmc.link" or "147.185.221.20:38120", copy one of these 2 ip and join minecraft server normally.

> Afterwards, get the number ip you got example: "147.185.221.20:38120"
> Go to https://shockbyte.com/subdomain-creator
> Put your email doesn't matter what email you put.
> Enter the number ip example: "147.185.221.20"
> Enter the port: "38120"

> Now Choose your domain name and server name! Enjoy your domain!

## Making the server last longer
By default github stops your codespace if your not using it for 30 minutes.
But, you can change this to 4 hours by following the steps below:
> Go to settings, click "Codespaces" under the "Code, planning, and automation"
> Scroll down to "Default idle timeout" and set it to 240 minutes aka 4 hours

