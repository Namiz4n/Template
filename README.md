<p align="center">
  <a href="https://github.com/Namiz4n/Template/" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
      <img width="160" height="160" src="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
    </picture>
  </a>
</p>
<h1 align="center">Various templates for the <a href="https://github.com/Gozargah/Marzban">Marzban</a> panel</h1>

<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>

# Introduction
A list of customized templates for Marzban

# List of Templates
- [Home Page](https://github.com/Namiz4n/Template/tree/master/home)
- [Subscription Page](https://github.com/Namiz4n/Template/tree/master/subscription)
- [Template for v2ray](https://github.com/Namiz4n/Template/tree/master/Xray)
- [Template for sing-box](https://github.com/Namiz4n/Template/tree/master/Singbox)
- [Template for Clash](https://github.com/Namiz4n/Template/tree/main/clash)

# Installation Steps
To install each template, refer to its respective page

# Install All
To install all available templates, execute the following commands in your server's terminal:
1. Download the template files
```sh
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/Namiz4n/Template/master/home/index.html
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/Namiz4n/Template/master/subscription/index.html
sudo wget -N -P /var/lib/marzban/templates/xray/ https://raw.githubusercontent.com/Namiz4n/Template/master/v2ray/template.yml
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/Namiz4n/Template/master/singbox/template.yml
sudo wget -N -P /var/lib/marzban/templates/clash/ https://raw.githubusercontent.com/Namiz4n/Template/master/clash/template.yml
```

2.Run the following commands in your server's terminal:
```
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/template.yml"' | sudo tee -a /opt/marzban/.env
echo 'V2RAY_SUBSCRIPTION_TEMPLATE="v2ray/template.yml"' | sudo tee -a /opt/marzban/.env
echo 'CLASH_SUBSCRIPTION_TEMPLATE="clash/template.yml"' | sudo tee -a /opt/marzban/.env
```

Or add the following values to the `.env` file in the `/opt/marzban` directory
```
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/template.yml"
V2RAY_SUBSCRIPTION_TEMPLATE="v2ray/template.yml"
CLASH_SUBSCRIPTION_TEMPLATE="clash/template.yml"
```
3.Restart Marzban
```
marzban restart
```
## update
 
To update the templates, simply repeat step 1.

# Support Me

<a href="https://nowpayments.io/donation?api_key=J5CVKFP-7ENME50-QDF7XGZ-2S74E0B" target="_blank" rel="noreferrer noopener"> <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments"> </a>
