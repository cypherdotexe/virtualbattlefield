# CIS 141 Technical Blog
## Christian Bruce Young
### christianbruceyoung@gmail.com

###**Biography**

IT and Cybersecurity student at Sierra College. I watch movies, and play Nintendo. I have no professional IT experience, but am proficient in Microsoft and Adobe products. In May 2018, I built my first computer. These are its specifications:

-Intel i7-8700K CPU
-Corsair H100i v2 liquid CPU cooler
-ASUS ROG STRIX Z370-E motherboard
-Gigabyte GeForce GTX 1060 6GB Windforce OC video card
-Corsair Vengeance RGB 16GB DDR4-3000 memory
-Corsair 3x LL120 and 2x LL140 RGB fans
-Samsung 860 EVO 256gb SSD
-Seagate FireCuda 3TB 3.5" 7200RPB HDD


This will serve somewhat as a digital portfolio for my experiences in CIS 141 - Client Operating System Installation and Configuration.

#### Skill 1.1 - Prepare for Installation Requirements

Warm-up: How many computers are in this room? Explain your answer.

There are 36 computers in this room because I counted the computers in each row, 4 each row, multiplied it by 8, totaling 32 student computers. Add it with one student laptop, one teacher's laptop, and two teacher's computers in the very front behind the desk, that would be 36 computers.

Notes:

Deployment Options
 Wipe & Load / Clean Install
  1. Capture data /settings
  2. Deploy (custom) OS image
  3. Inject Drivers
  4. Install Apps
  5. Restore Data /Settings
Usage: Viable for all scenarios

In-Place Upgrade
  1. Preserve data, settings
  2. Install (standard) OS image
  3. Restore everything
Usage: Recommended for existing Windows 7/8/8.1 devices

Provisioning
 Transform into an enterprise device:
  -Remove unneeded components / Harden
  -Add organizational apps
  -Add organizational configuration
Usage: For Windows 10 CYOD scenarios


Prompt: At school, work or home, find a PC that has not yet been upgraded to Windows 10 (or role play with one that is upgraded to Windows 10).

1. Who is the primary user of the PC?
2. What are the technical specifications of that machine, as compared to the Windows 10 minimum requirements?
3. How would you go about upgrading this machine?  Why did you choose this approach?  Did you use any Microsoft tools to help determine your upgrade?  If so, which tools?
4. What version of Windows 10 would you install?  Why?


I have an old Toshiba laptop that runs on Windows 8.1. Specifically, it was a Satellite series, model S55-A5167.

1. I am the primary user of the laptop.

2. The technical specifications, compared to the minimum requirements for Windows 10 are:

Toshiba S55-A5167
Processor: 2.4GHz i7-4700MQ (6M Cache, up to 3.40GHz)
RAM: 8GB DDR3L 1600MHz RAM
Storage: 1TB (5400 RPM) Serial ATA hard disk drive
Graphics card: Mobile Intel HM86 Express Chipset, NVIDIA GeForce GT 740M with 2GB of DDR3 discrete graphics memory w/ Optimus
Display: 1366x768

Windows 10 minimum requirements
Processor: 1GHz or faster or SoC
RAM: 1GB for 32-bit or 2GB for 64-bit
Storage: 16GB for 32-bit OS, 20GB for 64-bit OS
Graphics card: DirectX 9 or later with WDDM 1.0 driver
Display: 800x600

3. To upgrade an old laptop like this, I will have to install Windows 10 using the in-place upgrading method. This method is ideal for daily-use laptops such as this one, because it's not a recommended computer for business use, and it has a dozen of personal files on it. Although it meets the minimum requirements to install Windows 10, being a four-year-old laptop, it might run slowly. I did not have to use any Microsoft software to determine my upgrade.

4. I would have to install Windows 10 Home because the age of the laptop would not make it suitable for professional or other editions.




#### Skill 1.2 - Install Windows 10


#### 1.3 Sept 10 Warmup Activity

