---
layout: page
title: Organizational Structure
description: >-
    Overview of naming conventions and organizational standards within Jamf.
nav_order: 3
---

# Organizational Structure
{:.no_toc}

---

## Overview

The Jamf instance is organized to provide clarity, consistency, and ease of search across all configurations, policies, and scripts. This organizational structure ensures that each department and function can easily locate, manage, and deploy the resources they need while following a standardized format.

---

## Naming Conventions

The Jamf instance employs naming conventions across all resource types—policies, configuration profiles, and scripts. Each convention serves as an indicator of the resource's function, scope, or department to maintain consistency and streamline management.

---

### Policies

Policies are organized using a **layered naming convention** with a hierarchical structure. Each policy name includes a **ROOT category** that represents the top-level purpose, followed by department-specific subcategories.

- **ROOT Category**: The "root" or basic configurations for a device.
- **Department-Specific Category**: Specific identifiers for departments such as ARCH, LARCH, or RE.

#### Examples
- `ROOT: Enable FileVault`
- `ARCH: Adobe Creative Cloud Installation`

This layered approach helps administrators filter policies by both general function and departmental relevance, making it easier to locate and manage policies that apply to specific groups within the organization.

```
            ==========================================================
                            JAMF ORGANIZATIONAL STRUCTURE
            ==========================================================

                             ┌──────────────────────┐
                             │        ROOT          │
                             │    (Top Category)    │
                             └──────────────────────┘
                                        │
                    ┌───────────────────┼───────────────────┐
                    │                   │                   │
                    │                   │                   │
            ┌───────▼───────┐   ┌───────▼───────┐   ┌───────▼───────┐
            │ ARCH: Policy  │   │ LARCH: Policy │   │ RE: Policy    │
            │    Item       │   │    Item       │   │    Item       │
            └───────────────┘   └───────────────┘   └───────────────┘

```

---

### Configuration Profiles

Similar to policies, configuration profiles follow a **layered naming convention**. The names begin with a **ROOT category** or **Departmental category** that identifies the configuration’s primary purpose, followed by the specific configuration profile setting group.

- **ROOT Category**: The "root" or basic configurations for a device.
- **Department-Specific Category**: The relevant department or organizational group (e.g., ARCH, LARCH, RE).
- **Configuration Profile Setting Group**: The setting group associated with the configuration profiles.

#### Examples
- `ROOT: Restrictions`
- `ARCH: Privacy Preference Policy Control`

Using this approach keeps configuration profiles organized by their function and department, helping administrators quickly locate profiles based on their intended audience and purpose.

---

### Scripts

Scripts are named based on their **purpose** to facilitate easy searching and identification. Each script name is prefixed with a specific keyword that identifies its function, such as “Initialize” or “Settings.” 

- **Prefix**: A keyword that describes the script’s purpose (e.g., Initialize, Install, Settings, Update, Configure).
- **Description**: A concise description of the script’s task (e.g., “Install Rosetta” or “Finder Settings”).

#### Examples
- `Initialize: Install Rosetta`
- `Settings: Finder`
- `Update: Software Inventory`

This convention allows administrators to quickly find scripts based on their purpose, which streamlines searches and supports efficient script management.

---

## Best Practices for Naming and Organization

1. **Use Consistent Categories**: Ensure all new policies, profiles, and scripts use the established ROOT categories and department-specific identifiers.
2. **Prioritize Clarity**: Choose descriptive names that convey the purpose of the item at a glance.
3. **Document Naming Conventions**: Maintain a document of naming conventions and guidelines to ensure all administrators follow the same standards.
4. **Regular Review and Cleanup**: Periodically review and update names to prevent outdated or inconsistent items from accumulating in the Jamf instance.

---

Following these organizational standards helps maintain a clear and manageable Jamf instance, enabling quick access to necessary resources while reducing confusion. This structure also makes it easier to onboard new administrators, as it provides an intuitive and logical layout across all configurations.
