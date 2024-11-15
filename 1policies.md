---
layout: page
title: 1. Policies
description: >-
    Detailing the initial setup procedures for a device
parent: Configurations
---

# Policies
{:.no_toc}

1. TOC
{:toc}

---

## What are Policies

In Jamf Pro, policies are customizable workflows that automate and enforce actions on managed devices. Policies can be used to install software, run scripts, enforce security settings, and manage device configurations remotely. By defining policies, administrators can ensure that devices meet organizational standards and comply with security requirements.

Key benefits of using Jamf Pro policies include:

- Automated software deployment and update management
- Remote enforcement of security settings and compliance checks
- Simplified configuration management for devices
- Improved control over device behaviors and functionality

---

## Steps for Creating a Policy in Jamf Pro

Follow these steps to create and apply a policy in Jamf Pro:

1. **Log in to Jamf Pro and Navigate to Policies**  
   Go to *Computers > Policies* in the Jamf Pro dashboard. Here, you can create new policies or manage existing ones.

    ![Policies Page](../assets/images/policies/policy1.png)

2. **Create a New Policy**  
   Click **New** to create a policy. Enter a descriptive name for the policy, select the appropriate category, and configure the policy’s scope to specify which devices it will apply to.

    ![Create New Policies Page](../assets/images/policies/policy2.png)

3. **Define the Policy Trigger and Frequency**  
   Specify when the policy will execute (e.g., at login, at startup, or on a recurring schedule). Choose the frequency based on the need, such as once per user, daily, or ongoing.

    ![Create Policy Trigger](../assets/images/policies/policy3.png)

4. **Add Policy Payloads**  
   In the policy configuration, select the payloads you want to include (e.g., *Files and Processes*, *Scripts*, or *Packages*). Each payload represents an action or setting that will be applied to the device.

    ![Create Policy Payloads](../assets/images/policies/policy4.png)   

5. **Configure Scope and Apply Policy**  
   Define the scope by selecting the devices or groups the policy should target. Once configured, save and enable the policy to activate it.

    ![Create Policy Scope](../assets/images/policies/policy5.png)  

6. **Monitor Policy Execution**  
   Check the *Policy Logs* in Jamf Pro to monitor the execution and success of the policy. Logs provide detailed feedback on the policy’s deployment status.

    ![Policy Logs](../assets/images/policies/policy6.png)  

---

## Steps for Packaging an App Using Jamf Composer

To deploy custom applications or software via Jamf Pro, you can package the app using Jamf Composer. Read more on composer [here](https://www.jamf.com/products/jamf-composer/). Follow these steps to create a deployable package:

1. **Open Jamf Composer and Create a New Package**  
   Launch Jamf Composer and select **New Package**. Choose whether to create a package from scratch or from a pre-installed application on your computer.

    ![Composer](../assets/images/policies/policy7.png)  

2. **Drag and Drop the App or Files into Composer**  
   If you have the app ready, drag and drop the app’s .app file or installation files into Composer. Composer will automatically detect files and dependencies needed for the application.

    ![Composer with File](../assets/images/policies/policy8.png)  

3. **Organize Files in the Desired Installation Path**  
   Arrange the files in Composer to match the correct directory structure on the target devices (e.g., placing the app in the *Applications* folder or other system folders). Make sure that permissions for all directories are set to *root* and *wheel*.

    ![Composer Permissions](../assets/images/policies/policy9.png)

4. **Add Scripts or Pre/Post-Installation Actions (Optional)**  
   If needed, add custom scripts to run before or after the installation (e.g., to configure settings or clear cache). This can be done by selecting the **Scripts** tab in Composer.

5. **Build the Package**  
   Once everything is set up, click **Build as PKG** to create a .pkg file. Name and save the package in a location where you can easily access it for upload to Jamf Pro.

   ![Composer Build Package](../assets/images/policies/policy10.png)

6. **Upload the Package to Jamf Pro**  
   In Jamf Pro, navigate to *Settings > Packages* and upload the newly created package. After uploading, the package can be used in a Jamf policy to deploy the app to targeted devices.
    ![Composer Build Package](../assets/images/policies/policy11.png)

---

By following these steps, you can effectively create and apply policies within Jamf Pro and package applications using Composer.
