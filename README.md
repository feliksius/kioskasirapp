# 🛒 KioskAsir - Smart POS System with AI Analytics

<div align="center">

![KioskAsir Logo](https://kioskasir.com/Logo_KK.png)

**Modern Point of Sale System with AI-Powered Business Intelligence**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PHP](https://img.shields.io/badge/PHP-8.0+-777BB4.svg)](https://php.net)
[![MySQL](https://img.shields.io/badge/MySQL-5.7+-4479A1.svg)](https://mysql.com)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3+-7952B3.svg)](https://getbootstrap.com)

[English](#english) | [Bahasa Indonesia](#bahasa-indonesia)

</div>

---

## English

### 🚀 Overview

KioskAsir is a comprehensive Point of Sale (POS) system designed for F&B businesses, retail stores, and small to medium enterprises. It combines traditional POS functionality with advanced AI-powered analytics to provide actionable business insights.

### ✨ Key Features

#### 📊 **Core POS Functions**
- **Sales Management** - Complete transaction processing with receipt printing
- **Inventory Control** - Real-time stock tracking and management
- **Customer Management** - Customer database with purchase history
- **Supplier Management** - Vendor information and purchase tracking
- **Multi-User Support** - Role-based access control (Admin, Cashier, Supervisor)
- **Shift Management** - Daily shift reporting and cash reconciliation

#### 🤖 **AI-Powered Analytics**
- **Sales Prediction** - 7-day revenue forecasting using linear regression
- **Peak Hours Analysis** - Traffic pattern analysis for optimal staffing
- **Smart Inventory** - Auto-reorder recommendations and dead stock detection
- **Profitability Analysis** - Margin analysis and pricing optimization
- **Business Intelligence** - AI-generated actionable recommendations

#### 🔐 **Security & Management**
- **Role-Based Permissions** - Granular access control system
- **License Management** - Feature licensing and activation system
- **Audit Trail** - Complete transaction void and modification tracking
- **Data Security** - XSS and SQL injection protection

### 🏗️ Architecture

```
kioskasir/
├── 📁 config/          # Configuration files and documentation
├── 📁 includes/        # Core functions and templates
├── 📁 models/          # Data models (if using MVC)
├── 📁 controllers/     # Business logic controllers
├── 📁 views/           # UI templates and components
├── 📁 assets/          # CSS, JS, and images
├── 📁 ajax/            # AJAX endpoints for dynamic features
├── 📁 uploads/         # User uploaded files
└── 📄 *.php            # Main application pages
```

### 🛠️ Technology Stack

- **Backend**: PHP 8.0+
- **Database**: MySQL 5.7+
- **Frontend**: Bootstrap 5.3, JavaScript ES6
- **Charts**: Chart.js for analytics visualization
- **Icons**: Bootstrap Icons
- **Security**: Built-in XSS and SQL injection protection

### ⚡ Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/kioskasir.git
   cd kioskasir
   ```

2. **Setup database**
   - Create MySQL database
   - Import database schema
   - Configure `config/database.php`

3. **Install dependencies**
   ```bash
   composer install
   ```

4. **Start development server**
   ```bash
   npm run dev
   # or
   php -S localhost:8000 -c php.ini
   ```

5. **Access the application**
   - Open `http://localhost:8000`
   - Default login: admin/admin

### 📈 AI Analytics Features

#### Sales Prediction Algorithm
```php
// Linear regression for 7-day forecast
$slope = ($n * $sumXY - $sumX * $sumY) / ($n * $sumX2 - $sumX * $sumX);
$intercept = ($sumY - $slope * $sumX) / $n;

// Generate predictions
for ($i = 1; $i <= 7; $i++) {
    $predictions[] = $intercept + $slope * ($n + $i);
}
```

#### Smart Inventory Management
- **Stock Prediction**: Days until empty calculation
- **Auto Reorder**: Dynamic reorder point recommendations
- **Dead Stock Detection**: Products not sold in 30+ days
- **Priority Alerts**: Urgent, High, Medium, Low priority system

### 🎯 Use Cases

- **Restaurant & Café** - Order management with kitchen integration
- **Retail Store** - Product sales with inventory tracking
- **Pharmacy** - Medicine sales with expiry tracking
- **Convenience Store** - Quick checkout with loyalty programs
- **Small Business** - Complete business management solution

### 📱 Mobile Friendly

Responsive design optimized for:
- Tablet POS terminals
- Mobile device management
- Touch-friendly interface
- Offline capability (planned)

### 🔒 Security Features

- **Input Validation** - All user inputs sanitized
- **SQL Injection Protection** - Prepared statements
- **XSS Prevention** - Output escaping
- **Role-Based Access** - Granular permissions
- **Session Management** - Secure session handling

### 📊 Reports & Analytics

- Daily, weekly, monthly sales reports
- Inventory turnover analysis
- Customer purchase patterns
- Supplier performance metrics
- Profit margin analysis
- Cash flow tracking

### 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

### 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Bahasa Indonesia

### 🚀 Gambaran Umum

KioskAsir adalah sistem Point of Sale (POS) komprehensif yang dirancang untuk bisnis F&B, toko retail, dan usaha kecil menengah. Menggabungkan fungsi POS tradisional dengan analitik AI canggih untuk memberikan wawasan bisnis yang actionable.

### ✨ Fitur Utama

#### 📊 **Fungsi POS Inti**
- **Manajemen Penjualan** - Pemrosesan transaksi lengkap dengan cetak struk
- **Kontrol Inventori** - Pelacakan dan manajemen stok real-time
- **Manajemen Pelanggan** - Database pelanggan dengan riwayat pembelian
- **Manajemen Supplier** - Informasi vendor dan pelacakan pembelian
- **Dukungan Multi-User** - Kontrol akses berbasis peran (Admin, Kasir, Supervisor)
- **Manajemen Shift** - Laporan shift harian dan rekonsiliasi kas

#### 🤖 **Analitik Bertenaga AI**
- **Prediksi Penjualan** - Peramalan pendapatan 7 hari menggunakan regresi linear
- **Analisis Jam Sibuk** - Analisis pola lalu lintas untuk staffing optimal
- **Inventori Cerdas** - Rekomendasi auto-reorder dan deteksi dead stock
- **Analisis Profitabilitas** - Analisis margin dan optimasi harga
- **Business Intelligence** - Rekomendasi actionable yang dihasilkan AI

#### 🔐 **Keamanan & Manajemen**
- **Izin Berbasis Peran** - Sistem kontrol akses granular
- **Manajemen Lisensi** - Sistem lisensi dan aktivasi fitur
- **Audit Trail** - Pelacakan void dan modifikasi transaksi lengkap
- **Keamanan Data** - Perlindungan XSS dan SQL injection

### 🏗️ Arsitektur

```
kioskasir/
├── 📁 config/          # File konfigurasi dan dokumentasi
├── 📁 includes/        # Fungsi inti dan template
├── 📁 models/          # Model data (jika menggunakan MVC)
├── 📁 controllers/     # Controller logika bisnis
├── 📁 views/           # Template UI dan komponen
├── 📁 assets/          # CSS, JS, dan gambar
├── 📁 ajax/            # Endpoint AJAX untuk fitur dinamis
├── 📁 uploads/         # File yang diupload user
└── 📄 *.php            # Halaman aplikasi utama
```

### 🛠️ Stack Teknologi

- **Backend**: PHP 8.0+
- **Database**: MySQL 5.7+
- **Frontend**: Bootstrap 5.3, JavaScript ES6
- **Charts**: Chart.js untuk visualisasi analitik
- **Icons**: Bootstrap Icons
- **Keamanan**: Perlindungan XSS dan SQL injection built-in

### ⚡ Mulai Cepat

1. **Clone repository**
   ```bash
   git clone https://github.com/your-username/kioskasir.git
   cd kioskasir
   ```

2. **Setup database**
   - Buat database MySQL
   - Import schema database
   - Konfigurasi `config/database.php`

3. **Install dependencies**
   ```bash
   composer install
   ```

4. **Jalankan development server**
   ```bash
   npm run dev
   # atau
   php -S localhost:8000 -c php.ini
   ```

5. **Akses aplikasi**
   - Buka `http://localhost:8000`
   - Login default: admin/admin

### 📈 Fitur AI Analytics

#### Algoritma Prediksi Penjualan
```php
// Regresi linear untuk forecast 7 hari
$slope = ($n * $sumXY - $sumX * $sumY) / ($n * $sumX2 - $sumX * $sumX);
$intercept = ($sumY - $slope * $sumX) / $n;

// Generate prediksi
for ($i = 1; $i <= 7; $i++) {
    $predictions[] = $intercept + $slope * ($n + $i);
}
```

#### Manajemen Inventori Cerdas
- **Prediksi Stok**: Kalkulasi hari sampai habis
- **Auto Reorder**: Rekomendasi titik reorder dinamis
- **Deteksi Dead Stock**: Produk tidak terjual 30+ hari
- **Alert Prioritas**: Sistem prioritas Urgent, Tinggi, Sedang, Rendah

### 🎯 Kasus Penggunaan

- **Restoran & Kafe** - Manajemen pesanan dengan integrasi dapur
- **Toko Retail** - Penjualan produk dengan pelacakan inventori
- **Apotek** - Penjualan obat dengan pelacakan kadaluarsa
- **Minimarket** - Checkout cepat dengan program loyalitas
- **Usaha Kecil** - Solusi manajemen bisnis lengkap

### 📱 Mobile Friendly

Desain responsif yang dioptimalkan untuk:
- Terminal POS tablet
- Manajemen perangkat mobile
- Interface ramah sentuh
- Kapabilitas offline (direncanakan)

### 🔒 Fitur Keamanan

- **Validasi Input** - Semua input user disanitasi
- **Perlindungan SQL Injection** - Prepared statements
- **Pencegahan XSS** - Output escaping
- **Akses Berbasis Peran** - Izin granular
- **Manajemen Sesi** - Penanganan sesi aman

### 📊 Laporan & Analitik

- Laporan penjualan harian, mingguan, bulanan
- Analisis turnover inventori
- Pola pembelian pelanggan
- Metrik performa supplier
- Analisis margin profit
- Pelacakan cash flow

### 🤝 Kontribusi

1. Fork repository
2. Buat feature branch (`git checkout -b feature/fitur-keren`)
3. Commit perubahan (`git commit -m 'Tambah fitur keren'`)
4. Push ke branch (`git push origin feature/fitur-keren`)
5. Buka Pull Request

### 📄 Lisensi

Proyek ini dilisensikan di bawah MIT License - lihat file [LICENSE](LICENSE) untuk detail.

---

<div align="center">

**🚀 Transform your business with AI-powered POS analytics!**

**🚀 Transformasi bisnis Anda dengan analitik POS bertenaga AI!**

Made with ❤️ for the business community

</div>
