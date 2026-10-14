<div align="center">

# 🏛️ Apadana Template | تمپلیت آپادانا
### قالب اختصاصی، پرسرعت و مدرن صفحه اشتراک برای پنل‌های ربکا، مرزبان و پاسارگاد

![Version](https://img.shields.io/badge/version-3.0.0-gold?style=for-the-badge)
![Engine](https://img.shields.io/badge/Engine-Pongo2%20%7C%20Jinja2-blue?style=for-the-badge)
![Panel Support](https://img.shields.io/badge/Supports-Rebecca%20%7C%20Marzban%20%7C%20Pasarguard-00f0d6?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

<p align="center">
  <b>طراحی اصیل بر پایه هویت کهن پارسی، ترکیب طلای عیار بالا، لاجوردی شب، کارت‌های شیشه‌ای (Glassmorphism) و سبک مدرن بنتوگرید (Bento Grid).</b>
</p>

[پیش‌نمایش](#-پیشنمایش) • [ویژگی‌ها](#-ویژگیهای-برجسته) • [پروتکلها](#-پروتکلهای-پشتیبانیشده) • [راهنمای نصب](#-راهنمای-نصب)

---

</div>

## 📸 پیش‌نمایش

<div align="center">
  <img src="./preview.jpg" alt="Apadana Template Preview" width="380" style="border-radius: 20px; box-shadow: 0 10px 30px rgba(0,0,0,0.5);">
</div>

---

## ✨ ویژگی‌های برجسته

- 👑 **هویت بصری هخامنشی:** نشان برداری فروهر، خطوط کتیبه‌ای میخی و افکت متالیک طلای عیار بالا (Shimmer Foil).
- 📱 **اسکرول روان در موبایل:** رفع کامل باگ گیر کردن لمس و تداخل اسکرول در تمام مرورگرهای اندروید و iOS.
- ⚡ **دو نسخه مجزا برای سازگاری کامل:**
  - شاخه `main`: توسعه‌یافته با موتور **Pongo2** مخصوص پنل ربکا (Rebecca).
  - شاخه `master`: توسعه‌یافته با موتور **Jinja2** مخصوص مرزبان (Marzban) و پاسارگاد (Pasarguard).
- 🧩 **کاوشگر اختصاصی کانفیگ‌ها (Node Explorer):**
  - فهرست هوشمند کانفیگ‌ها با نام مرتب و نشان تفکیکی پروتکل‌ها.
  - جستجوگر سریع لوکیشن‌ها و نام سرورها.
  - فیلتر آنی بر اساس نوع پروتکل.
  - پنجره پاپ‌آپ (Modal) بارکد QR اختصاصی برای هر کانفیگ.
  - دکمه دانلود مستقیم برای پروتکل‌های فایلی (`.ovpn` و `.conf`).
- 🚀 **اتصال با یک کلیک (1-Click Connect):** دیپ‌لینک‌های مستقیم برای اپلیکیشن‌های Hiddify، v2rayNG، Shadowrocket و Sing-Box.
- 🔔 **فناوری صوتی Native Web Audio:** پخش بازخورد صوتی زنگ کهن هنگام لمس دکمه‌های کپی بدون نیاز به فایل صوتی خارجی.
- 🌐 **تشخیص هوشمند دامنه:** اصلاح خودکار آدرس‌های نسبی ساب‌اسکریپشن به نشانی کامل فعال در مرورگر کاربر.

---

## 🛰️ پروتکل‌های پشتیبانی‌شده

| پروتکل | نحوه نمایش و عملکرد |
| :--- | :--- |
| **VLESS** | نشان فیروزه‌ای نئونی + رونوشت سریع و QR اختصاصی |
| **VMess** | نشان طلایی هخامنشی + رمزگشایی متادیتای JSON |
| **Trojan** | نشان سرخ یاقوتی + کپی و بارکد مجزا |
| **Shadowsocks** | نشان بنفش متالیک + اسکن سریع |
| **OpenVPN (`.ovpn`)** | **نشان نارنجی + دکمه دانلود مستقیم فایل پروفایل** |
| **WireGuard (`.conf`)** | **نشان سرخ + دکمه دانلود مستقیم فایل کانکشن** |
| **Cisco AnyConnect** | نمایش گیت‌وی سرور سیسکو + رونوشت سریع |
| **PPTP / L2TP** | شناسایی آدرس سرور جهت راه‌اندازی دستی |

---

## 🚀 راهنمای نصب

### مرزبان (Marzban)

ابتدا قالب را با لینک زیر دانلود کنید:
```bash
sudo wget -N -P /var/lib/marzban/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)

سپس دستور زیر را بزنید تا تمپلیت ست شود:
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env

سپس با دستور زیر پنل خودتون رو ری‌استارت کنید:
marzban restart

ربکا (Rebecca)
ابتدا قالب را با لینک زیر دانلود کنید:
sudo wget -N -P /var/lib/rebecca/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html)

سپس دستور زیر را بزنید تا تمپلیت ست شود:
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/rebecca/templates/"' | sudo tee -a /opt/rebecca/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/rebecca/.env

سپس با دستور زیر پنل خودتون رو ری‌استارت کنید:
rebecca restart

پاسارگاد (Pasarguard)
ابتدا قالب را با لینک زیر دانلود کنید:
sudo wget -N -P /var/lib/pasarguard/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)

سپس دستور زیر را بزنید تا تمپلیت ست شود:
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/pasarguard/templates/"' | sudo tee -a /opt/pasarguard/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/pasarguard/.env

سپس با دستور زیر پنل خودتون رو ری‌استارت کنید:
pasarguard restart

📜 لایسنس
این پروژه تحت مجوز MIT منتشر شده است. استفاده، شخصی‌سازی و بازتوزیع آن کاملاً آزاد و رایگان است.

