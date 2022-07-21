# Ptero Modified Stats ( A fork of HirziDevs-PteroStats )


![Version](https://img.shields.io/github/package-json/v/HirziDevs/PteroStats?style=flat-square)
![License](https://img.shields.io/github/license/HirziDevs/PteroStats?style=flat-square)

![PteroStats Banner](https://media.discordapp.net/attachments/796259732683227157/861126504246411264/20210704_130856.jpg)

## Info

I am Not Owner of PteroStats, i have just increased its security like i added env, so if you host the bot at a Public Online IDE, So people cant get your bot token or panel api key.

[Real Repo Here](https://github.com/HirziDevs/PteroStats) 

## Introduction

PteroStats is a bot designed to check Pterodactyl Panel and Nodes status and post it to your discord server

- Written in Javascript, CloudServer is faster and more stable.
- PteroControl can be used with any server on Pterodactyl, irregardless of whether it's on shared hosting or your own hosted panel

PteroStats is still **under development** and we welcome contributions. 

### How it works?

PteroStats checks [Pterodactyl](https://pterodactyl.io) nodes wings with [Axios](https://www.npmjs.com/package/axios) to get nodes wings status, if the api didn't reply that mean the node is having [Wings/Daemon](https://pterodactyl.io/wings/1.0/installing.html) down and mark the node as offline.


## Installation

- `fill in the required informations in the config.yml file`
- `Run npm install in the root directory of the bot files`
- `Run node index.js and you are done`

if you need help contact me on discord `KRD66778#8419` or join [our discord server here](https://discord.gg/4rQpVzpzX7)

## Admin Apikey Permission

enable `read` on all options, if still didn't work enable `read & write` on all options
![Admin Apikey Permission](https://media.discordapp.net/attachments/819757140155564062/876320084992331816/Screenshot_2021-08-15-11-20-05-56.jpg)

### Setuping Config

You need to put right config to make the bot work at [config.yml](https://github.com/KRD66778/PteroStats/blob/main/config.yml) file
```
# PteroStats config
# If you need help, join my discord server: https://discord.gg/4rQpVzpzX7

# Bot Info's
botstatus:
  enable: false # Enable Custom Status (MUST BE "true" OR "false")
  text: 'Hosting Panel' # Bot Status Message
  type: 'WATCHING' # Bot Status Type. Ex: PLAYING, WATCHING, LISTENING, STREAMING

# Channel and RefreshTime Configuration
channel: 'CHANNEL ID' # Put channel id here where the embed will be sended
refreshtime: 10 # Time when the embed edited/refreshed (MUST BE A SECONDS) (RECOMMENDED MORE THAN 20 SECONDS)


# Embed Configuration
embed: 
  title: 'EMBED TITLE' # Embed Title here. Ex: PureNodes Stats
  color: 'E5BE11' # Embed Hex color here.
  description: 
    enable: false # Enable Embed Description (MUST BE "true" OR "false")
    text: 'EMBED DESCRIPTION' # Embed Description
  footer: 
    enable: true # Enable Embed Footer (MUST BE "true" OR "false")
    text: 'Your host name' # Embed Footer
  timestamp: true # Enable Embed TimeStamp (MUST BE "true" OR "false")

# Status Message Configuration
status:
  online: ':green_circle: Online' # Message if the status is Online
  offline: ':red_circle: Offline' # Message if the status is Offline
  check: ':orange_circle: Checking' # Message if the status is Checking

# Node Resource
resource:
  enable: true # Enable resource option ex [Ram: 2gb/5gb] bellow node name (MUST BE "true" OR "false")
  servers: true # Enable Total server on the node to resource text (MUST BE "true" OR "false")
  allocations: true # Enable Total Allocation on the node to resource text (MUST BE "true" OR "false")
  location: true # Enable location short name on the node to resource text (MUST BE "true" OR "false")
  unit: 'gb' # Must be 'mb', 'gb', or 'percent'

# Developers feature
debug: true # Enable and Disable debug log to console
debugaxios: false #Enable and Disable axios error logs
```

## Other
### FAQ

Q: Can i use pterodactyl v0.7?

A: No, the pterodactyl v0.7 is not supported


Q: How i can get support?

A: You can join our [discord server](https://discord.gg/4rQpVzpzX7)

### Links

* __[My Own Discord](https://discord.gg/4rQpVzpzX7)__
* __[PteroBot Discord](https://discord.gg/zv6maQRah3)__
* __[Pterodactyl Panel](https://pterodactyl.io)__
* __[Pterodactyl API](https://dashflo.net/docs/api/pterodactyl/v1)__

### Special Thanks to

- Hirzi Devs and his Team
