# 🏛️ Apadana Template | تمپلیت آپادانا

قالب اختصاصی، پرسرعت و مدرن صفحه اشتراک برای پنل‌های ربکا، مرزبان و پاسارگاد

---

## 📸 پیش‌نمایش

![Apadana Template Preview](./preview.jpg)

---

## ✨ ویژگی‌های برجسته

- **طراحی اصیل:** نشان برداری فروهر، خطوط کتیبه‌ای میخی و افکت متالیک طلای عیار بالا
- **بدون باگ اسکرول:** پیمایش کاملاً روان در مرورگرهای موبایل (iOS و Android)
- **سازگاری کامل:** شاخه main برای ربکا (Pongo2) و شاخه master برای مرزبان و پاسارگاد (Jinja2)
- **پشتیبانی کامل پروتکل‌ها:** VLESS, VMess, Trojan, Shadowsocks, OpenVPN, WireGuard, Cisco, PPTP/L2TP
- **دانلود مستقیم:** دکمه مستقیم دانلود فایل‌های ovpn. و conf.
- **اتصال با یک کلیک:** دیپ‌لینک‌های مستقیم برای Hiddify، v2rayNG، Shadowrocket و Sing-Box

---

## 🚀 راهنمای نصب

---

### 🔹 ۱. پنل مرزبان (Marzban)

ابتدا قالب را با لینک زیر دانلود کنید:

```bash
sudo wget -N -P /var/lib/marzban/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)

سپس دستور زیر را بزنید تا تمپلیت ست شود:
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env

سپس با دستور زیر پنل خودتون رو ری‌استارت کنید:
marzban restart

🔹 ۲. پنل ربکا (Rebecca)
ابتدا قالب را با لینک زیر دانلود کنید:
sudo wget -N -P /var/lib/rebecca/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html)

سپس دستور زیر را بزنید تا تمپلیت ست شود:
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/rebecca/templates/"' | sudo tee -a /opt/rebecca/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/rebecca/.env

سپس با دستور زیر پنل خودتون رو ری‌استارت کنید:
rebecca restart

🔹 ۳. پنل پاسارگاد (Pasarguard)
ابتدا قالب را با لینک زیر دانلود کنید:
sudo wget -N -P /var/lib/pasarguard/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)

سپس دستور زیر را بزنید تا تمپلیت ست شود:
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/pasarguard/templates/"' | sudo tee -a /opt/pasarguard/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/pasarguard/.env

سپس با دستور زیر پنل خودتون رو ری‌استارت کنید:
pasarguard restart

📜 لایسنس
این پروژه تحت مجوز MIT منتشر شده است. استفاده، شخصی‌سازی و بازتوزیع آن کاملاً آزاد و رایگان است.

