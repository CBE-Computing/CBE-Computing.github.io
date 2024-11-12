---
layout: page
title: 2. Configuration Profiles
description: >-
    Detailing the initial setup procedures for a device
parent: Configurations
---

# Configuration Profiles
{:.no_toc}

1. TOC
{:toc}

---

## What are Configuration Profiles

Configuration Profiles in Jamf Pro are used to manage device settings and enforce security standards across a fleet of devices. They allow administrators to define and distribute settings for Wi-Fi, VPN, restrictions, app configurations, and more, ensuring a consistent user experience and maintaining compliance with organizational policies. 

Key benefits of using Configuration Profiles in Jamf Pro include:

- Simplified deployment of complex settings and security policies
- Centralized management of network, app, and system configurations
- Ability to restrict or enable features across managed devices
- Enhanced control over user experience and device compliance

---

## Steps for Creating a Configuration Profile in Jamf Pro

Follow these steps to create and deploy a Configuration Profile in Jamf Pro:

1. **Log in to Jamf Pro and Navigate to Configuration Profiles**  
   Go to *Computers > Configuration Profiles* in the Jamf Pro dashboard. Here, you can create new profiles or manage existing ones.
   
   ![Configuration Profiles](../assets/images/config/config1.png)

2. **Create a New Configuration Profile**  
   Click **New** to create a configuration profile. Give the profile a descriptive name and select a category to help organize it within Jamf Pro.

   ![Configuration Profiles New](../assets/images/config/config2.png)

3. **Configure Profile Settings**  
   In the profile settings, add the specific payloads required for the configuration. Examples of available payloads include:

   - **Wi-Fi**: Configure Wi-Fi network settings, SSID, and security type.
   - **VPN**: Set up VPN configurations with connection type, server address, and authentication.
   - **Restrictions**: Enable or restrict device functions like the camera, app installation, or screen capture.
   - **Security & Privacy**: Enforce password policies, file encryption, and other security-related settings.

   ![Configuration Profiles Settings](../assets/images/config/config3.png)

4. **Define Scope for the Profile**  
   Set the scope by specifying the target devices or user groups that should receive the profile. This can be based on criteria such as device type, operating system, or department.

    ![Configuration Profiles Scope](../assets/images/config/config4.png)

5. **Save and Distribute the Profile**  
   Once the profile is fully configured, save it. After saving, the profile will be deployed to the selected devices. Jamf Pro will automatically push the profile to devices within the defined scope.

6. **Monitor Profile Status and Compliance**  
   Use the *Logs* and *Device Inventory* sections in Jamf Pro to track the deployment and ensure devices comply with the profile’s settings. If necessary, you can edit or remove profiles to address any issues.

   ![Configuration Profiles Logs](../assets/images/config/config5.png)

---

By following these steps, you can easily create and apply Configuration Profiles in Jamf Pro, enabling streamlined and secure management of device settings across your organization.
