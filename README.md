# Halo, saya **Sayid Adam Kaharianto**

*Programmer • Troubleshooter Jaringan & Sistem • Installer CCTV & Cloud Server*

[![Profil](https://img.shields.io/badge/GitHub-mryunkaka-181717?logo=github&logoColor=white)](https://github.com/mryunkaka)
[![Lokasi](https://img.shields.io/badge/Lokasi-Indonesia-blue)](#)
[![Bahasa](https://img.shields.io/badge/ID-EN-bilingual-brightgreen)](#)

<!-- Tech Logos -->
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=white)
![Filament](https://img.shields.io/badge/Filament-0EA5E9?logo=react&logoColor=white)
![Winbox](https://img.shields.io/badge/Winbox-MikroTik-lightgrey)
![Fortigate](https://img.shields.io/badge/Fortigate-F7323F?logo=fortinet&logoColor=white)
![Hikvision](https://img.shields.io/badge/Hikvision-C8102E?logoColor=white)
![Ubiquiti](https://img.shields.io/badge/Ubiquiti-0559C9?logo=ubiquiti&logoColor=white)
![Synology NAS](https://img.shields.io/badge/Synology-NAS-333333?logo=synology&logoColor=white)

> Saya membangun aplikasi Laravel full-stack sekaligus terbiasa menangani masalah nyata di dunia jaringan: routing MikroTik, link wireless point-to-point, VLAN, NAT, SMB share, hingga layanan on-prem. Saya juga berpengalaman dalam instalasi CCTV dan Synology cloud server. Saya senang menyelesaikan masalah secara menyeluruh—dari logika backend sampai packet trace di jaringan.

---

## 🚀 Proyek Unggulan

### 1) Sistem Manajemen Hotel — **hotel-bome**

* **Stack:** Laravel 12, PHP 8.2+, Filament v4 (Livewire 3), MySQL
* **Fitur utama:** Multi-hotel context, alur Reservasi & Tamu (Check-in/Check-out), Folio & Billing, export PDF & Excel, single-session login, activity log, serta form kompleks berbasis repeater.
* **Repo:** [https://github.com/mryunkaka/hotel-bome](https://github.com/mryunkaka/hotel-bome)

### 2) Sistem Inventaris Aset ICT — **ict**

* **Stack:** Laravel 12, Filament v4, Spatie Permission, Activity Log, Excel, DomPDF, Intervention Image
* **Fitur:** Katalog Unit & Aset, manajemen akses berbasis role, audit trail, import/export, dokumen siap cetak.
* **Catatan:** Repo privat (hubungi saya untuk demo/walkthrough).

### 3) Catatan Lab & Lapangan Jaringan

* **Vendor:** MikroTik (RouterOS), UniFi AP, TP-Link/Tenda Pharos
* **Topik:** Desain L2/L3, link 5 GHz P2P, bridge vs. route, VLAN, NAT, QoS dasar, perencanaan kanal Wi-Fi, konektivitas SMB (445), akses NAS (Synology) LAN/WAN.
* **Konten:** Diagram, konfigurasi, dan playbook troubleshooting (versi aman/redacted).

### 4) Instalasi CCTV & Synology Cloud Server

* **CCTV:** Instalasi dan konfigurasi sistem CCTV (IP camera, DVR/NVR, remote access).
* **Synology:** Setup cloud server berbasis Synology (DSM), user & permission management, backup/restore, remote access aman.
* **Keunggulan:** Integrasi antara CCTV, NAS, dan jaringan lokal/WAN dengan monitoring yang stabil.

---

## 🛠️ Tech Stack

**Backend / Aplikasi**

* PHP 8.2–8.4, Laravel 12, Filament v4, Livewire 3
* RESTful controller, service class, policy, observer
* Migration/Seeder, Eloquent (relasi, scope), Queue/Job

**Frontend**

* Blade, Alpine.js, Tailwind CSS, shadcn/ui
* Export PDF/Excel, layout print-ready

**Data & Ops**

* MySQL/MariaDB, Redis (dasar)
* Nginx/Apache, Laragon (Windows), Git (GitHub), CI dasar

**Jaringan & Infrastruktur**

* MikroTik RouterOS (NAT, VLAN, routing, firewall), WinBox
* Link P2P: Tenda O1, TP-Link Pharos; tuning UniFi AP
* NAS: SMB share, port 445, skema user/permission
* Troubleshooting: analisa ping/latensi, lebar kanal, kualitas sinyal dBm, trade-off throughput vs. stabilitas
* CCTV: instalasi & konfigurasi IP camera, DVR/NVR, integrasi LAN/WAN
* Synology: setup DSM, shared folder, backup otomatis, cloud server

---

## 🧩 Kisah Problem-Solving

* **Single-Session Login (Filament v4)** — hanya izinkan 1 sesi aktif per user via kolom `session_id`; listener untuk set/clear saat login/logout; takeover flow aman.
* **Perhitungan Reservasi** — konsistensi logika `expected_arrival/expected_departure` dengan `checkin/checkout`; kalkulasi nights; breakdown tarif/diskon/pajak; output PDF.
* **Koneksi SMB** — diagnosa masalah “tidak bisa akses NAS” lewat link site-to-site: cek TCP 445, resolusi nama vs. IP, masalah MTU, dan setting klien Win10/11.
* **Stabilisasi Link P2P** — ubah 40 MHz → 20 MHz untuk margin SNR, atur align antena, pilih kanal DFS/non-DFS, optimasi ACK timeout.
* **Integrasi CCTV & Synology** — desain sistem monitoring yang bisa diakses aman dari luar kantor dengan integrasi backup otomatis ke NAS.

---

## 🧪 Contoh Kode

* **Form Filament v4**: schema repeater kompleks (Reservation ↔ ReservationGuest) dengan hook `mutateRelationshipData*`, dynamic grid preview, tombol aksi (Check-In, Pindah Kamar, Guest Folio, Split Bill, Payment & Check-Out).
* **Auth & Policy**: scoping per-hotel, halaman login custom, role via `spatie/permission`.
* **Export/Print**: `maatwebsite/excel` dengan styling; `barryvdh/laravel-dompdf` dengan CSS sesuai keterbatasan DOMPDF.

> Butuh snippet spesifik? Cek repo saya atau kontak langsung—bisa saya share contoh redacted.

---

## 🎓 Sertifikasi & Pelatihan (pilihan)

* Dasar-dasar jaringan & vendor-spesifik (fokus MikroTik)
* Sertifikat kompetensi bahasa Inggris
* (Lengkap ada di CV; bisa diminta jika diperlukan.)

---

## 🧰 Tools Harian

* **Editor:** VS Code (PHP Intelephense, Tailwind, Blade, GitLens, Prettier)
* **Dev Lokal:** Laragon (Windows), Composer, Node/NPM/Vite
* **Infra:** WinBox, UniFi Controller, CLI RouterOS, Synology DSM, CMS CCTV

---

## 📫 Kontak

* **GitHub:** @mryunkaka
* **Email:** [mryunkaka@gmail.com](mailto:mryunkaka@gmail.com)
* **LinkedIn:** (tambahkan link)

Jika Anda butuh bantuan membangun aplikasi Laravel, menyiapkan jaringan, instalasi CCTV, atau setup Synology cloud server—ayo ngobrol.

---
