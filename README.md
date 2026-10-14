<div align="center">

# 🏛️ Apadana Template
### تمپلیت اختصاصی صفحه اشتراک آپادانا

قالبی مدرن، سریع و اختصاصی برای پنل‌های Rebecca، Marzban و Pasarguard

---

</div>

## 📸 پیش‌نمایش

<div align="center">

![Apadana Template Preview](./preview.jpg)

</div>

---

## ✨ ویژگی‌های برجسته

- 🏛️ **طراحی اصیل ایرانی:** الهام‌گرفته از هنر هخامنشی، نشان فروهر، خطوط کتیبه‌ای و افکت متالیک طلایی.
- ⚡ **عملکرد سریع و روان:** طراحی بهینه برای مرورگرهای موبایل و دسکتاپ.
- 📱 **سازگاری با موبایل:** تجربه کاربری مناسب در Android و iOS.
- 🔧 **پشتیبانی از چند پنل:** شاخه `main` برای Rebecca با Pongo2 و شاخه `master` برای Marzban و Pasarguard با Jinja2.
- 🌐 **پشتیبانی از پروتکل‌های مختلف:** VLESS، VMess، Trojan، Shadowsocks، OpenVPN، WireGuard، Cisco، PPTP و L2TP.
- 📥 **دانلود مستقیم کانفیگ:** امکان دانلود فایل‌های `.ovpn` و `.conf`.
- 🔗 **اتصال سریع:** پشتیبانی از لینک‌های اتصال مستقیم برای Hiddify، v2rayNG، Shadowrocket و Sing-box.

---

# 🚀 راهنمای نصب

## 🔹 ۱. پنل Marzban

### دانلود قالب

```bash
sudo mkdir -p /var/lib/marzban/templates/subscription/

sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html
```

### تنظیم قالب

```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env

echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
```

### راه‌اندازی مجدد پنل

```bash
marzban restart
```

---

## 🔹 ۲. پنل Rebecca

### دانلود قالب

```bash
sudo mkdir -p /var/lib/rebecca/templates/subscription/

sudo wget -N -P /var/lib/rebecca/templates/subscription/ https://raw.githubusercontent.com/Deepside-607/Apadana-Template/main/index.html
```

### تنظیم قالب

```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/rebecca/templates/"' | sudo tee -a /opt/rebecca/.env

echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/rebecca/.env
```

### راه‌اندازی مجدد پنل

```bash
rebecca restart
```

---

## 🔹 ۳. پنل Pasarguard

### دانلود قالب

```bash
sudo mkdir -p /var/lib/pasarguard/templates/subscription/

sudo wget -N -P /var/lib/pasarguard/templates/subscription/ https://raw.githubusercontent.com/Deepside-607/Apadana-Template/master/index.html
```

### تنظیم قالب

```bash
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/pasarguard/templates/"' | sudo tee -a /opt/pasarguard/.env

echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/pasarguard/.env
```

### راه‌اندازی مجدد پنل

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

این پروژه تحت مجوز **MIT** منتشر شده است.

استفاده، ویرایش، شخصی‌سازی و بازتوزیع پروژه مطابق شرایط مجوز MIT آزاد است.

برای اطلاعات بیشتر، فایل `LICENSE` موجود در مخزن را مطالعه کنید.

---

<div align="center">

### 🏛️ Apadana Template

**طراحی اصیل ایرانی، تجربه‌ای مدرن**

Developed by [Deepside-607](https://github.com/Deepside-607)

</div>
