# 🛒 **Mini Market POS System**

A full-featured **Point of Sale** system for mini markets and retail shops — built with **PHP**, **MySQL**, **HTML**, **CSS**, and **JavaScript**.  
Manage products, members, inventory, sales, thermal receipts, and cash drawer from one clean dashboard.

✨ Feel free to explore, contribute, and enhance the project! 🚀

<p align="center">
  <img src="https://img.shields.io/badge/PHP-8%2B-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
  <img src="https://img.shields.io/badge/MySQL-8-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Bootstrap-5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap" />
  <img src="https://img.shields.io/badge/XAMPP-Ready-FB7A24?style=for-the-badge&logo=xampp&logoColor=white" alt="XAMPP" />
  <img src="https://img.shields.io/badge/License-MIT%20NC-2ea44f?style=for-the-badge" alt="License" />
</p>

---

## ✨ **Features**

- 🔐 **Admin & Staff Login** — split login portal, role-based access, session + CSRF protection
- 📊 **Live Dashboard** — today / month sales, low-stock alerts, recent activity
- 📦 **Inventory** — products, categories, suppliers, purchases, stock adjustments
- 🛒 **POS Cashier** — barcode scan, cart, SST tax, cash / TNG checkout
- 👤 **Members & Loyalty** — add members from POS, welcome points, redeem at checkout
- 🧾 **Thermal Receipts** — 80mm ticket, local print agent, auto-cut, cash drawer kick
- 🔔 **Notifications** — unread badge on the bell; opening the page marks all as read
- 📑 **Reports** — sales / inventory / members with print & Excel export
- 🌍 **i18n** — English, 中文, Bahasa Malaysia

---

## 🏗️ **Tech Stack**

| **Category** | **Technology** |
| --- | --- |
| 🖥️ **Frontend** | HTML5, CSS3, JavaScript, Bootstrap 5, Bootstrap Icons |
| 🔙 **Backend** | Native PHP 8+ (no framework) |
| 🗄️ **Database** | MySQL / MariaDB (`ekoperasi_db`) |
| 🔐 **Security** | PDO prepared statements, CSRF tokens, `password_hash` |
| 🖨️ **Printing** | Local USB print agent (Xprinter XP-80) |
| 🌐 **Server** | Apache (XAMPP / cPanel) |

---

## 🖼️ **Project Screenshots**

<table>
  <tr>
    <td colspan="2" align="center">
      <img src="docs/screenshots/01-login.png" alt="Login portal" width="100%" />
      <br/>
      <sub>🔐 <b>Login Portal</b> — Admin / Staff glassmorphism sign-in</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="docs/screenshots/02-dashboard.png" alt="Dashboard" width="100%" />
      <br/>
      <sub>📊 <b>Dashboard</b> — live sales cards & charts</sub>
    </td>
    <td align="center" width="50%">
      <img src="docs/screenshots/03-pos.png" alt="POS cashier" width="100%" />
      <br/>
      <sub>🛒 <b>POS Cashier</b> — products, cart & checkout</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="docs/screenshots/04-members.png" alt="Members" width="100%" />
      <br/>
      <sub>👤 <b>Members</b> — register & loyalty points</sub>
    </td>
    <td align="center" width="50%">
      <img src="docs/screenshots/05-receipt.png" alt="Receipt" width="100%" />
      <br/>
      <sub>🧾 <b>Receipt</b> — 80mm ticket + print / drawer</sub>
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="docs/screenshots/06-reports.png" alt="Reports" width="100%" />
      <br/>
      <sub>📑 <b>Reports</b> — filters, print & Excel export</sub>
    </td>
  </tr>
</table>

---

## 📋 **Requirements**

- 💻 **XAMPP** (Apache + MySQL + PHP 8.0+) **or** PHP hosting (cPanel)
- 🌐 Modern browser (Chrome / Edge / Firefox)
- 🖨️ Optional: USB thermal printer + `print-agent` for auto-cut / cash drawer

---

## 🚀 **Installation**

1. 📁 Place the project in your web root:
   ```text
   C:\xampp\htdocs\Pos_System
   ```
2. ▶️ Start **Apache** and **MySQL** in the XAMPP Control Panel.
3. 🗄️ Restore the database (pick one):
   - Double-click `import-database.bat`
   - Open [http://localhost/Pos_System/install-db.php](http://localhost/Pos_System/install-db.php)
   - Or run: `php cli-install-db.php`
4. 🌐 Open the app:
   ```text
   http://localhost/Pos_System/
   ```

### 🔑 **Default credentials**

| Role | Username | Password |
| --- | --- | --- |
| 👨‍💼 Admin | `admin` | `admin123` |
| 🧾 Staff | `user` | `user123` |

> ⚠️ Change the default passwords after first login.

### ☁️ **cPanel / production**

1. Copy `config/database.local.example.php` → `config/database.local.php`
2. Fill in your hosting MySQL name / user / password
3. Upload the project and run `install-db.php` once (then remove it)

---

## 📁 **Folder Structure**

```text
Pos_System/
├── admin/                 # Dashboard, POS, products, members, reports
├── auth/                  # Login portal, admin/staff login, logout
├── api/                   # Barcode lookup, add-member
├── config/                # database.php + local overrides
├── database/              # schema.sql
├── docs/screenshots/      # README project screenshots
├── includes/              # init, navbar, sidebar, migrations
├── assets/                # CSS, JS, vendor (Bootstrap)
├── print-agent/           # Local USB printer + cash drawer
├── uploads/               # Product images
├── install-db.php         # Browser database installer
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

---

## 🤝 **Contributing**

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

💡 To contribute, check the guidelines and open a PR with a clear description of what you changed.

---

## 📝 **License**

This project is licensed under the [MIT Non-Commercial License](LICENSE).

---

## ©️ **Copyright**

**Copyright © 2026 Eng Choon Hao. All Rights Reserved.**

Unauthorized copying or redistribution of this project without permission is prohibited.

---

⭐ If you find this project helpful, don't forget to **star** the repository! 🌟

Happy coding! 💻🎉
