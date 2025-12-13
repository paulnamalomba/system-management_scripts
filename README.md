# System Management Scripts

**Last updated**: December 13, 2025<br>
**Author**: [Paul Namalomba](https://github.com/paulnamalomba)<br>
  - SESKA Computational Engineer<br>
  - Software Developer<br>
  - PhD Candidate (Civil Engineering Spec. Computational and Applied Mechanics)<br>

**Contact**: [kabwenzenamalomba@gmail.com](kabwenzenamalomba@gmail.com)<br>
**Website**: [paulnamalomba.github.io](https://paulnamalomba.github.io)<br>

<!-- [![PowerShell](https://img.shields.io/badge/PowerShell-7%2B-blue.svg)](https://github.com/PowerShell/PowerShell) -->
[![License: MIT](https://img.shields.io/badge/License-MIT-gray.svg)](https://opensource.org/licenses/MIT)

## Overview

A collection of system management scripts, automation utilities, and technical power user guides for developers, system administrators, and engineers. This repository provides mostly in-depth guides covering databases, containers, messaging systems, security, and enterprise authentication.

## Contents

- [System Management Scripts](#system-management-scripts)
  - [Overview](#overview)
  - [Contents](#contents)
  - [Purpose](#purpose)
  - [Repository Structure](#repository-structure)
  - [Power User Guides](#power-user-guides)
    - [Enterprise Authentication \& Identity](#enterprise-authentication--identity)
    - [Programming LAnguages, Data Structures \& Identity](#programming-languages-data-structures--identity)
    - [Django Development](#django-development)
    - [.NET Development](#net-development)
    - [Containerization \& DevOps](#containerization--devops)
    - [Databases](#databases)
    - [Security \& Networking](#security--networking)
    - [Development Tools](#development-tools)
  - [PowerShell Scripts](#powershell-scripts)
    - [Directory Navigation (`directory-navigation.ps1`)](#directory-navigation-directory-navigationps1)
    - [File Operations (`file-operations.ps1`)](#file-operations-file-operationsps1)
    - [GitHub Management (`github-management.ps1`)](#github-management-github-managementps1)
    - [Document Conversion (`document-conversion.ps1`)](#document-conversion-document-conversionps1)
    - [Python Environment (`python-environment.ps1`)](#python-environment-python-environmentps1)
    - [Profile Management (`profile-management.ps1`)](#profile-management-profile-managementps1)
    - [Utility Functions (`utility-functions.ps1`)](#utility-functions-utility-functionsps1)
    - [File System Management (`file-system_management.ps1`)](#file-system-management-file-system_managementps1)
    - [File Size Lister (`filesize-lister.ps1`)](#file-size-lister-filesize-listerps1)
    - [Media Download (`media-download.ps1`)](#media-download-media-downloadps1)
    - [Job Scheduler (`job-scheduler_template.ps1`)](#job-scheduler-job-scheduler_templateps1)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
  - [Usage Examples](#usage-examples)
    - [Example 1: Quick Directory Navigation](#example-1-quick-directory-navigation)
    - [Example 2: GitHub Workflow Automation](#example-2-github-workflow-automation)
    - [Example 3: File Operations](#example-3-file-operations)
    - [Example 4: Python Environment Setup](#example-4-python-environment-setup)
    - [Example 5: System Analysis](#example-5-system-analysis)
    - [Example 6: Using Technical Guides](#example-6-using-technical-guides)
  - [Contributing](#contributing)
    - [Contribution Guidelines](#contribution-guidelines)
  - [License](#license)
  - [Contact](#contact)
  - [Acknowledgments](#acknowledgments)
  - [Statistics](#statistics)

---

## Purpose

This repository serves two primary purposes:

1. **Technical Documentation**: Comprehensive power user guides for backend engineers, platform engineers, security engineers, and SREs covering enterprise-level technologies
2. **Automation Scripts**: Production-ready PowerShell scripts for Windows system management, file operations, GitHub workflows, and development automation

All guides follow a consistent template with quickstart instructions, key concepts, configuration best practices, security considerations, detailed examples, troubleshooting tips, and performance tuning recommendations.

## Repository Structure

```
system-management_scripts/
├── guides/                  # Technical power user guides
│   ├── AUTH_SERVICES_*.md   # Enterprise authentication (OAuth2, OIDC, SAML, SCIM)
│   ├── DOCKER_*.md          # Container management and orchestration
│   ├── DOTNET_*.md          # .NET libraries (BCrypt, RabbitMQ)
│   ├── POSTGRESQL_*.md      # Database administration
│   ├── REDIS_*.md           # In-memory caching
│   ├── SSL_TLS_*.md         # Certificate management
│   ├── DJANGO_MULTI-AUTHENTICATION_*.md  # Django authentication strategies
|   ├── C_SHARP_*.md         # C# guides
|   ├── MEMORY_MANAGEMENT_*.md # Memory management guides (C#, C++, Python, JavaScript)
│   └── VI_*.md              # Text editor mastery
│
├── windows/                 # PowerShell automation scripts
│   ├── directory-navigation.ps1    # Quick directory navigation
│   ├── document-conversion.ps1     # Document format conversion
│   ├── file-operations.ps1         # File/folder operations
│   ├── file-system_management.ps1  # Filesystem utilities
│   ├── filesize-lister.ps1         # Directory size analysis
│   ├── github-management.ps1       # GitHub workflow automation
│   ├── job-scheduler_template.ps1  # Task scheduling
│   ├── media-download.ps1          # Media download utilities
│   ├── profile-management.ps1      # PowerShell profile setup
│   ├── python-environment.ps1      # Python environment management
│   └── utility-functions.ps1       # General utilities
│
└── README.md               # This file
```

---

## Power User Guides

### Enterprise Authentication & Identity

- **[AUTH_SERVICES_CSHARP_POWERUSER_GUIDE.md](guides/AUTH_SERVICES_CSHARP_POWERUSER_GUIDE.md)**  
  OAuth 2.0, OIDC, SAML, JWT implementation in C#; ASP.NET Core authentication; SCIM provisioning; token lifecycle management
  
- **[AUTH_SERVICES_POWERSHELL_POWERUSER_GUIDE.md](guides/AUTH_SERVICES_POWERSHELL_POWERUSER_GUIDE.md)**  
  Azure AD management with Microsoft Graph; service principal automation; conditional access policies; certificate-based auth

### Programming LAnguages, Data Structures & Identity

- **[C_SHARP_PROGRAMMING_DATA_STRUCTURES.md](guides/C_SHARP_PROGRAMMING_DATA_STRUCTURES.md)**  
  C# development with PowerShell integration; compiling and running C# code; automating builds; interop scenarios
- **[MEMORY_MANAGEMENT_CSHARP_POWERUSER_GUIDE.md](guides/MEMORY_MANAGEMENT_CSHARP_POWERUSER_GUIDE.md)**  
  C# memory management on Windows; value vs reference types; stack vs heap storage; copy semantics; nullability features
- **[MEMORY_MANAGEMENT_CPP_POWERUSER_GUIDE.md](guides/MEMORY_MANAGEMENT_CPP_POWERUSER_GUIDE.md)**  
  C++ memory management on Windows (MSVC); value vs reference semantics; stack vs heap storage; copy semantics; nullability
- **[MEMORY_MANAGEMENT_PYTHON_POWERUSER_GUIDE.md](guides/MEMORY_MANAGEMENT_PYTHON_POWERUSER_GUIDE.md)**  
  Python memory management (CPython on Windows); value vs reference semantics; heap storage; copy semantics; nullability
- **[MEMORY_MANAGEMENT_JAVASCRIPT_POWERUSER_GUIDE.md](guides/MEMORY_MANAGEMENT_JAVASCRIPT_POWERUSER_GUIDE.md)**  
  JavaScript memory management (Node.js on Windows); value vs reference types; heap-managed objects; copy semantics; nullability

### Django Development

- **[DJANGO_MULTI-AUTHENTICATION_POWERSHELL_POWERUSER_GUIDE.md](guides/DJANGO_MULTI-AUTHENTICATION_POWERSHELL_POWERUSER_GUIDE.md)**  
  Implementing authentication in Django applications; OAuth2 and JWT integration; user management; security best practices; setting up multi-factor authentication in Django; integrating with third-party MFA providers; enhancing application security

- **[DJANGO_MULTI-AUTHENTICATION_PYTHON_POWERUSER_GUIDE.md](guides/DJANGO_MULTI-AUTHENTICATION_PYTHON_POWERUSER_GUIDE.md)**  
  Implementing authentication in Django applications; OAuth2 and JWT integration; user management; security best practices; setting up multi-factor authentication in Django; integrating with third-party MFA providers; enhancing application security

- **[DJANGO_MULTI-AUTHENTICATION_BASH_POWERUSER_GUIDE.md](guides/DJANGO_MULTI-AUTHENTICATION_BASH_POWERUSER_GUIDE.md)**  
  Implementing authentication in Django applications; OAuth2 and JWT integration; user management; security best practices; setting up multi-factor authentication in Django; integrating with third-party MFA providers; enhancing application security

### .NET Development

- **[DOTNET_BCRYPT_CSHARP_POWERUSER_GUIDE.md](guides/DOTNET_BCRYPT_CSHARP_POWERUSER_GUIDE.md)**  
  Password hashing with BCrypt.Net-Next; secure authentication patterns; work factor tuning; ASP.NET Core integration
  
- **[DOTNET_RABBITMQ_CSHARP_POWERUSER_GUIDE.md](guides/DOTNET_RABBITMQ_CSHARP_POWERUSER_GUIDE.md)**  
  RabbitMQ message broker integration; exchange patterns; dead-letter queues; connection pooling; async patterns

### Containerization & DevOps

- **[DOCKER_POWERSHELL_POWERUSER_GUIDE.md](guides/DOCKER_POWERSHELL_POWERUSER_GUIDE.md)**  
  Docker container management on Windows; multi-stage builds; Docker Compose; volume management; networking

### Databases
- **[POSTGRESQL_16_BASH_POWERUSER_GUIDE.md](guides/POSTGRESQL_16_BASH_POWERUSER_GUIDE.md)**  
  PostgreSQL administration on Linux; performance tuning; backup strategies; replication; query optimization
  
- **[POSTGRESQL_16_POWERSHELL_POWERUSER_GUIDE.md](guides/POSTGRESQL_16_POWERSHELL_POWERUSER_GUIDE.md)**  
  PostgreSQL administration on Windows; connection pooling; automated backups; monitoring
  
- **[REDIS_POWERSHELL_POWERUSER_GUIDE.md](guides/REDIS_POWERSHELL_POWERUSER_GUIDE.md)**  
  Redis in-memory caching; data structures; persistence; clustering; PowerShell client integration

### Security & Networking

- **[SSL_TLS_BASH_POWERUSER_GUIDE.md](guides/SSL_TLS_BASH_POWERUSER_GUIDE.md)**  
  Certificate management on Linux; OpenSSL operations; certificate authorities; TLS configuration
  
- **[SSL_TLS_POWERSHELL_POWERUSER_GUIDE.md](guides/SSL_TLS_POWERSHELL_POWERUSER_GUIDE.md)**  
  Certificate management on Windows; PKI infrastructure; automated certificate rotation; IIS configuration

### Development Tools

- **[VI_POWERUSER_GUIDE.md](guides/VI_POWERUSER_GUIDE.md)**  
  Vi/Vim text editor mastery; navigation; editing commands; macros; configuration

---

## PowerShell Scripts

### Directory Navigation (`directory-navigation.ps1`)

Quick navigation functions for common directories:
- `ChDir-Work` - Navigate to work directory
- `ChDir-Documents` - Navigate to Documents folder
- `ChDir-Downloads` - Navigate to Downloads folder
- `ChDir-Desktop` - Navigate to Desktop
- `ChDir-OneDrive` - Navigate to OneDrive directory

### File Operations (`file-operations.ps1`)

Advanced file and folder operations:
- `MoveItem-Overwrite` - Move with automatic overwrite
- `CopyItem-Safe` - Safe copy with conflict handling
- `Remove-EmptyDirectories` - Clean up empty folders recursively
- `Get-FileHash-Bulk` - Compute hashes for multiple files
- `Compare-DirectoryContent` - Compare two directory structures

### GitHub Management (`github-management.ps1`)

Automated GitHub repository workflows:
- `Manage-GitHubAppDev` - Full repository management workflow
- `Initialize-GitRepository` - Initialize new repositories
- `Create-GitTag` - Create and push tags
- `Create-GitHubRelease` - Automated release creation
- `Sync-GitHubFork` - Keep forks synchronized

### Document Conversion (`document-conversion.ps1`)

Document format conversion utilities:
- `Convert-MarkdownToHtml` - Markdown to HTML conversion
- `Convert-MarkdownToPdf` - Markdown to PDF conversion
- `Convert-HtmlToPdf` - HTML to PDF conversion
- `Batch-ConvertDocuments` - Bulk document conversion

### Python Environment (`python-environment.ps1`)

Python environment management:
- `New-PythonVenv` - Create virtual environments
- `Activate-PythonVenv` - Activate virtual environment
- `Install-PythonPackages` - Bulk package installation
- `Export-PythonRequirements` - Generate requirements.txt
- `Update-PythonPackages` - Update all packages

### Profile Management (`profile-management.ps1`)

PowerShell profile configuration:
- `Install-PowerShellProfile` - Set up custom profile
- `Add-ProfileFunction` - Add functions to profile
- `Backup-PowerShellProfile` - Backup profile configuration
- `Restore-PowerShellProfile` - Restore from backup

### Utility Functions (`utility-functions.ps1`)

General-purpose utilities:
- `Test-Administrator` - Check admin privileges
- `Get-SystemInfo` - Display system information
- `Test-InternetConnection` - Network connectivity check
- `Get-InstalledSoftware` - List installed applications
- `Measure-CommandTime` - Benchmark command execution

### File System Management (`file-system_management.ps1`)

Advanced filesystem utilities:
- `Get-LargestFiles` - Find largest files in directory tree
- `Get-DuplicateFiles` - Detect duplicate files by hash
- `Compress-OldFiles` - Archive files older than specified date
- `Export-DirectoryStructure` - Generate directory tree report

### File Size Lister (`filesize-lister.ps1`)

Directory size analysis:
- `Get-DirectorySize` - Calculate folder sizes recursively
- `Export-SizeReport` - Generate size report CSV
- `Find-LargeDirectories` - Identify space-consuming folders

### Media Download (`media-download.ps1`)

Media download utilities:
- `Download-YouTubeVideo` - Download YouTube videos
- `Download-Playlist` - Download entire playlists
- `Convert-MediaFormat` - Convert media formats
- `Extract-AudioFromVideo` - Extract audio tracks

### Job Scheduler (`job-scheduler_template.ps1`)

Task scheduling framework:
- `New-ScheduledTask` - Create scheduled tasks
- `Register-TaskScheduler` - Register with Windows Task Scheduler
- `Remove-ScheduledTask` - Remove scheduled tasks
- `Get-TaskStatus` - Check task execution status

---

## Getting Started

### Prerequisites

**For PowerShell Scripts:**
- Windows 10/11 or Windows Server 2016+
- PowerShell 7.0 or later (recommended)
- Administrator privileges (for some operations)

**For Guides:**
- Relevant technology installed (Docker, PostgreSQL, Redis, etc.)
- Basic understanding of the technology stack
- Command-line familiarity

### Installation

1. **Clone the repository:**
```powershell
git clone https://github.com/paulnamalomba/system-management_scripts.git
cd system-management_scripts
```

2. **Set execution policy (if needed):**
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

3. **Import scripts into your PowerShell session:**
```powershell
# Import all functions from a script
. .\windows\file-operations.ps1
. .\windows\github-management.ps1

# Or add to your PowerShell profile for persistent availability
```

4. **Add to PowerShell Profile (Optional):**
```powershell
# Edit your profile
notepad $PROFILE

# Add this line to source scripts automatically
Get-ChildItem "C:\Path\To\system-management_scripts\windows\*.ps1" | ForEach-Object { . $_.FullName }
```

---

## Usage Examples

### Example 1: Quick Directory Navigation

```powershell
# Load navigation functions
. .\windows\directory-navigation.ps1

# Navigate to work directory
ChDir-Work -workPath "C:\Projects"

# Navigate to OneDrive
ChDir-OneDrive
```

### Example 2: GitHub Workflow Automation

```powershell
# Load GitHub management functions
. .\windows\github-management.ps1

# Automated commit, tag, and release
Manage-GitHubAppDev `
    -appName "my-project" `
    -commitTag "v1.2.0" `
    -commitMessage "Added new features and bug fixes" `
    -method "update"
```

### Example 3: File Operations

```powershell
# Load file operations
. .\windows\file-operations.ps1

# Move with overwrite
MoveItem-Overwrite -Src "C:\Source\File.txt" -Dest "C:\Destination\File.txt"

# Find and remove empty directories
Remove-EmptyDirectories -Path "C:\Projects" -Recurse
```

### Example 4: Python Environment Setup

```powershell
# Load Python environment functions
. .\windows\python-environment.ps1

# Create new virtual environment
New-PythonVenv -Path ".\venv" -PythonVersion "3.11"

# Activate environment
Activate-PythonVenv -Path ".\venv"

# Install packages from requirements.txt
Install-PythonPackages -RequirementsFile ".\requirements.txt"
```

### Example 5: System Analysis

```powershell
# Load utility functions
. .\windows\utility-functions.ps1

# Check if running as administrator
if (Test-Administrator) {
    Write-Host "Running with admin privileges"
}

# Get system information
Get-SystemInfo

# List installed software
Get-InstalledSoftware | Where-Object { $_.Name -like "*Visual Studio*" }
```

### Example 6: Using Technical Guides

```powershell
# Navigate to guides directory
cd guides

# View available guides
Get-ChildItem *.md | Select-Object Name

# Open a guide in your default markdown viewer
Start-Process .\DOCKER_POWERSHELL_POWERUSER_GUIDE.md

# Or view in terminal with bat (if installed)
bat .\POSTGRESQL_16_POWERSHELL_POWERUSER_GUIDE.md
```

---

## Contributing

Contributions are welcome! Please follow these guidelines:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit your changes**: `git commit -m 'Add amazing feature'`
4. **Push to the branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### Contribution Guidelines

**For PowerShell Scripts:**
- Follow PowerShell best practices and style guidelines
- Include comment-based help for all functions
- Add parameter validation and error handling
- Test on PowerShell 7+ before submitting

**For Technical Guides:**
- Follow the existing template structure
- Include practical, copy-paste ready examples
- Cover security considerations and best practices
- Add troubleshooting section with common issues
- Include references and further reading

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact

**Paul Namalomba**
- GitHub: [@paulnamalomba](https://github.com/paulnamalomba)
- Email: kabwenzenamalomba@gmail.com
- Website: [https://paulnamalomba.github.io](https://paulnamalomba.github.io)
- LinkedIn: [Paul Namalomba](https://www.linkedin.com/in/paulnamalomba/)

---

## Acknowledgments

- PowerShell community for extensive documentation and examples
- Microsoft Graph PowerShell SDK team
- Open-source contributors to the technologies covered in guides
- DevOps and SRE communities for best practices

---

## Statistics

- **Power User Guides**: 15 comprehensive technical guides
- **PowerShell Scripts**: 11 automation script collections
- **Technologies Covered**: Docker, PostgreSQL, Redis, RabbitMQ, Azure AD, SSL/TLS, .NET, and more
- **Lines of Documentation**: 10,000+ lines of technical documentation
- **Code Examples**: 100+ production-ready code snippets

---

**Last Updated**: December 13, 2025  
**Repository Status**: Active Development  
**PowerShell Version**: 7.0+  
**Windows Compatibility**: Windows 10/11, Server 2016+
