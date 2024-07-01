# IT Lab Setup Part 3: Active Directory Account Creation and Essential CMD Commands

This part of the IT Lab series continues our exploration of Active Directory with the creation of a specialized user account named "HelpDesk" and introduces several crucial CMD commands that are foundational for anyone in an IT support role, especially useful for help desk operations.

## Objectives

- Create a specialized "HelpDesk" user account in Active Directory with appropriate permissions.
- Introduce essential CMD commands for effective network management and troubleshooting.

## Prerequisites

- Completion of Part 2 where Active Directory Domain Services was installed.
- Windows Server 2016 running on VirtualBox.

## Steps

### 1. Log into Your Virtual Machine

Start by launching your Server 2016 VM in VirtualBox:

1. Open VirtualBox and start the `Server 2016 Lab` VM.
2. Log in using the administrator credentials established in previous labs.

### 2. Creating the "HelpDesk" User Account

We will use the Active Directory Users and Computers management console to create a new user account called "HelpDesk" with appropriate permissions for help desk operations.

1. Open **Server Manager**.
2. Go to **Tools > Active Directory Users and Computers**.
3. Right-click on the `Users` container and select **Copy** on an existing user like `Administrator` to use as a template.
4. Enter the new user details for "HelpDesk". Set a strong password and specify the necessary group memberships based on required access levels.

    ![Creating Help Desk User](https://path_to_your_image/create-help-desk-user.png "Creating the HelpDesk User Account")

### 3. Essential CMD Commands for IT Support

#### Basic Network Configuration and Troubleshooting

- **IP Configuration**: View detailed network configuration.
  ```cmd
  ipconfig /all
