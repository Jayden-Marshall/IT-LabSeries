# IT Lab Setup Part 1

This repository provides a guide and resources for setting up a basic IT lab using VirtualBox and Windows Server 2016. This lab is intended for beginners in IT, particularly those interested in Help Desk and IT support roles.

## Requirements

- A computer with sufficient hardware resources (minimum 8GB RAM recommended)
- [VirtualBox](https://www.virtualbox.org/) installed
- Windows Server 2016 ISO file (download from [Microsoft Evaluation Center](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2016))

## Steps

### 1. Download and Install VirtualBox

1. Go to [VirtualBox download page](https://www.virtualbox.org/wiki/Downloads).
2. Download the appropriate version for your operating system (Windows, macOS, Linux).
3. Install VirtualBox by following the installation wizard.

### 2. Check System Requirements

1. Open `This PC` or `My Computer`.
2. Right-click and select `Properties` to view your system specifications.
3. Ensure you have at least 8GB of RAM.

### 3. Enable Virtualization in BIOS

1. Restart your computer, and enter BIOS/UEFI settings (usually by pressing `F2`, `F10`, `Del`, or `Esc` during boot).
2. Find the `Virtualization Technology` setting and enable it.
3. Save and exit BIOS.

### 4. Download Windows Server 2016 ISO

1. Go to the [Microsoft Evaluation Center](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2016).
2. Download the ISO file for Windows Server 2016.

### 5. Create a Virtual Machine in VirtualBox

1. Open VirtualBox and click `New`.
2. Name the VM (e.g., `Server 2016 Lab`), set the type to `Microsoft Windows`, and version to `Windows 2016 (64-bit)`.
3. Allocate at least 4GB of RAM (8GB recommended).
4. Create a virtual hard disk (VDI) with at least 50GB of storage.
5. Start the VM, and select the Windows Server 2016 ISO file as the startup disk.

### 6. Install Windows Server 2016

1. Follow the installation prompts to install Windows Server 2016.
2. Choose `Windows Server 2016 Standard (Desktop Experience)` when prompted.
3. Complete the installation and initial setup.

## Additional Resources

- [VirtualBox User Manual](https://www.virtualbox.org/manual/UserManual.html)
- [Microsoft Docs: Windows Server 2016](https://docs.microsoft.com/en-us/windows-server/get-started/windows-server-2016)

