# Setup & Installation Guide for diKasir-POSApp

This document provides detailed steps to install, configure, and run **diKasir-POSApp**, a modern Point of Sale (POS) application built with WinUI 3.

---

## 🖥️ Prerequisites

Before starting, ensure the following are installed:

- **Operating System**
  - Windows 11 (recommended) or Windows 10 (latest updates)
  - Architecture: x64

- **SDK & Frameworks**
  - [.NET 8 SDK](https://dotnet.microsoft.com/download) (version 8.0.x)
  - [Windows App SDK](https://learn.microsoft.com/windows/apps/windows-app-sdk/) (version 1.8.250907003)
  - WinUI 3 (included in Windows App SDK)

- **IDE & Tools**
  - Visual Studio 2022 (version 17.9 or newer) with workloads:
    - .NET Desktop Development
    - Desktop development with C++
  - Git (version 2.40 or newer)
  - Node.js (version 20.x, optional for web dashboard integration)
  - Postman or Insomnia (optional, for API testing)

---

## 📂 Repository Structure

diKasir-POSApp/ ├── POSApp/ # Main WinUI 3 project ├── Docs/ # Technical documentation └── README.md             # Project description

---

## 🚀 Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/<username>/diKasir-POSApp.git
   cd diKasir-POSApp
2. Navigate to the project folder
    cd POSApp
3. Restore dependencies
    dotnet restore
4. Build the project
    dotnet build
5. Run the application
    dotnet run

## ⚙️ Initial Configuration

1. Database
    -Default: SQLite (local development)
    -Optional: SQL Server 2022 for enterprise deployment
2. Role-Based UI
    -Default user role: Admin
    -Roles can be configured in appsettings.json
3. Hardware Integration
    -POS printer, barcode scanner, and cash drawer support
    -Configuration available in Infrastructure/HardwareConfig.cs

## 🧪 Testing

Run unit and integration tests:
    -- dotnet test

## 📈 Setup Roadmap

    -[ ] Add SQL Server configuration guide
    -[ ] Integrate API Gateway for web dashboard
    -[ ] Setup CI/CD pipeline (GitHub Actions / GitLab CI)
    -[ ] Add digital payment integration (QRIS, e-wallet)
    
---