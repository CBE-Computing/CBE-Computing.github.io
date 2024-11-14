---
layout: page
title: 3. Device Enrollment
description: >-
    Detailing the initial setup procedures for a device
parent: Setup
---

# Device Enrollment
{:.no_toc}

1. TOC
{:toc}

---

## What is Jamf Device Enrollment

Jamf Device Enrollment is a streamlined method for registering Apple devices into Jamf Pro, allowing organizations to manage and secure devices from day one. By enrolling devices, IT administrators can automate configurations, enforce security policies, and deploy applications remotely. Device Enrollment simplifies the setup process, ensuring all devices meet organizational requirements before they’re handed over to users.

Key benefits of using Jamf Device Enrollment:

- Automated device configuration and security policy enforcement
- Remote app deployment and management
- Simplified ongoing maintenance and updates
- Compliance with organization-wide security standards

---

## Steps for Enrolling a Device with Jamf Pro

If you have completed steps 1 and 2 faithfully you can then continue to the steps below. To enroll a device in Jamf Pro, follow these steps to ensure it is properly configured and managed:

1. **Prepare Enrollment Settings in Jamf Pro**  
   Log in to your Jamf Pro dashboard and go to *Devices > PreStage Enrollments*. Here, you can configure the settings that will automatically apply during the enrollment process, including profiles, apps, and security policies.

2. **Assign Device to Jamf Pro via Apple School Manager (ASM)**  
   In *Apple School Manager*, navigate to *Devices > Device Assignments*. Select the devices you wish to enroll and assign them to the Jamf MDM server. This assignment ensures that devices will automatically enroll in Jamf Pro during setup. (Refer to Apple School Manager page for more detailed instructions)

3. **Turn on the Device and Begin Setup**  
   Power on the device and proceed through the initial setup screens. When connected to a network, the device will recognize its enrollment in Jamf Pro and automatically begin the configuration process.

   {: .note} 
   > **As of currently, you must enroll the computer via Ethernet and or authenticate with your NetID to the WiFi. Guest WiFi will not work for enrollment.

5. **Complete Device Setup and Verify Enrollment**  
   Once the device finishes setup, verify that it appears in the Jamf Pro dashboard. Confirm that all assigned configurations, profiles, and apps have been applied to ensure compliance with organizational standards.

---

## Steps for Manually Enrolling a Device

If a device isn’t registered in Apple School Manager, you can still manually enroll it in Jamf Pro:

1. **Log into Jamf Pro and Generate an Enrollment Link**  
   In the Jamf Pro dashboard, navigate to *Devices > Enrollment Invitations*. Generate a unique enrollment link for the device.

2. **Open the Enrollment Link on the Device**  
   On the device, open a web browser and enter the enrollment link. This link will guide the device through the enrollment steps.

3. **Install the MDM Profile**  
   Follow the on-screen prompts to download and install the Jamf MDM profile. This profile will allow Jamf Pro to manage the device.

4. **Verify Enrollment in Jamf Pro**  
   After installing the MDM profile, confirm the device’s enrollment status in Jamf Pro. Ensure that policies, configurations, and app