Warmup: Windows 7 was the world's most used Windows OS, but updates for Windows 10 last August have started to decrease the number of computers running Windows 7. Microsoft has been pushing for more users to upgrade to Windows 10, and users are reluctant because they view Windows 7 (and previously Windows XP) as the most stable OS. Microsoft has announced that they will end Windows 7 support in 2020, and those who continue to use it must pay for security updates through 2023. Although this is aimed towards businesses, the number of Windows 7 users in the world outnumber Windows 10 users, and Windows 7 users are concerned that they will have to upgrade to 10.

#### 1.2 Technical Blog Prompt: Answer the following questions and, when applicable, be sure to include screenshots and links to the Internet:


 1. Why would a user be interested in multiple partitions on a hard drive?  Use a Windows tool (GUI or CLI) to create a partition and describe the steps that you took to create multiple partitions.

A user would want multiple partitions on a hard drive because they want to be able to alternate between different operating systems, ex. Windows and Linux back to back. But partitioning can also make organizing your data much easier.

Using Disk Management, what I did to make a partition on my hard disk drive was right-clicking it and selecting Shrink Volume. From there I choose the amount of space (in megabytes) to shrink for the new partition. After shrinking, I repeated this step one more time.


 2. Describe each step that requires "user attention" during the clean installation of Windows 10.

-1: Select the language, time and currency format, and keyboard layout.
-2: Enter the activation key or select "I don't have a product key" at the bottom of the window.
-3: Agree to the license terms.
-4: Choose "Custom" installation.
-5: Choose the drive to install Windows on.
-6: Connect to a wired or wireless connection.
-7: Choose to use Express settings or customized settings.
-8: Sign in with a Microsoft account or skip the step.
-9: Create an account for the computer.

 3. What is one Windows Feature that you chose to add after installation?  How did you add that feature?

I added Windows Hypervisor Platform after installation by going to the Control Panel, clicking on Programs, then Programs and Features, and selecting "Turn Windows features on or off." I looked through the directory of features and gave a checkmark to the Windows Hypervisor Platform folder. The window told me to restart to apply the change.




#### Sept. 17 Warmup

"What is 'Patch Tuesday'? When did it last occur? What was included in the most recent?

"Patch Tuesday" is an unofficial term used to refer to when Microsoft frequently releases security patches for its software. It last occured on September 11. This month's patch covers 61 vulnerabilities in Microsoft software, 17 of which were rated Critical.

#### Skill 1.2 Technical Blog - Windows 8.1 Upgrade

1. On Windows 8.1, install an application that may not be Windows 10 compatible. Why do you think this application may not be compatible?

I have installed VLC for Windows 8.1, and I suspect it might not be compatible on 10 because it is a previous version.

2. Create a very special text file that you would like to be included in the upgrade.  What is in the file?  Where is it located?

The file contains a line from an old sitcom that I found funny. It is located on the desktop. (C:\Users\cyoung13\Desktop)

3. Describe each step that requires "user attention" during the in-place upgrade of Windows 10.

1-The setup window first asks you to download updates for 8.1 before upgrading. You can choose to do so or not.
2-It then asks you to accept the software license agreement.
3-When the window tells you it is ready to install, you have the option to change what files that you want to keep in the 10 upgrade.

4. In what ways was the upgrade process similar to the clean install process?  How did it differ?

Both processes require users' complete and undivided attention when choosing the right options to install and upgrade. The upgrading process allows users to choose what files to transfer over to Windows 10.

5. Are there any additional folders that remain after the upgrade process is complete?  What are the contents of those folders?

After the upgrade process is complete, a new folder with data from Windows 8.1 remains, called Windows.old, which can allow the user to roll back to 8.1 if they encounter any problems with 10.


#### Skill 1.3 - Configure Devices and Device Drivers

#### Skill 1.3 Technical Blog Prompt

1. Create a list of hardware that a user might have that require a driver installation.
  -Motherboards
  -Microphones or headsets
  -Printers
  -Sound cards
  -External storage (USB drives, hard drives)

