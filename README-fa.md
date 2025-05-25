<p align="center">
  <a href="https://github.com/Namiz4n/Template/" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
      <img width="160" height="160" src="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
    </picture>
  </a>
</p>
<h1 align="center"/>تمپلیت های مختلف برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>
<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>

# مقدمه
لیستی از تمپلیت های شخصی سازی شده برای مرزبان

# لیست تمپلیت ها
- [صفحه خانه](https://github.com/Namiz4n/Template/tree/master/home)
- [صفحه سابسکریپشن](https://github.com/Namiz4n/Template/tree/master/subscription)
- [تمپلیت برای v2ray](https://github.com/Namiz4n/Template/tree/master/Xray)
- [تمپلیت برای sing-box](https://github.com/Namiz4n/Template/tree/master/Singbox)
- [تمپلیت برای Clash](https://github.com/Namiz4n/Template/tree/master/Clash)

# مراحل نصب
برای نصب هر تمپلیت به صفحه مربوط به آن مراجعه کنید

# نصب همه
برای نصب همه تمپلیت های موجو دستورات زیر را در ترمینال سرور خود اجرا کنید:
1. دانلود فایل های تمپلیت
```sh
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/Namiz4n/Template/master/home/index.html
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/Namiz4n/Template/master/subscription/index.html
sudo wget -N -P /var/lib/marzban/templates/xray/ https://raw.githubusercontent.com/Namiz4n/Template/master/v2ray/template.yml
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/Namiz4n/Template/master/singbox/template.yml
sudo wget -N -P /var/lib/marzban/templates/clash/ https://raw.githubusercontent.com/Namiz4n/Template/master/clash/template.yml
```
2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
echo 'SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/template.yml"' | sudo tee -a /opt/marzban/.env
echo 'V2RAY_SUBSCRIPTION_TEMPLATE="v2ray/template.yml"' | sudo tee -a /opt/marzban/.env
echo 'CLASH_SUBSCRIPTION_TEMPLATE="clash/template.yml"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
SINGBOX_SUBSCRIPTION_TEMPLATE="singbox/template.yml"
V2RAY_SUBSCRIPTION_TEMPLATE="v2ray/template.yml"
CLASH_SUBSCRIPTION_TEMPLATE="clash/template.yml"

```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت ها فقط کافیست مرحله 1 را تکرار کنید.

# حمایت از من

<a href="https://nowpayments.io/donation?api_key=J5CVKFP-7ENME50-QDF7XGZ-2S74E0B" target="_blank" rel="noreferrer noopener"> <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments"> </a>
