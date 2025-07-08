# VirtualBox KVM-Patched Version

This is a patched version of VirtualBox 7.1.6 with KVM support improvements.

## Features
- **Self-contained RPM**: All required libraries (Qt6, OpenGL, curl, etc.) are bundled
- **KVM support**: Enhanced KVM compatibility patches applied
- **Easy deployment**: No need to manually install dependencies

## Installation

### System Requirements
- Fedora 42 with kernel 6.15.4-200.fc42.x86_64
- Basic system packages: `kernel-devel`, `dkms`

### Install
```bash
sudo dnf install -y kernel-devel dkms
sudo dnf install VirtualBox-patched-7.1.6-1.fc42.x86_64.rpm
```

### Usage
After installation, VirtualBox can be started from:
- Applications menu (GUI)
- Command line: `VirtualBox`
- VirtualBox Manager: `VBoxManage`

## What's Included
- VirtualBox GUI and command-line tools
- All necessary Qt6 libraries
- OpenGL/GLX libraries
- Network and XML libraries
- Proper desktop integration

## Notes
- The RPM conflicts with the standard VirtualBox package
- All dependencies are bundled - no external library installation needed
- Uses wrapper scripts to ensure proper library loading
