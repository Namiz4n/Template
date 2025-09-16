<p align="center">
  <a href="https://github.com/Namiz4n/Template/tree/master/singbox" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://sing-box.sagernet.org/assets/icon.svg">
      <img width="160" height="160" src="https://sing-box.sagernet.org/assets/icon.svg">
    </picture>
  </a>
</p>
<h1 align="center"/>Sing-box Config Example for <a href="https://github.com/Gozargah/Marzban">Marzban</a></h1>

<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation Steps](#installation-steps)
- [Sing-box Download Link](https://github.com/SagerNet/sing-box)

# Introduction
Sing-box is a rule-based proxy that allows you to configure program settings such as DNS, routing, and more from the server side. In this template, Sing-box is configured server-side to establish direct connections to local (internal) websites.  
One of the most notable features of the Sing-box client is its support for multiple platforms, including Android, iOS, macOS, and more.

# Features
- Connects to the fastest configuration.
- Directly accesses Iranian websites when the VPN is active.
- Blocks advertisements.  
And more.

# Installation Steps
1. Download the template file.
```sh
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/Namiz4n/Template/master/singbox/default.yml
```
2. Run the following commands in your server terminal:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.yml"' | sudo tee -a /opt/marzban/.env
```
Alternatively, add the following values to the .env file located in the /opt/marzban directory:
```sh
sudo nano /opt/marzban/.env
```
```sh
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/default.yml"
SINGBOX_SETTINGS_TEMPLATE="singbox/settings.json"
```

3. Restart Marzban:
```sh
marzban restart
```

## Updating
To update the templates, simply repeat step 1.


# Support
<a href="https://nowpayments.io/donation?api_key=J5CVKFP-7ENME50-QDF7XGZ-2S74E0B" target="_blank" rel="noreferrer noopener"> <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments"> </a>
