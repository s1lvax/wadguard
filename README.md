# Wadguard
## The easiest way to run Wireguard VPN/UI + Adguard Home AdBlocker

Disclaimer : This repository is merely a mix of 2 well developed repositories (Wg-Easy and AdguardHome). I do not claim credit for those repos, all I did was put them together in an accessible way.

## Features

* All-in-one: WireGuard + Web UI.
* Easy installation, simple to use.
* List, create, edit, delete, enable & disable clients.
* Show a client's QR code.
* Download a client's configuration file.
* Statistics for which clients are connected.
* Tx/Rx charts for each connected client.
* Ad Blocker
* DNS Filtering
* Parental Control
* ...all Adguard features

## Requirements

* A host with a kernel that supports WireGuard (all modern kernels).
* A host with Docker installed.

## Installation

1. Clone this repository into your host machine using ```git clone https://github.com/s1lvax/wadguard```
2. Create 3 folders : work, conf, wg.
3. If you have another app using port 53, you need to disable it.
4. Configure the docker-compose for your specific use case (WG_HOST, Password)
5. Run the docker compose using ```docker-compose up -d```
6. Visit HOST_IP:3000 and finish configuring Adguard Home.
7. Wg_Easy should be accessible at HOST_IP:51821, access it and start creating users.
8. Connect to your VPN and have fun :).

## Guidelines

Your Adguard Home dashboard is available at http://10.2.0.100 when connected to the Wireguard server.
