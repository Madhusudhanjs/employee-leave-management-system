# Employee Leave Management System

A web-based Employee Leave Management System built using **PHP, MySQL, and Bootstrap**.  
This system allows employees to apply for leave and admins to manage leave records efficiently.

---

## 🔧 Tech Stack

- PHP (Core PHP)
- MySQL (phpMyAdmin)
- Apache Server (XAMPP)
- HTML, CSS, JavaScript
- Bootstrap

---

## 📂 Project Structure

```
employee-leave-management-system/
│
├── elms/              # Main project folder
├── Sql file/          # Database SQL file
├── README.md
```

---

## 🚀 How To Run This Project

### Step 1: Install XAMPP
Download and install from:
https://www.apachefriends.org/index.html

Start:
✅ Apache  
✅ MySQL  

---

### Step 2: Clone this repository

Open terminal and run:

```
cd C:\xampp\htdocs
git clone https://github.com/Madhusudhanjs/employee-leave-management-system.git
```

---

### Step 3: Setup Database

1. Open browser  
   ```
   http://localhost/phpmyadmin
   ```
2. Create a database named:
   ```
   elms
   ```
3. Click **Import**  
4. Select this file from your project:
   ```
   Sql file/elms.sql
   ```

---

### Step 4: Configure Database Connection

Open this file in your project:

```
elms/includes/config.php
```

Make sure it has:

```php
define('DB_HOST', 'localhost');
define('DB_USER', 'root');
define('DB_PASS', '');
define('DB_NAME', 'elms');
```

---

### Step 5: Run the project

Open in browser:

Employee:
```
http://localhost/employee-leave-management-system/elms/
```

Admin:
```
http://localhost/employee-leave-management-system/elms/admin/
```

---

## 🔐 Default Admin Login

If login fails, reset password using phpMyAdmin SQL tab:

```sql
UPDATE admin SET Password = MD5('admin') WHERE id = 1;
```

Then login with:

```
Username: admin
Password: admin
```

---

## 👨‍💻 Developed By

**Madhusudhan J S**  
GitHub: https://github.com/Madhusudhanjs
