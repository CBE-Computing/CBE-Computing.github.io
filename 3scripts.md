---
layout: page
title: 3. Scripts
description: >-
    How to create, manage, and deploy scripts in Jamf.
parent: Configurations
---

# Scripts
{:.no_toc}

1. TOC
{:toc}

---

## What are Scripts

Scripts in Jamf Pro allow administrators to automate tasks and customize configurations on managed devices. Scripts can be written in various scripting languages, including Bash, Python, and AppleScript, and can be deployed to devices for tasks like software installation, system maintenance, and custom configuration.

Scripts help administrators:
- Automate repetitive tasks, saving time
- Apply consistent settings across devices
- Address specific needs that aren’t covered by standard policies or configuration profiles

---

## Steps for Creating and Deploying a Script in Jamf Pro

1. **Create or Obtain the Script**
   - Write a new script or obtain an existing one that fulfills your needs. Ensure it’s compatible with the target devices’ OS and follows best practices for security and performance.

2. **Log in to Jamf Pro and Navigate to Scripts**
   - Go to *Settings > Scripts*.

3. **Upload the Script**
   - Click **New** and name the script for easy identification. Then, either paste the script code or upload a file containing the script.

    ![Scripts Settings](../assets/images/script/script1.png)
    ![Scripts Paste](../assets/images/script/script2.png)

4. **Configure Script Parameters**
   - If the script requires parameters, set these in the “Parameters” section. Jamf allows up to 11 customizable parameters for scripts.

    ![Scripts Params](../assets/images/script/script3.png)

5. **Assign the Script to a Policy**
   - To deploy the script, assign it to a policy. Go to *Computers > Policies*, create a new policy or edit an existing one, and add the script under the *Scripts* payload.
   ![Scripts Policy](../assets/images/script/script4.png)

6. **Define Scope for the Policy**
   - Specify which devices or groups should receive the script by setting the policy’s scope. This can be by device type, department, location, or custom criteria.

7. **Test and Monitor Script Deployment**
   - Before deploying widely, test the script on a single device to ensure it works as expected. After deployment, use Jamf’s logging tools to monitor the results and confirm successful execution.

---

## Best Practices for Using Scripts in Jamf

- **Test Thoroughly**: Always test scripts on a small group of devices before deploying to larger groups.
- **Use Comments and Documentation**: Document each script’s function and usage for future reference.
- **Maintain Version Control**: Keep scripts updated and stored in a version-controlled environment like Git.
- **Leverage Parameters**: Use parameters to make scripts more flexible and reusable for different use cases.
