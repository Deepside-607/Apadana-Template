<div align="center">

# 🏛️ Apadana Template
### تمپلیت اختصاصی صفحه اشتراک آپادانا

قالبی اختصاصی، پرسرعت و مدرن برای پنل‌های Rebecca، Marzban و Pasarguard

---

</div>

## 📸 پیش‌نمایش

<div align="center">

![Apadana Template Preview](./preview.jpg)

</div>

---

## ✨ ویژگی‌های برجسته

- **🏛️ طراحی اصیل ایرانی:** نشان فروهر، خطوط کتیبه‌ای میخی و افکت متالیک طلای عیار بالا
- **⚡ اسکرول روان:** پیمایش بهینه در مرورگرهای موبایل iOS و Android
- **🔧 سازگاری کامل:** شاخه `main` برای Rebecca با Pongo2 و شاخه `master` برای Marzban و Pasarguard با Jinja2
- **🌐 پشتیبانی از پروتکل‌ها:** VLESS، VMess، Trojan، Shadowsocks، OpenVPN، WireGuard، Cisco، PPTP و L2TP
- **📥 دانلود مستقیم:** امکان دانلود فایل‌های `.ovpn` و `.conf`
- **🔗 اتصال با یک کلیک:** دیپ‌لینک‌های مستقیم برای Hiddify، v2rayNG، Shadowrocket و Sing-Box

---

# 🚀 راهنمای نصب

## 🔹 ۱. پنل مرزبان (Marzban)

ابتدا قالب را با دستور زیر دانلود کنید:

```bash
sudo wget -N -P /var/lib/marzban/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)
```

سپس دستور زیر را اجرا کنید تا تمپلیت تنظیم شود:

```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
```

در نهایت پنل را ری‌استارت کنید:

```bash
marzban restart
```

---

## 🔹 ۲. پنل ربکا (Rebecca)

ابتدا قالب را با دستور زیر دانلود کنید:

```bash
sudo wget -N -P /var/lib/rebecca/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html)
```

سپس دستور زیر را اجرا کنید تا تمپلیت تنظیم شود:

```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/rebecca/templates/"' | sudo tee -a /opt/rebecca/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/rebecca/.env
```

در نهایت پنل را ری‌استارت کنید:

```bash
rebecca restart
```

---

## 🔹 ۳. پنل پاسارگاد (Pasarguard)

ابتدا قالب را با دستور زیر دانلود کنید:

```bash
sudo wget -N -P /var/lib/pasarguard/templates/subscription/ [https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html](https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html)
```

سپس دستور زیر را اجرا کنید تا تمپلیت تنظیم شود:

```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/pasarguard/templates/"' | sudo tee -a /opt/pasarguard/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/pasarguard/.env
```

در نهایت پنل را ری‌استارت کنید:

```bash
pasarguard restart
```

---

## 🌿 ساختار شاخه‌ها

| شاخه | پنل | موتور قالب |
|:---:|:---|:---|
| `main` | Rebecca | Pongo2 |
| `master` | Marzban | Jinja2 |
| `master` | Pasarguard | Jinja2 |

---

## 📜 لایسنس

این پروژه تحت مجوز [MIT](https://www.google.com/search?q=LICENSE) منتشر شده است.

استفاده، شخصی‌سازی و بازتوزیع آن آزاد و رایگان است.

---

<div align="center">

### 🏛️ Apadana Template

**طراحی اصیل ایرانی، تجربه‌ای مدرن**

Developed by [Deepside-607](https://github.com/Deepside-607)

</div>
