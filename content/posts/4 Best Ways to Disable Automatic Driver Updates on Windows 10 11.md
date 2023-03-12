---
title: "You won't believe how simple it is to stop automatic driver updates on Windows 10 and 11 - try these 4 expert-approved methods now!"
ShowToc: true 
date: "2023-04-10"
author: "Christina Thomas"
---
*****
# You Won't Believe How Simple it is to Stop Automatic Driver Updates on Windows 10 and 11 - Try These 4 Expert-Approved Methods Now!

Windows 10 and 11 automatically update drivers to ensure that your computer runs smoothly with the latest hardware changes. While this might sound like a great feature, it can cause problems if the update installs a faulty driver or if you prefer a different version of the driver. Fortunately, Windows 10 and 11 allows you to stop automatic driver updates with just a few clicks. Here are expert-approved methods to try.

## Method 1: Using the Group Policy Editor

The Group Policy Editor is a tool that allows you to configure various Windows settings. Follow the steps below to disable automatic driver updates using the Group Policy Editor:

1. Press the Windows key + R on your keyboard to open the Run command.

2. Type "gpedit.msc" and press Enter. This will open the Group Policy Editor.

3. On the left-hand pane of the editor window, navigate to Computer Configuration > Administrative Templates > System > Device Installation > Device Installation Restrictions.

4. On the right-hand pane, double-click the "Prevent installation of devices that match any of these device IDs" policy.

5. Enable the policy and click the Show button.

6. Using the Show Contents dialog box, add the Device ID of the device you want to restrict from automatic updates. You can find the Device ID by right-clicking the device in Device Manager, selecting Properties, and then clicking the Details tab.

## Method 2: Using the Registry Editor

The Registry Editor is another tool you can use to stop automatic driver updates. Here's how to do it:

1. Press the Windows key + R on your keyboard to open the Run command.

2. Type "regedit" and press Enter. This will open the Registry Editor.

3. Navigate to Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\DeviceInstall\Restrictions.

4. Right-click the Restrictions folder and select New > DWORD (32-bit) Value.

5. Name the new value "DenyDeviceIDs".

6. Double-click DenyDeviceIDs and enter the Device ID of the device you want to restrict.

## Method 3: Using Device Manager

You can also stop automatic driver updates using Device Manager. Here's how:

1. Press the Windows key + X on your keyboard and select Device Manager.

2. Right-click the device you want to restrict from updates and select Properties.

3. Click the Driver tab, then click the Update Driver button.

4. Select "Browse my computer for driver software".

5. Select "Let me pick from a list of available drivers on my computer".

6. Select the driver version you want to use and click Next.

## Method 4: Using Group Policy

The Group Policy method only works on Windows 10 Pro, Enterprise, and Education editions.

1. Press the Windows key + R on your keyboard to open the Run command.

2. Type "gpedit.msc" and press Enter. This will open the Group Policy Editor.

3. Navigate to Computer Configuration > Administrative Templates > Windows Components > Windows Update.

4. Locate the policy "Do not include drivers with Windows Updates" and double-click it.

5. Select "Enabled" and click OK.

These four methods are the easiest ways to stop automatic driver updates on Windows 10 and 11. Try them out and enjoy more control over your computer's hardware updates.

{{< youtube 4T6aOHC_A7U >}} 



## What Are Drivers


Before we get started, it’s important to understand what drivers are.
The hardware (physical components) present in your system requires specialized software to run, operate, and perform all its functions optimally. This specialized software is essentially the ‘driver’ for that specific hardware. Microsoft defines drivers as a ‘software component that lets the operating system and a device communicate with each other. 
An example can be when you connect a hardware device like a keyboard. Windows OS will now look for drivers so it can communicate with the keyboard so you can use it to type on your computer.

 
### Different Hardware Component Require Different Drivers


Drivers are built specifically for different hardware with different functions and are developed by the device manufacturer. You can find all the drivers installed on your computer listed under Device Manager. There are many including device drivers for biometric devices, display adapters, keyboards and mice, system firmware, networking drivers, etc.

 
## Why You May Need to Disable Automatic Driver Updates


