# 💈 Saloon & Spa Booking Platform — Multi-Tenant SaaS Architecture

[![PHP Version](https://img.shields.io/badge/PHP-8.2%2B-777bb4?style=for-the-badge&logo=php&logoColor=white)](https://php.net)
[![Laravel](https://img.shields.io/badge/Laravel-11.x-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)](https://laravel.com)
[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
[![MySQL](https://img.shields.io/badge/MySQL-8.0%2B-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://mysql.com)
[![Status](https://img.shields.io/badge/Build-Production%20Hardened-success?style=for-the-badge)](https://github.com/RG-Creators)

> **Public Architecture Showcase**: This repository provides high-level architectural documentation, system capabilities, and workflow specifications for the **Saloon & Spa Booking SaaS Platform**. Full underlying source code and proprietary mobile applications are maintained securely in a private repository.

---

## 🏗️ System Architecture & Multi-Tenant Model

The **Saloon & Spa Booking Platform** ecosystem is engineered around an isolated multi-tenant architecture designed to scale seamlessly across independent salons, spas, and multi-location grooming franchises:

```
+-----------------------------------------------------------------------------------------+
|                                LARAVEL MULTI-TENANT BACKEND                             |
|       - Global Tenant Partitioning & Multi-Branch Database Scoping                      |
|       - High-Performance RESTful API Gateway with Sanctum Authentication                |
|       - Dynamic Slot Availability & Conflict-Resolution Engine                          |
+-----------------------------------------------------------------------------------------+
                                             |
                     +-----------------------+-----------------------+
                     |                                               |
                     v                                               v
+-----------------------------------------+     +-----------------------------------------+
|           CUSTOMER MOBILE APP           |     |            SALON OWNER APP              |
|             (Flutter / Dart)            |     |            (Flutter / Dart)             |
|  - Browse Salons, Stylists & Portfolios |     |  - Live Interactive Calendar Schedule   |
|  - Real-Time Slot Reservation           |     |  - Stylist Assignment & Service Queue   |
|  - Multi-Service Add-on Selection       |     |  - Real-Time Revenue & Tip Analytics    |
|  - Digital Checkout & Status Tracking   |     |  - Staff Attendance & Commission Ledger |
+-----------------------------------------+     +-----------------------------------------+
```

---

## ⚡ Core Platform Highlights

### 1. Multi-Tenant Franchise Scoping
- **Isolated Tenant Boundaries**: Relational database foreign-key segregation preventing data leakage between salon chains.
- **Dynamic Branch Routing**: Support for salon chains operating across multiple cities with shared customer loyalty points and centralized inventory oversight.

### 2. Intelligent Slot Booking & Scheduling Engine
- Real-time slot availability calculator that prevents double-booking across stylists and specialized treatment rooms.
- Service duration buffers and variable clean-up time calculation between appointments.

### 3. Comprehensive Mobile Ecosystem
- **Customer Flutter App**: Fluid booking flow, favorite stylist bookmarking, order history, and instant appointment reminders.
- **Salon Owner Flutter App**: Drag-and-drop schedule planner, walk-in appointment quick-ticket generation, and daily settlement auditing.

---

## 🛠️ Tech Stack

- **Backend Platform**: Laravel 11.x, PHP 8.2+, Eloquent ORM, Sanctum API Tokens
- **Mobile Applications**: Flutter 3.x, Dart 3.x, Provider / Riverpod State Management
- **Database Architecture**: MySQL 8.0+ / MariaDB (Normalized Relational Schema with Composite Indexes)
- **Security & Pipeline**: Parameterized SQL, Environment Variable Isolation, Tamper-Evident SHA-256 Audit Trail

---

## 🔒 Proprietary Code Notice
The underlying application codebase, Flutter mobile client source code, and enterprise deployment configs are privately maintained. For partnership, custom deployment, or architectural inquiries, please contact:
- **Developer**: Ronit Goswami (RG Creators)
- **Email**: [rgcreatorsofficial@gmail.com](mailto:rgcreatorsofficial@gmail.com)
- **Portfolio**: [rgcreators.netlify.app](https://rgcreators.netlify.app)
