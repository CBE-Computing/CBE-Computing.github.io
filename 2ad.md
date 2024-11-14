---
layout: page
title: 2. Active Directory
description: >-
    Detailing the initial setup procedures for a device
parent: Setup
---

# Microsoft Active Directory
{:.no_toc}

1. TOC
{:toc}

---

## What is Active Directory

Microsoft Active Directory (AD) is a directory service that enables centralized domain management and security in an organization. AD organizes users, computers, and resources, allowing administrators to manage permissions and access controls for network resources. By integrating Apple devices with AD, you can leverage existing security and identity management while ensuring seamless access to shared resources, applications, and network configurations. Our main use case is to allow our end users to be able to log in to their device via their UW NetID.

---

## Steps for Adding a Device in Active Directory

To add a new device to Active Directory, follow these steps:

1. **Access RDWEB via Windows App**  
    Access RDWEB via Windows App to access the Directory Services Tool. Eric should have put this somewhere on solo. Log in with your NetID. You will be see a CMD prompt to sign in with the *a_cbeit* account. After sign in type *dsa* and hit enter.

    ![Windows App Sign-In](../assets/images/ad/ad1.png)

    ![Windows DSA](../assets/images/ad/ad2.png)

2. **Add New AD Object**  
    Add the new AD Object inside the tool. Make sure to follow the naming conventions CBE-['Asset Tag'] and to include a description.

    ![Add AD Object](../assets/images/ad/ad3.png)

---

## Steps for Manually Binding a Device to Active Directory

Once the device is added to Active Directory, the device if properly named should bind automatically with a policy that I've setup. If it has not, follow the instructions below to manually bind the device to the AD NetID domain.

   {: .warning }
   >**If you unbind the device it will delete the object in Active Directory.**

1. **Navigate to Directory Utility**  
    Open *Directory Utility* and click on the lock. Sign in with the motley account. Click on *Active Directory*.
    ![Add AD Object](../assets/images/ad/ad4.png)

2. **Enter AD Settings**  
    * Active Directory Domain: *netid.washington.edu*
    * Computer ID: *CBE-['Asset Tag'] make sure this matches with the AD object name* 
    * Create mobile account at login: Checked
    ![Add AD Object Settings](../assets/images/ad/ad5.png)

    Under *Administrative*
    * Check *Allow administration by:* and remove the enterprise and domain admin entries, add *uw_be_computing*
    * click *Bind*
    ![Allow Administration By](../assets/images/ad/ad6.png)
    * Authenticate with *a_cbeit* account to bind
    ![Allow Administration By](../assets/images/ad/ad7.png)

---

