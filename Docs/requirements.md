# Requirements & Dependencies

This document lists the required dependencies, versions, and tools needed to build and run **diKasir-POSApp**.

---

## 🖥️ Operating System
- **Windows 11** (recommended) or the latest version of Windows 10
- Architecture: x64

---

## 🔧 SDK & Framework
- **.NET 8 SDK** → version 8.0.x
- **Windows App SDK** → version 1.8.250907003
- **WinUI 3** → included in Windows App SDK

---

## 🛠️ IDE & Tools
- **Visual Studio 2022** (version 17.9 or newer) with workloads:
  - .NET Desktop Development
  - Desktop development with C++
- **Git** → version 2.40 or newer
- **Node.js** → version 20.x (optional, for web dashboard integration)
- **Postman / Insomnia** → for API testing (optional)

---

## 📦 NuGet Packages
- `Microsoft.WindowsAppSDK` → 1.8.250907003
- `Microsoft.Extensions.Logging` → 8.0.x
- `Microsoft.Data.Sqlite` → 8.0.x (for local database)
- `Newtonsoft.Json` → 13.0.x (JSON serialization)
- `xUnit` → 2.6.x (unit testing)

---

## 🗄️ Database
- **SQLite** → version 3.45 or newer (default)
- **SQL Server 2022** (optional, for enterprise deployment)

---

## 🔌 Hardware Integration
- POS Printer (ESC/POS compatible)
- Barcode Scanner (USB/HID)
- Cash Drawer (via printer kick port)

---

## 📈 Dependency Roadmap
- [ ] Add packages for digital payment integration (QRIS/e-wallet)
- [ ] Add libraries for multi-tenant support
- [ ] Add monitoring & logging stack (Serilog, Loguru, or similar)
