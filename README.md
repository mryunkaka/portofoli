# Hi, I’m **Sayid Adam Kaharianto**

*Programmer • Network & Systems Troubleshooter*

[![Profile](https://img.shields.io/badge/GitHub-mryunkaka-181717?logo=github\&logoColor=white)](https://github.com/mryunkaka)
[![Location](https://img.shields.io/badge/Location-Indonesia-blue)](#)
[![Language](https://img.shields.io/badge/ID-EN-bilingual-brightgreen)](#)

> I build full‑stack Laravel apps and also get my hands dirty with real‑world networking: MikroTik routing, point‑to‑point wireless links, VLANs, NAT, SMB shares, and on‑prem services. I love solving messy problems end‑to‑end—from backend logic to packet traces.

---

## 🚀 Spotlight Projects

### 1) Hotel Management System — **hotel‑bome**

* **Stack:** Laravel 12, PHP 8.2+, Filament v4 (Livewire 3), MySQL
* **Key features:** Multi‑hotel context, Reservation & Guest flows (Check‑in/Check‑out), Folio/Billing, PDF & Excel exports, single‑session auth, activity logging, and advanced repeater‑based forms.
* **Repo:** [https://github.com/mryunkaka/hotel-bome](https://github.com/mryunkaka/hotel-bome)

### 2) ICT Asset Tracking — **ict**

* **Stack:** Laravel 12, Filament v4, Spatie Permission, Activity Log, Excel, DomPDF, Intervention Image
* **Highlights:** Units & Assets catalog, role‑based access, audit trails, import/export, printable documents.
* **Note:** Private repo (ask me for a walkthrough/demo).

### 3) Networking Lab & Field Notes

* **Vendors:** MikroTik (RouterOS), UniFi AP, TP‑Link/Tenda Pharos
* **Topics:** L2/L3 design, P2P 5 GHz links, bridge vs. route, VLAN, NAT, QoS basics, Wi‑Fi channel planning, SMB (445) connectivity, NAS (Synology) access over LAN/WAN.
* **Artifacts:** Diagrams, configs, and troubleshooting playbooks (sanitized examples).

---

## 🛠️ Tech Stack

**Backend / App**

* PHP 8.2–8.4, Laravel 12, Filament v4, Livewire 3
* RESTful controllers, service classes, policies, observers
* Migrations/Seeders, Eloquent (relations, scopes), Queues/Jobs

**Frontend**

* Blade, Alpine.js, Tailwind CSS, shadcn/ui styling patterns
* PDF/Excel generation, print‑ready layouts

**Data & Ops**

* MySQL/MariaDB, Redis (basic)
* Nginx/Apache, Laragon (Windows), Git (GitHub), CI basics

**Networking**

* MikroTik RouterOS (NAT, VLAN, routing, firewall), WinBox
* P2P links: Tenda O1, TP‑Link Pharos; UniFi AP tuning
* NAS: SMB shares, port 445, user/permission schemes
* Troubleshooting: ping/latency analysis, channel width, dBm signal quality, throughput vs. stability trade‑offs

---

## 🧩 Featured Problem‑Solving Stories

* **Single‑Session Login (Filament v4)** — enforce one active session per user via `session_id` column; listeners to set/clear on login/logout; safe takeover flow.
* **Reservation math** — consistent `expected_arrival/expected_departure` vs. `checkin/checkout` logic; nights calculation; rate/discount/tax breakdown with PDF output.
* **SMB Connectivity** — diagnose “can’t reach NAS” over site‑to‑site links: confirm TCP 445, name resolution vs. IP, MTU quirks, and Win10/11 client settings.
* **P2P Link Stabilization** — move from 40 MHz to 20 MHz for SNR margin, align antennas, select DFS/non‑DFS channels, and optimize ACK timeout.

---

## 🧪 Code Samples

* **Filament v4 Forms**: complex repeater schemas (Reservation ↔ ReservationGuest) with `mutateRelationshipData*` hooks, dynamic grid previews, action buttons (Check‑In, Move Room, Guest Folio, Split Bill, Payment & Check‑Out).
* **Auth & Policy**: per‑hotel scoping, custom login page, `spatie/permission` roles.
* **Exports/Print**: `maatwebsite/excel` styled sheets; `barryvdh/laravel-dompdf` with careful CSS for DOMPDF quirks.

> Need a specific snippet? Check the repos or ping me—happy to share redacted examples.

---

## 🎓 Certifications & Training (selected)

* Networking basics & vendor‑specific (MikroTik‑oriented)
* English competency certificates
* (More listed in my CV; available upon request.)

---

## 🧰 Tools I Use Daily

* **Editor:** VS Code (PHP Intelephense, Tailwind, Blade, GitLens, Prettier)
* **Local Dev:** Laragon (Windows), Composer, Node/NPM/Vite
* **Infra:** WinBox, UniFi Controller, RouterOS CLI

---

## 📫 Contact

* **GitHub:** @mryunkaka
* **Email:** [sayidadamkaharianto@gmail.com](mailto:sayidadamkaharianto@gmail.com)
* **LinkedIn:** (add link)

If you’d like help with a Laravel app that must work reliably on a real‑world network—or you want someone who can tune the network *and* the app—let’s talk.

---

### 📝 How to use this as your GitHub profile

Create a repo named exactly **`mryunkaka`** (same as your username) and put this file as `README.md`. GitHub will display it on your profile.

```bash
# 1) Create the special profile repo (one time)
mkdir mryunkaka && cd mryunkaka
git init

# 2) Add this README
echo "(paste this whole markdown here)" > README.md

# 3) Push to GitHub
git add README.md
git commit -m "feat: add profile README"
git branch -M main
git remote add origin https://github.com/mryunkaka/mryunkaka.git
git push -u origin main
```

> Tip: add screenshots, diagrams (PNG/SVG), and links to key issues/PRs. Keep a short “Now” section for what you’re currently building.
