<p align="center">
  <a href="https://github.com/Namiz4n/Template/tree/master/home" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Namiz4n/Template/master/home/preview.gif">
      <img width="363" height="328" src="https://raw.githubusercontent.com/Namiz4n/Template/master/home/preview.gif">
    </picture>
  </a>
</p>
<h1 align="center"/>قالب صفحه خانه برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>

<p align="center">
 <a href="./README.md">
 English
 </a>
 /
 <a href="./README-fa.md">
 فارسی
 </a>
</p>

## فهرست مطالب
- [مقدمه](#مقدمه)
- [مراحل نصب](#مراحل-نصب)

# مقدمه
یک قالب html ساده برای صفحه خانه مرزبان

# مراحل نصب
1. دانلود فایل template
```sh
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/Namiz4n/Template/master/home/index.html
```

2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'HOME_PAGE_TEMPLATE="home/index.html"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
HOME_PAGE_TEMPLATE="home/index.html"
```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت فقط کافیست مرحله 1 را تکرار کنید.



# حمایت از من

<a href="https://nowpayments.io/donation?api_key=J5CVKFP-7ENME50-QDF7XGZ-2S74E0B" target="_blank" rel="noreferrer noopener"> <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments"> </a>
