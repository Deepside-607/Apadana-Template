علت این به‌هم‌ریختگی این است که گیت‌هاب در نسخه موبایل متن‌های فارسی را به‌صورت چپ‌به‌راست (LTR) نمایش می‌دهد؛ به همین دلیل دونقطه‌ها جابه‌جا شده، کلمات بریده می‌شوند و دستورات خط فرمان با متن فارسی تداخل پیدا می‌کنند.
برای حل قطعی این مشکل، متن‌ها داخل تگ‌های استاندارد راست‌چین (<div dir="rtl">) و دستورات در بلاک‌های اختصاصی چپ‌به‌راست قرار گرفتند تا هم راست‌چین بی‌نقص باشد و هم دکمه Copy گیت‌هاب درست کار کند:
<div align="center">

# 🏛️ Apadana Template | تمپلیت آپادانا
### قالب مدرن، اختصاصی و پرسرعت صفحه اشتراک برای پنل‌های ربکا، مرزبان و پاسارگاد

![Version](https://img.shields.io/badge/version-3.0.0-gold?style=for-the-badge)
![Engine](https://img.shields.io/badge/Engine-Pongo2%20%7C%20Jinja2-blue?style=for-the-badge)
![Panel Support](https://img.shields.io/badge/Supports-Rebecca%20%7C%20Marzban%20%7C%20Pasarguard-00f0d6?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

<p align="center">
  <b>طراحی اصیل بر پایه هویت کهن پارسی، ترکیب طلای عیار بالا، لاجوردی شب، پنل‌های شیشه‌ای (Glassmorphism) و سبک مدرن بنتوگرید (Bento Grid).</b>
</p>

</div>

---

<div dir="rtl">

## 📸 پیش‌نمایش

</div>

<div align="center">
  <img src="./preview.jpg" alt="Apadana Template Preview" width="360" style="border-radius: 20px;">
</div>

---

<div dir="rtl">

## ✨ ویژگی‌های برجسته

* 👑 **هویت اصیل هخامنشی:** نشان برداری فروهر، خطوط کتیبه‌ای میخی و افکت متالیک طلای عیار بالا.
* 📱 **پیمایش بهینه در موبایل:** رفع کامل مشکل قفل شدن تاچ و باگ اسکرول در تمام مرورگرهای گوشی.
* ⚡ **دو نسخه مجزا برای سازگاری کامل:**
  * شاخه `main`: توسعه‌یافته با موتور **Pongo2** برای پنل ربکا (Rebecca).
  * شاخه `master`: توسعه‌یافته با موتور **Jinja2** برای مرزبان (Marzban) و پاسارگاد (Pasarguard).
* 🧩 **کاوشگر اختصاصی کانفیگ‌ها:** دسته‌بندی خودکار پروتکل‌ها، جستجوی بلادرنگ، QR اختصاصی و دکمه دانلود فایل پروفایل (`.ovpn` و `.conf`).
* 🚀 **اتصال با یک کلیک:** پشتیبانی از لینک‌های مستقیم Hiddify، v2rayNG، Shadowrocket و Sing-Box.
* 🔔 **فناوری صوتی Native Web Audio:** پخش صدای دلنشین زنگ کهن هنگام کپی کردن بدون نیاز به فایل صوتی جانبی.

---

## 🛰️ پروتکل‌های پشتیبانی‌شده

| پروتکل | نحوه نمایش و عملکرد |
| :---: | :--- |
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

### ۱. مرزبان (Marzban)

**گام اول:** ابتدا قالب را با لینک زیر دانلود کنید:
</div>

```bash
sudo wget -N -P /var/lib/marzban/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)

<div dir="rtl">
گام دوم: دستورهای زیر را اجرا کنید تا تمپلیت ست شود:
</div>
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env

<div dir="rtl">
گام سوم: پنل مرزبان را ری‌استارت کنید:
</div>
marzban restart

<div dir="rtl">
۲. ربکا (Rebecca)
گام اول: ابتدا قالب را با لینک زیر دانلود کنید:
</div>
sudo wget -N -P /var/lib/rebecca/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html)

<div dir="rtl">
گام دوم: دستورهای زیر را اجرا کنید تا تمپلیت ست شود:
</div>
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/rebecca/templates/"' | sudo tee -a /opt/rebecca/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/rebecca/.env

<div dir="rtl">
گام سوم: پنل ربکا را ری‌استارت کنید:
</div>
rebecca restart

<div dir="rtl">
۳. پاسارگاد (Pasarguard)
گام اول: ابتدا قالب را با لینک زیر دانلود کنید:
</div>
sudo wget -N -P /var/lib/pasarguard/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)

<div dir="rtl">
گام دوم: دستورهای زیر را اجرا کنید تا تمپلیت ست شود:
</div>
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/pasarguard/templates/"' | sudo tee -a /opt/pasarguard/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/pasarguard/.env

<div dir="rtl">
گام سوم: پنل پاسارگاد را ری‌استارت کنید:
</div>
pasarguard restart

<div dir="rtl">
📜 لایسنس
این پروژه تحت مجوز MIT منتشر شده است. استفاده، شخصی‌سازی و بازتوزیع آن کاملاً آزاد و رایگان است.
</div>

