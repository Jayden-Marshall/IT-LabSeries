# IT Lab Setup Part 2

This part of the IT Lab series covers the installation and configuration of Active Directory Domain Services (AD DS) on Windows Server 2016. This setup is essential for anyone looking to deepen their understanding of network management and Windows Server administration.

## Objectives

- Rename the server to simplify management.
- Install Active Directory Domain Services to create a domain controller.

## Requirements

- Completed Part 1: Installation of Windows Server 2016 on VirtualBox.
- Windows Server 2016 operational on VirtualBox.

## Steps

### 1. Rename the Server

Renaming the server provides a simpler and more manageable reference throughout the IT lab series.

1. Log into your Windows Server 2016 VM.
2. Open the File Explorer and right-click on 'This PC'.
3. Select 'Properties' and then 'Change settings' next to the computer name.
4. Click 'Change...' and enter a new computer name, such as `Server2016`.
5. Click 'OK', and restart the server for the changes to take effect.

   ![Change Computer Name](https://github.com/Jayden-Marshall/IT-LabSeries/blob/main/Part2/ImageChangeComputerName.md)

### 2. Install Active Directory Domain Services

Setting up AD DS turns the server into a domain controller, managing network resources such as user data, security, and other directory services.

1. Log into the server post-restart.
2. Open 'Server Manager'.
3. Select 'Manage' and then 'Add Roles and Features'.
4. Proceed to the 'Roles' section and check 'Active Directory Domain Services'. Add all required features and tools when prompted.
5. Continue and finalize the installation. Do not close the wizard until you see the prompt to configure AD DS.

   ![Installing Active Directory Domain Services](https://github.com/Jayden-Marshall/IT-LabSeries/blob/main/Part2/ImageInstallingADDS.md)

### 3. Promote the Server to a Domain Controller

After installing AD DS, the next step involves promoting the server to a domain controller.

1. Once AD DS installation completes, click on the notification flag in Server Manager and select 'Promote this server to a domain controller'.
2. Choose 'Add a new forest' and type your desired domain name (e.g., `jaymarsh.com`).
3. Follow the prompts to configure the domain controller settings, including DSRM (Directory Services Restore Mode) password.
4. Confirm the settings and click 'Install'. The server will restart automatically upon completion.


## What's Next?

In the upcoming parts of this series, we will configure user accounts, join a client PC to the domain, and delve into group policy management. Stay tuned as we expand our IT skills further!

## Additional Resources

- [Active Directory Basics on Microsoft Docs](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
- [How to Manage Active Directory Domain Services](https://www.manageengine.com/products/active-directory-audit/kb/how-to/how-to-setup-a-domain-controller.html)

