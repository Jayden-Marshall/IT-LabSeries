# IT Lab Setup Part 4

Welcome back to our IT lab setup series! In Lab 3, we created a HelpDesk account, enabled the Recycle Bin on Server 2016, and learned how to copy and create admin accounts. Today, we're taking a big step forward by installing Windows 10 on a VM and joining it to a domain. This lab will equip you with essential skills for managing Windows environments in a real-world IT support and help desk role.

## Installation of Windows 10 on a VM

Today's focus is on getting Windows 10 up and running inside a virtual environment and integrating it within our existing domain structure. Follow these steps:

### 1. Open VirtualBox

- Start by launching VirtualBox where your Server 2016 is already operational.
- Log in using the HelpDesk account we configured previously.

### 2. Download Windows 10 ISO

- Visit the official [Windows 10 download page](https://www.microsoft.com/software-download/windows10ISO) to get the ISO file.
- Select 'Create Installation Media for another PC', then choose 'ISO file'. This allows you to save the ISO directly to your system.
- Store the ISO in an accessible location, as you'll need it shortly to set up the new VM.

### 3. Create and Configure the New VM

- In VirtualBox, click 'New' to initiate the creation of a new virtual machine.
- Name your VM "Windows 10 Lab" for clarity.
- Allocate at least 8GB of RAM for optimal performance.
- Attach the Windows 10 ISO you downloaded to the virtual drive.
- Power on the VM and follow the on-screen instructions to install Windows 10.

## Join the VM to the Domain

Configuring our VM to join the domain is a critical step for network integration and management.

### 1. Network Configuration

- Adjust the VM's network settings to use a static IP that matches the subnet of your domain controller. This ensures seamless communication.
- Confirm network connectivity using tools like `ping` or `nslookup` to ensure the VM can reach the domain controller.

### 2. Domain Joining

- Right-click 'This PC', go to 'Properties', and then 'Change settings'.
- Click 'Change...' and select the 'Domain' option to enter your domain name.
- Input your domain credentials when prompted to authenticate the join.

## Additional Configuration

### 1. Software Installation

- Install essential applications such as Google Chrome or Firefox for web access, and TeamViewer for remote management capabilities.
- These tools are vital for a fully functional IT support environment.

### 2. Firewall Configuration

- Adjust the firewall settings to allow specific network traffic for domain communication and external connectivity.

## Wrapping Up

By the end of this lab, your Windows 10 VM will be fully set up and integrated into the domain, ready for you to perform a variety of network tasks and management operations. This practical setup prepares you for real-world IT scenarios and enhances your troubleshooting skills.

Stay tuned for the next part of our series, where we'll delve into advanced domain management and tackle more complex configurations!

**Pro Tip:** Always double-check your configurations and maintain backups to ensure you can restore your virtual environment if necessary.
