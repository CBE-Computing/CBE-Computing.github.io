---
layout: page
title: Commands
description: >-
    Detailing the common Jamf CLI Commands
---

# Jamf Commands
{:.no_toc}

<!-- ## Table of contents
{: .no_toc .text-delta } -->

<!-- 1. TOC
{:toc} -->

---

## Common Jamf CLI Commands

```bash
    # Uninstall the JAMF agent
    sudo jamf –removeFramework

    # Jamf help; gets you more commands for your use
    jamf help

    # Force a full inventory from the client
    sudo jamf recon

    # Forces a check in from the client
    sudo jamf policy

    # Check for enrollment and Jamf version on local Mac
    jamf about

    # Services/Running processes
    sudo launchctl list
    top –o cpu
    top –o rsize

    # Show computer level profiles
    sudo profiles -Cv
```

## Other Commands

   {: .note }
   >**This below can also be found by running 'jamf help' in your CLI**

```md
    Usage: jamf verb [options]

	verb is one of the following:

	about			 Displays information about the jamf binary
	bind			 Binds this computer to a directory service
	bless			 Blesses a System or a NetBoot Server
	changePassword		 Changes a local user's password
	checkJSSConnection	 Checks the availability of the JSS
	createAccount		 Creates a new local account on the system
	createConf		 Creates a configuration file that the jamf binary uses to find the JSS
	createSetupDone		 Ensures the Setup Assistant does not launch immediately on the next boot
	createStartupItem	 Creates a startup script to contact the JSS
	deleteAccount		 Deletes a local account from NetInfo or the local dscl database
	deletePrinter		 Deletes a printer from the system
	deleteSetupDone		 Causes the Setup Assistant to launch on the next boot
	displayMessage		 Displays a message to the current user
	enablePermissions	 Enables permissions on a volume
	enroll			 Enrolls this computer with the JSS
	fixByHostFiles		 Fixes the ByHost files
	fixDocks		 Repairs docks that have question marks after certain OS Updates
	flushCaches		 Flush cache files for the system and/or users
	flushPolicyHistory	 Flush the policy history on the JSS
	getARDFields		 Displays the ARD Fields on a volume
	getComputerName		 Displays the computer name on a volume
	help			 Displays this message or details on a specific verb
	launchSelfService	 Opens the Self Service app
	listUsers		 Lists all the users on the computer
	log			 Log the IP address, action, and username to the JSS
	manage			 Enforces the entire management framework from the JSS
	mapPrinter		 Maps a printer
	modifyDock		 Installs or removes items in all users docks
	mount			 Mounts a file share
	policy			 Checks for policies on the JSS
	reboot			 Reboots the computer
	recon			 Runs Recon to update the inventory in the JSS
	removeFramework		 Removes the JAMF Binary and associated files from the computer
	removeSWUSettings	 Remove settings that point SWU at internal servers
	renewDeviceCert		 Renews the existing management framework device certificate
	resetPassword		 Resets a local user account password (Warning: User keychain and FileVault 2 passwords may be affected. Use changePassword when current password is known)
	runSoftwareUpdate	 Run Software Update
	setARDFields		 Sets the ARD Fields
	setComputerName		 Sets the computer name
	setHomePage		 Sets the default home page for users
	setOFP			 Sets the Open Firmware mode and password
	startSSH		 Starts the ssh server
	startup			 Checks the connection to the Jamf Pro server and triggers startup actions as defined in Jamf Pro > Settings > Computer Management > Check-In > Startup Script.
	uninstall		 Uninstalls a package
	unmountServer		 Unmounts a file server
	updatePrebindings	 Updates the prebindings on a volume
	version			 Prints the version of this application



	Global Flags:

	-displayJSSTraffic 	 Displays the total network traffic between the jamf binary and the JSS
	-randomDelaySeconds 	 Delays a random amount of time before starting
				 Specify the maximum number of seconds as the next parameter
	-showPID 		 Prints the PID of the process
	-stopConsoleLogs 	 Stops logs from being sent to the console
	-verbose 		 Shows verbose events



	jamf help <verb> will provide details on that verb

```