2. Locate a device from your list (for example, printer or external storage) and install it on Windows 10 (VM in class, machine at home, maybe the host machine in class?)
  -I have installed a microphone on my computer.

3. Locate the version of the driver and see if it is the most current version available (in the case of the printer, check the manufacturer website).
 - If necessary update the device.

 -Its last installed update was on April 11, 2018. It is current.

4. Disable the device.  Does this affect Windows performance?  What happens when you disable other devices?  Try disabling your network card - how was that experience?

-Disabling the microphone does not affect Windows performance on my computer. Disabling my network card prevents Internet access until it is enabled again.

5. Why would I disable updates over metered connections?  Capture a screenshot of the screen on which you disabled this feature.

Downloading Windows updates over metered connections would limit the computer's data usage and stop it from automatically updating. But it will also prevent other applications from updating, and they might operate differently. https://i.imgur.com/qlmmpED.png

6. Perform a "rollback" of a driver update.  Note, you will need to access a different USB device if you have been working with a printer.

 -I performed a rollback on my printer, but it performs the same.

7. After installing a USB microphone, a system has extremely poor performance.  How would you check to see if the performance issues are related to the USB microphone?

 -I go to Device Manager and disable the microphone to see if the computer performs better. It might need a driver update.


#### Sept. 24, 2018

Warmup: Take a few minutes to read the article posted in Canvas. What do you think is the future of operating systems? Feel free to add additional research to your response.

Answer: Microsoft announced Windows Virtual Desktop, where Windows 10 can be used on the Azure cloud computing platform. I believe that operating systems are headed in a direction where not only can they be bought at a fixed price, users can rent a monthly or annual subscription for them, much like SaaS products e.g. Adobe.




#### Skill 1.4 Technical Blog Prompt

- Using your textbook, ITPro.tv videos and notes, as well as Microsoft documentation, research one of the following post-installation activities, create a step-by-step guide, and test out your guide on your VM.

* Configuring Hyper-V
1. You go into Windows Features
2. Select and Enable Hyper-V
3. Reboot the machine to apply change
4. Search "Hyper-V Manager" and select application



#### Oct. 1, 2018

Warmup: What is "UAC"? Why is it important? When did Microsoft introduce UAC? Is UAC on your Sierra host machine different than your VM? If so, how so?

Answer: UAC is short for User Account Control, a security control introduced in Windows Vista. UAC is designed to prevent the computer from running software from making unauthorized changes to the operating system's settings before asking for the user's permission. The UAC on my Sierra host machine is nearly identical to the one on my VM.


#### Skill 1.5 - Enterprise Implementations Notes

LSDO - Local, Site, Domain, Organizational units - order of operations for user privileges in an enterprise environment

Group Policy
 * Let's play around with Local Group Policy Editor
  * Centralized control for...
    -User Settings
    -Computer Settings
    -Control and Deployment of Applications
    -Control User Experience

  What does it change?
   - It changes the system registry.
   - gpupdate /force or logoff to apply changes.

GPEdit Challenge
   - Can you block Microsoft Accounts?
    Yes.

    Computer Configuration > Windows Settings > Local Policy > User Rights Assignment

   - Enforce a password length of 10 characters?
    Yes.

    Computer Configuration > Windows Settings > Security Settings > Account Policies > Password Policy

   - Disable secure desktop in UAC? (NOT recommended)
    Yes. *But it is NOT recommended to do so!*

    Computer Configuration > Windows Settings > Local Policies > Security Options > "User Account Control: Switch to the secure desktop when prompting for elevation"

#### Oct. 8, 2018

Prompt: What is a "software bug" Describe the "bug" that is delaying the release of the 1809 update for Windows 10.

A software bug is a flaw in software that causes the computer to behave in an unintended manner. The particular "bug" in the 1809 update is deleting documents and photos on the user's computer.


