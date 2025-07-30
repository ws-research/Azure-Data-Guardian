# Azure Data Guardian  
**Enterprise Azure Data Management Suite (Phase 1)**  

[![Java 17](https://img.shields.io/badge/Java-17+-orange?logo=openjdk)](https://java.com)
[![Graph API](https://img.shields.io/badge/Microsoft_Graph_API-v1.0-blue?logo=microsoftazure)](https://learn.microsoft.com/graph)
[![Release Phase](https://img.shields.io/badge/Release-Phase_1-yellow)](https://github.com/ws-research/azure-data-guardian/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Roadmap](https://img.shields.io/badge/Roadmap-Public-brightgreen)](ROADMAP.md)

> **Phase 1**: Secure email management solution for Azure administrators. A comprehensive data management suite evolving through planned releases.

---

## 🚀 Phase 1: Core Foundation (Available Now)

### 🔐 Secure Authentication
- Desktop UI for Azure credential input (Tenant ID, Client ID, Client Secret)
- Microsoft Graph API integration with OAuth 2.0
- Permission validation and error handling

### ✉️ Email Data Management
- Full mailbox processing via Microsoft Graph API
- User selection interface for targeted exports
- Raw EML format export with metadata preservation

### 🖥️ Standalone Desktop Application
- Java JAR executable (Java 17+ required)
- Intuitive desktop UI (SwingX)

**Phase 1 UI Preview**:  
![Phase 1 UI](screenshots/phase1-ui.png)  
*Current interface showing authentication and email export workflow*

---


## 🔮 Future Release Roadmap

### Phase 2: Search & Expand (Q3 2025)
- **OneDrive Integration**: Business file management and export
- **SharePoint Access**: Document library retrieval
- **File Type Filtering**: Selective exports (e.g., ".docx only")

### Phase 3: Advanced Operations (Q4 2025)
- **Multi-Format Exports**: CSV, JSON, XML metadata reports
- **ZIP Compression**: Archive creation options
- **Export Statistics**: Performance metrics dashboard

### Phase 4: Enterprise Readiness (Q1 2026)
- **Office Previews**: Native Word/Excel/PPT viewing
- **Transfer Reliability**: Pause/resume functionality
- **Progress Tracking**: Real-time export monitoring
- **Bulk Operations**: Multi-user/data source processing

### Phase 5: Optimization & Scale (Q1 2026)
- **Distributed Processing**: High-volume handling
- **Azure Blob Integration**: Cloud storage options
- **Scheduled Backups**: Automated export workflows

```mermaid
gantt
    title Development Timeline
    dateFormat  YYYY-MM-DD
    section Phase 1 (Now)
    Authentication      :done, auth, 2025-07-01, 10d
    Email Export        :done, email, after auth, 20d
    
    section Phase 2 (Q3 2025)
    OneDrive            :active, 2025-08-01, 30d
    SharePoint          : 2025-09-01, 20d
    File Type Filtering : 2025-09-20, 10d
    
    section Phase 3 (Q4 2025)
    Export Formats      : 2025-10-01, 15d
    Export Statistics   : 2025-10-15, 30d
    
    section Phase 4 (Q4 2025)
    Office Previews     : 2025-11-15, 30d
    Transfer Management : 2025-12-15, 15d
    
    section Phase 5 (Q1 2026)
    Scalability Engine  : 2026-01-01, 20d
    Admin Suite         : 2026-01-20, 10d
```

---

## ⚡ Getting Started with Phase 1

### Prerequisites
- Java 17+ Runtime ([Download](https://java.com))
- Azure AD App Registration with:
  - `Mail.Read` permission
  - Admin consent granted
- Valid admin credentials (Tenant ID, Client ID, Client Secret)


### First-Time Workflow
1. Enter Azure credentials in authentication screen
2. Navigate to "Email Management" tab
3. Select target user mailbox
4. Initiate export (saves as EML files to local directory)

---

## 💼 Phase 1 Use Case: Email Archive Migration

**Scenario**: Export emails from departed employee `j.smith@company.com` for legal retention

**Workflow**:
1. Launch application and authenticate
2. Select "Email Export" module
3. Enter target email address
4. Export full mailbox as EML files
5. Preserve original folder structure

**Key Benefits**:
- No PowerShell expertise required
- Native format preservation for compliance
- Desktop-based secure processing

---

## 🛠️ Technical Specifications (Phase 1)

### Architecture
```mermaid
graph LR
A[SwingX] --> B[Auth Module]
B --> C[Graph API Client]
C --> D[File System]
D --> E[Export Validation]
```

### Supported Environments
- Windows 10/11 (64-bit)
- macOS 12+ (Intel/Apple Silicon)
- Linux (Ubuntu 20.04+, Fedora 36+)

---

## 📬 What's Next in Phase 2?
- OneDrive business data management
- SharePoint document access
- File type filtering capabilities

**Contribute to our roadmap**:  
[![Feature Voting](https://img.shields.io/badge/Vote-Next_Features-blue)](https://github.com/ws-research/azure-data-guardian/discussions/1)

---

## 🧪 Testing & Feedback
We invite administrators to:
1. Validate authentication workflows
2. Test email export integrity
3. Suggest UI improvements

[![Report Issues](https://img.shields.io/badge/REPORT_ISSUES-Here-red)](https://github.com/ws-research/azure-data-guardian/issues)
[![Join Discussion](https://img.shields.io/badge/COMMUNITY-Discussions-green)](https://github.com/ws-research/azure-data-guardian/discussions)

---

## 🤝 Contribution Guidelines
1. Fork the repository
2. Create feature branch (`git checkout -b feature/your-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/your-feature`)
5. Open pull request

**Priority Contribution Areas**:
- Graph API error handling
- Export performance optimization
- UI test automation
- Localization framework

---

## 📜 License  
MIT License 

**Security Reports**: [kien61365@gmail.com](mailto:kien61365@gmail.com)  

---

**Join Our Evolution**:  
⭐ **Star this repo to stay updated on new releases** ⭐  

---

> "The journey of a thousand backups begins with a single export." - Phase 1 Motto