Before you disable or enable automatic driver updates on your computer, understand the pros and cons so you can make an informed decision.
Pros:

 
 Your system will potentially be more stable. Pre-existing drivers for the various hardware of your system are tested by the manufacturer to be working 100%. Lesser issues to deal with as a system admin or IT administrator. While managing multiple PCs of big teams, disabling automatic driver updates prevents random issues from occurring in the future, thereby saving time. Gives a user the ability to cherry-pick the drivers used on their system, and update them as they wish from the manufacturer of that hardware.  


Cons:

 
 Disabling automatic driver updates will leave your system out of date. If your drivers are from the current ongoing year, it’s acceptable.  Requires effort from the system’s user end for maintaining drivers.  Until a driver is installed, certain hardware won’t function. Many laptops and PCs ship with drivers for various hardware devices which install them automatically. Others need to be installed manually. 
 
## How to disable Automatic Driver Updates on Windows 10/11


There are quite a few ways to disable automatic updates of drivers on Windows 10 and 11. We will discuss four ways with you and that’s all you need to know.

 
### 1. Disable During GPU Driver Installation


This method is for users who are looking to do a clean installation of their graphics card driver, without Windows interrupting the process.
Often, users of AMD Radeon/NVIDIA GeForce/Intel Arc graphics drivers end up running into an issue where Windows forcefully installs a different device driver for the GPU’s various components that include display drivers, HDMI Audio drivers, or the control panel software. 
This actually happens in the middle of an ongoing driver installation or sometimes right after it completes. Hence, we need to make sure we select the right installation settings while installing the graphics card driver.
1. Find and download the correct driver for your graphics card. Once you have the file, open it but do not continue with the installation of the setup file completely.
Note: Need help with finding what graphics card you have? Do read our detailed step-by-step guide on how to find what graphics you have, and download and install the correct GPU driver for it.
2. You will find the custom installation options at different points depending on the manufacturer while installing the driver. For NVIDIA, click on the tickmark for Perform a clean installation. After you’re done, click on the Next button. This will start the driver installation process.
6. For the AMD Radeon driver setup, check the Factory Reset option.
7. For the Intel Graphics Driver setup, check the Execute a clean installation option.
Also Read: 2 Ways to Set Default Graphics Card on Windows 11

 
### 2. Disable Search for Automatic Driver Updates in Advanced System Settings


1. Click the Windows button, and start typing Advanced System Settings. Then select View advanced system settings.
2. In the Advanced System Settings window, click on the Hardware tab. From there, click on Device Installation Settings. Then, finally, select No (your device might not work as expected) option. After this, click on Save Changes.
After doing this, Windows Update will not download drivers for many of your system components. However, if a driver is missing and its files come with the system by default, as default drivers for its devices, it is going to install that driver. You can still install your own drivers through the Device Manager.

 
### 3. Edit Windows Update Settings From Registry Editor


1. Press the Windows button, and then type regedit in the search options and select Registry Editor to open it.
2. Once the registry editor opens, Navigate to the folder structure below.
Find the key that says ExcludeWUDriversInQualityUpdate. Right-click on this key, and then click Modify.
3. On the modification screen, set the Value data to 1. Then select Hexadecimal for the base, and then click on OK to save changes.
You have now successfully set the registry setting in place that will disable Windows automatic driver updates with Windows Update. 

 
### 4. Disable Automatic Driver Updates From Group Policy Editor (Windows 10/11 Pro Users Only)


For this method, it’s important to note that it is only available for Windows 10/11 Pro edition users. The steps cannot be followed on the Home edition of Windows, as it does not feature the Group Policy Editor. You may use other methods if you don’t have Windows 10/11 Pro edition, but if you do, using Group Policy Editor is a reliable method for disabling automatic driver updates.
1. Press the Windows button and type Edit Group Policy in the search menu and open it to launch GPE.
2. Navigate to the folder structure below using the left sidebar.
3. Under the final subfolder, you will now find a few settings in the right window pane. You have to right-click on Do not include drivers with Windows Updates file and select Edit button.
4. Finally, you will be looking at the group policy for automatic driver updates on Windows. Make sure you select Enabled here to set this policy in active state. After doing this, click on OK to save changes, and then exit the Group Policy Editor.

 
## Who’s in the Driving Seat


We have now successfully disabled automatic GPU driver updates on Windows 10/11. We hope that this helped you in fixing the issue. Meanwhile, if you want to boost your CPU performance, we would recommend you read our guide on ways to maximize CPU performance on Windows 11.