-Create a "Provisioning Package"
-Review Skill 2.1 Key Concepts
-Complete Skill 2.1 Technical Blog Prompt & Professionalism 7&8

C:\Users  \Documents \ Windows Imaging & Configuration Designer

local administrator account and pass for provision
cyoung13 77778

#### Skill 2.1 Technical Blog Prompt

Prompt: Create a Top 5 list of Windows 10 networking best practices, tips, tricks, and troubleshooting strategies.

1. Configuring VPN connections.
2. Use Event Viewer to collect information about system activity and IP conflicts.
3. Using Windows Firewall with advanced security rules.
4. Using IPConfig via a command-line interface to diagnose networking issues.
5. Connect to a HomeGroup.


#### Oct. 15, 2018

What is BitLocker?

A: BitLocker is a security feature that encrypts hard drives and prevent them from theft when the OS is not running. It was introduced on Windows Vista.

How is it configured?

A: BitLocker is configured by plugging in your USB or external hard drive, right click on them in Windows Explorer, then click on "Turn on BitLocker...", then choose how you want to unlock the drive in the event of an offline attack, using a password to unlock it.

I have a USB drive that is configured with BitLocker. Will it work on all Windows 10 machines?

A: BitLocker will only work on Windows 10 Pro and Windows 10 Enterprise.

How about a Macbook or a Chromebook?

A: They cannot work on Macbooks, but they are pre-enabled on Surface Pro 3 tablets.

#### Review Skill 2.2 Key Concepts

#### Skill 2.2 Technical Blog Prompt

Scenario 1: Creating a Large Volume

You have a new desktop running Windows 10. However, you try to copy your file repository and find out that you do not have enough disk space. You have 400 GB of free disk space on your C drive and you have 3 smaller 500 GB drives. What can you do?

Answer: You can create a spanned volume across one of the smaller 500 GB drives so that the drive running Windows 10 can allow you to copy your file repository.

Scenario 2: Configuring a Storage Space/Storage Pool.

You create a new storage pool for the following disks on your Windows 10 computer:

Serial ATA (SATA): 1 TB
Serial Attached SCSI (SAS): 1 TB

SATA and SAS are two different types of drives with different connectors/interfaces.

What is the maximum size you can allocate for your new storage space?

Answer: You can allocate a maximum of 2 TB for this storage space.



#### Oct. 29, 2018

Browse the Windows Store. What app did you find that surprised you? Is there an essential app
to your life missing that from the store? What is it and where can one find it?

Answer: I found a video player called VLC, which surprised me because being a free application,
I thought it was an open source program you couldn't get on the Microsoft Store.

One essential application to me is foobar2000, an audio player that is also free. What's special about it
is that music lovers like myself can look at the spectograms of any of my songs and see how their sounds
are visualized. It can be downloaded at www.foobar2000.org


#### Notes

The home stretch

Technical Blog Sheckpoints
Professoinalism weeks
2x mcsa practice quizzes
change managment whitepaper (ch.2)
break windows 10 image challenge (ch.3)

Night of Case Studies


#### Skill 2.4 Technical Prompt

You work for a small business of 25 employees, split between two offices that
are in different buildings but share a parking lot.

1. You have been tasked with designing a file sharing solution that is fast,
reliable, easy to use, and secure. What would you do?

A: I would set up a site-to-site VPN connection between the two buildings, or G Suite.

2. You have been tasked with deploying Microsoft Office to all
machines, Adobes CS Suite to the Marketing team, and QuickBooks to
the Accounting Team. You also want allow users to selectively install
Adobe Acrobat. What would you do?

A: I would create and distribute a provisioning package that includes Microsoft Office,
Adobe CS Suite, and QuickBooks for their respective intended users and place
the package onto the network folder.

To allow users to install Adobe Acrobat by themselves, I would use Group Policy to make
exceptions for them to do so.


cypherdotexe
44183286+cypherdotexe@users.noreply.github.com


#### Skill 2.3 Technical Prompt