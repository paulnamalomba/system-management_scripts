# System Management Scripts

A collection of PowerShell scripts for automating common system management tasks on Windows. These scripts help with file operations, directory navigation, document conversion, Python environment management, media downloads, and GitHub repository management.

## Table of Contents

- [Installation](#installation)
- [Scripts Overview](#scripts-overview)
- [Usage Examples](#usage-examples)
- [Configuration](#configuration)
- [Contributing](#contributing)

## Installation

### Prerequisites

- Windows 10/11
- PowerShell 5.1 or PowerShell 7+
- Git (for GitHub management scripts)
- Python 3.x (for Python environment scripts)
- Pandoc and XeLaTeX (for document conversion)
- yt-dlp and ffmpeg (for media download scripts)

### Setup

1. Clone this repository:
```powershell
git clone https://github.com/yourusername/system-management_scripts.git
cd system-management_scripts
```

2. Import the scripts you need into your PowerShell profile or dot-source them:
```powershell
# Add to your $PROFILE
. "C:\path\to\system-management_scripts\windows\file-operations.ps1"
. "C:\path\to\system-management_scripts\windows\directory-navigation.ps1"
# ... add other scripts as needed
```

3. Configure paths in each script by replacing placeholders like `<path/to/folder>` with your actual paths.

## Scripts Overview

### 1. **file-operations.ps1**
Functions for file and folder operations.

**Functions:**
- `MoveItem-Overwrite` - Moves items with automatic overwrite
- `RenameFolders-FirstLetterUppercase` - Renames folders to capitalize first letter
- `ListSize-Directory` - Lists directory sizes in GB

**Example:**
```powershell
# List sizes of all subdirectories
ListSize-Directory

# Rename folders to have first letter uppercase
RenameFolders-FirstLetterUppercase -Path "C:\MyFolder"

# Move with overwrite
MoveItem-Overwrite -Src "C:\source\file.txt" -Dest "C:\destination\file.txt"
```

### 2. **directory-navigation.ps1**
Quick navigation functions for common directories.

**Functions:**
- `ChDir-Work` - Navigate to work folder
- `ChDir-Documents` - Navigate to Documents
- `ChDir-Downloads` - Navigate to Downloads
- `ChDir-CustomProject` - Template for custom project directories

**Example:**
```powershell
# Navigate to work folder
ChDir-Work -workPath "C:\Projects\Work"

# Navigate to Documents
ChDir-Documents

# Navigate to custom project
ChDir-CustomProject -projectPath "C:\Projects\MyApp"
```

### 3. **document-conversion.ps1**
Document format conversion utilities.

**Functions:**
- `ConvertMD-ToPDF` - Convert Markdown to PDF using Pandoc

**Example:**
```powershell
# Basic conversion
ConvertMD-ToPDF -inputFile "document.md"

# With custom font and size
ConvertMD-ToPDF -inputFile "document.md" -fontName "Arial" -fontSize "11pt"
```

### 4. **python-environment.ps1**
Python virtual environment management.

**Functions:**
- `ActivatePyEnv-Py3Env` - Activate a Python virtual environment

**Example:**
```powershell
# Activate default environment
ActivatePyEnv-Py3Env

# Activate specific environment
ActivatePyEnv-Py3Env -envName "myenv" -envBasePath "C:\VirtualEnvs"
```

### 5. **media-download.ps1**
YouTube and media download utilities using yt-dlp.

**Functions:**
- `YtDL-Playlist` - Download entire YouTube playlists as MP3
- `YtDL-Song` - Download single YouTube videos as MP3

**Example:**
```powershell
# Download a playlist
YtDL-Playlist -playlistUrl "https://youtube.com/playlist?list=..." -ytdlpPath "C:\Tools\yt-dlp.exe"

# Download a single song
YtDL-Song -songUrl "https://youtube.com/watch?v=..." -ytdlpPath "C:\Tools\yt-dlp.exe"
```

### 6. **github-management.ps1**
Automated GitHub repository management.

**Functions:**
- `Manage-GitHubAppDev` - Manage development workflow (commit, tag, push)
- `Manage-GitTags` - Manage Git tags (list, create, delete)

**Example:**
```powershell
# Update repository with new tag
Manage-GitHubAppDev -appName "my-app" -commitTag "v1.0.0" -commitMessage "Release v1.0.0" -method "update"

# List all tags for a repository
Manage-GitTags -appName "my-app" -method "list"

# Delete a tag
Manage-GitTags -appName "my-app" -commitTag "v0.9.0" -method "delete"
```

### 7. **profile-management.ps1**
PowerShell profile management utilities.

**Functions:**
- `Load-Profile` - Reload PowerShell profile without restarting

**Example:**
```powershell
# Reload current profile
Load-Profile

# Reload specific profile
Load-Profile -profilePath "C:\Users\Username\Documents\PowerShell\Microsoft.PowerShell_profile.ps1"
```

### 8. **utility-functions.ps1**
Miscellaneous utility functions.

**Functions:**
- `Get-CurrentTime` - Get current time in HH:mm:ss format
- `InstallBulk-Fonts` - Install multiple fonts from a folder

**Example:**
```powershell
# Get current time
$time = Get-CurrentTime
Write-Host "Current time: $time"

# Install fonts
InstallBulk-Fonts -family "Arial" -fontFolder "C:\Fonts"
```

### 9. **filesize-lister.ps1**
Already existing script for listing file sizes.

### 10. **file-system_management.ps1**
Already existing script for file system management.

### 11. **job-scheduler_template.ps1**
Already existing template for Windows Task Scheduler jobs.

## Configuration

### Path Configuration

Each script uses placeholder paths like `<path/to/folder>`. Before using, replace these with your actual paths:

1. Open the script file
2. Find placeholders: `<path/to/folder>`, `<path/to/yt-dlp.exe>`, etc.
3. Replace with actual paths on your system

Example:
```powershell
# Before
[string]$ytdlpPath = "<path/to/yt-dlp.exe>"

# After
[string]$ytdlpPath = "C:\Tools\yt-dlp.exe"
```

### Adding to PowerShell Profile

To make these functions available in every PowerShell session:

1. Open your PowerShell profile:
```powershell
notepad $PROFILE
```

2. Add dot-source commands:
```powershell
# Source system management scripts
$scriptPath = "C:\path\to\system-management_scripts\windows"
. "$scriptPath\file-operations.ps1"
. "$scriptPath\directory-navigation.ps1"
. "$scriptPath\document-conversion.ps1"
. "$scriptPath\python-environment.ps1"
. "$scriptPath\media-download.ps1"
. "$scriptPath\github-management.ps1"
. "$scriptPath\profile-management.ps1"
. "$scriptPath\utility-functions.ps1"
```

3. Save and reload your profile:
```powershell
. $PROFILE
```

## Usage Examples

### Complete Workflow Example

```powershell
# 1. Navigate to your project
ChDir-CustomProject -projectPath "C:\Projects\MyApp"

# 2. Activate Python environment
ActivatePyEnv-Py3Env -envName "myapp-env"

# 3. Do your work...

# 4. Commit and tag to GitHub
Manage-GitHubAppDev -appName "MyApp" -commitTag "v1.2.0" -commitMessage "Added new features" -method "update"

# 5. Download documentation resources
YtDL-Song -songUrl "https://youtube.com/watch?v=tutorial-video"

# 6. Convert documentation
ConvertMD-ToPDF -inputFile "README.md"
```

### Bulk Operations Example

```powershell
# List all directory sizes to find large folders
ChDir-Work
ListSize-Directory

# Rename all folders to have proper capitalization
RenameFolders-FirstLetterUppercase

# Install custom fonts for documentation
InstallBulk-Fonts -family "CustomFonts" -fontFolder "C:\Fonts"
```

## PowerShell Verb Warnings

Note: Some functions use non-standard PowerShell verbs (e.g., `ChDir-`, `YtDL-`). This is intentional for brevity and convenience in interactive use. The warnings can be safely ignored, or you can create aliases with approved verbs:

```powershell
# Create aliases with approved verbs
Set-Alias -Name Set-WorkDirectory -Value ChDir-Work
Set-Alias -Name Get-YouTubePlaylist -Value YtDL-Playlist
```

## Requirements by Script

| Script | Dependencies |
|--------|--------------|
| document-conversion.ps1 | Pandoc, XeLaTeX |
| media-download.ps1 | yt-dlp, ffmpeg |
| github-management.ps1 | Git, GitHub CLI (optional) |
| python-environment.ps1 | Python 3.x, venv |
| utility-functions.ps1 | Administrator rights (for font installation) |

## Security Notes

- **GitHub Management**: These scripts may handle sensitive repository operations. Always review changes before confirming.
- **Path Security**: Ensure paths don't expose sensitive information when sharing scripts.
- **Execution Policy**: You may need to adjust your PowerShell execution policy:
  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```

## Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch
3. Make your changes with clear commit messages
4. Ensure all placeholder paths are properly marked
5. Submit a pull request

## License

This project is provided as-is for personal and educational use. Modify as needed for your environment.

## Troubleshooting

### Common Issues

1. **Script not found**: Ensure you're using the correct path when dot-sourcing
2. **Permission denied**: Some functions (like font installation) require administrator rights
3. **Module not loaded**: Some functions use `Export-ModuleMember` - ensure the script is properly sourced
4. **Path not found**: Replace all `<path/to/folder>` placeholders with actual paths

### Getting Help

Each function includes comprehensive help documentation:
```powershell
Get-Help FunctionName -Full
Get-Help ConvertMD-ToPDF -Examples
```

## Author

Created for personal system management automation. Sanitized and shared for community benefit.

---

**Last Updated**: January 2025
