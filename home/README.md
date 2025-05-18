<p align="center">
  <a href="https://github.com/Namiz4n/Template/tree/master/home" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Namiz4n/Template/master/home/preview.gif">
      <img width="363" height="328" src="https://raw.githubusercontent.com/Namiz4n/Template/master/home/preview.gif">
    </picture>
  </a>
</p>
<h1 align="center"/>Home Page Template for the <a href="https://github.com/Gozargah/Marzban">Marzban</a> Panel</h1>

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
- [Installation Steps](#installation-steps)

# Introduction
A simple HTML template for the Marzban home page.

# Installation Steps
1. Download the template file.

```sh
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/Namiz4n/Template/master/home/index.html
```

2. Run the following commands in your server terminal:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'HOME_PAGE_TEMPLATE="home/index.html"' | sudo tee -a /opt/marzban/.env
```
Alternatively, add the following values to the .env file located in the /opt/marzban directory:
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
HOME_PAGE_TEMPLATE="home/index.html"
```

3. Restart Marzban:
```sh
marzban restart
```

## Updating
To update the templates, simply repeat step 1.


# Support

<a href="https://nowpayments.io/donation?api_key=J5CVKFP-7ENME50-QDF7XGZ-2S74E0B" target="_blank" rel="noreferrer noopener">
  <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments"> </a>
