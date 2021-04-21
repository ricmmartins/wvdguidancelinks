# WVD Guidance Links  
This repository contains the information needed to describe the main topics on a wvd architecture design and implementation.

## WVD Architecture Guidance

1. [**What is WVD**](https://docs.microsoft.com/en-us/azure/virtual-desktop/overview)<br/>

2. [**WVD Requirements**](https://docs.microsoft.com/en-us/azure/virtual-desktop/overview#requirements)<br/>
3. [**Supported OS images**](https://docs.microsoft.com/en-us/azure/virtual-desktop/overview#supported-virtual-machine-os-images)<br/>
4. [**Network guidelines**](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/network-guidance?context=/azure/virtual-desktop/context/context)<br/>
5. [**Windows Virtual Desktop experience estimator**](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/network-guidance?context=/azure/virtual-desktop/context/context#windows-virtual-desktop-experience-estimator)<br/>
6. **Virtual Machine Guidance:**<br/>
6.1. [Virtual machine sizing guidelines](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs?context=/azure/virtual-desktop/context/context)<br/>
6.2. [Multi-session recommendations](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs#multi-session-recommendations)<br/>
6.3. [Single-session recommendations](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs?context=/azure/virtual-desktop/context/context#single-session-recommendations)<br/>
6.4. [General virtual machine recommendations](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs?context=/azure/virtual-desktop/context/context#general-virtual-machine-recommendations)<br/>
7. [**WVD Architecture Sample**](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop#architecture)<br/>
8. **FSLogix:**<br/>
8.1. [FSLogix for enterprise](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix)<br/>
8.2. [Storage options for FSLogix profile containers](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#storage-options-for-fslogix-profile-containers)<br/>
8.3. [Azure Files Best practices](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#azure-files-best-practices)<br/>
8.4. [Azure NetApp Files Best Practices](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#azure-netapp-files-best-practices)<br/>
9. [**Best Practices for WVD**](https://docs.microsoft.com/en-us/azure/virtual-desktop/fslogix-containers-azure-files#best-practices-for-windows-virtual-desktop)<br/>


## WVD Deployment Guidance

1. [**Deploy an Azure AD Tenant**](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-create-new-tenant)<br/>

2. [**Deploy an Azure Subscription**](https://docs.microsoft.com/en-us/azure/cost-management-billing/manage/create-subscription)<br/>
3. **Deploy Azure infrastructure and AD DS:**<br/>
3.1. [Virtual Network](https://docs.microsoft.com/en-us/azure/virtual-network/quick-create-portal)<br/>
3.2. [Subnet](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-network-manage-subnet#add-a-subnet)<br/>
3.3. [NSG](https://docs.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview) (Permits AD Traffic, RDP incoming traffic, restricts DMZ access)<br/>
3.4. [DNS configured to point to the domain controller](https://docs.microsoft.com/en-us/azure/virtual-network/manage-virtual-network#change-dns-servers)<br/>
3.5. [Virtual Machine:](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/quick-create-portal)<br/>
3.5.1. Active Directory Domain Services installed and configured<br/>
3.5.2. Azure AD Connect installed and ready for configuration<br/>
4. **Configure Azure AD Connect with AD DS:**<br/>
4.1. [What is Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-azure-ad-connect)<br/>
4.2. [Azure AD connect and Azure AD Connect Health installation](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-install-roadmap)<br/>
5. [**Windows Virtual Desktop environment concepts**](https://docs.microsoft.com/en-us/azure/virtual-desktop/environment-setup)<br/>
6. [**Create Azure AD Security Groups for WVD**](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)<br/>
7. [**Assign users to Groups**](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-groups-members-azure-portal)<br/>
8. **Create a Master Image for WVD:**<br/>
8.1. [Create a Master Image for WVD](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/capture-image-resource)<br/>
8.1.2. [Install Office on a master VHD image](https://docs.microsoft.com/en-us/azure/virtual-desktop/install-office-on-wvd-master-image)<br/>
8.1.3. [Install Microsoft Teams on a WVD](https://docs.microsoft.com/en-us/azure/virtual-desktop/teams-on-wvd)<br/>
8.1.4. [Azure Academy - Teams AV Redirect](https://www.youtube.com/watch?v=RfbolIgPcBY&t=661s)<br/>
8.1.5. [Download and install FSLogix](https://docs.microsoft.com/en-us/fslogix/install-ht)<br/>
8.1.6. [OS Settings | Prepare and customize a master VHD image](https://docs.microsoft.com/en-us/azure/virtual-desktop/set-up-customize-master-image)<br/>
8.1.7. [OS Settings | Prepare a Windows VHD or VHDX to upload to Azure](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/prepare-for-upload-vhd-image)<br/>
8.1.8. [OS Settings | Run Disk Cleanup](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/cleanmgr)<br/>
9. **Image Management:**<br/>
9.1. [Azure Academy - Image Management](https://www.youtube.com/watch?v=PCWJEoG8X-I)<br/>
9.1.2. [Azure Academy - Shared Image Gallery](https://www.youtube.com/watch?v=2LxvwR9LGWQ)<br/>
9.1.3. [Image Management : How to manage and deploy custom images (including versioning) with the Azure Shared Image Gallery (SIG) (robinhobo.com)](https://www.robinhobo.com/windows-virtual-desktop-wvd-image-management-how-to-manage-and-deploy-custom-images-including-versioning-with-the-azure-shared-image-gallery-sig/)
1. **Define a strategy to store FSLogix profiles containers:**<br/>
12.1. [Storage options for FSLogix Profile containers](https://docs.microsoft.com/en-us/azure/virtual-desktop/store-fslogix-profile)<br/>
13.1.1. [Azure Files and Active Directory Domain Services](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-file-share)<br/>
13.1.2. [How to implement FSLogix Profile container using Azure Files and Active Directory authentication for Windows Virtual Desktop (WVD) (robinhobo.com)](https://www.robinhobo.com/how-to-implement-fslogix-profile-container-using-azure-files-and-active-directory-authentication-for-windows-virtual-desktop-wvd/)
15.1.2. [Azure NetApp Files](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-fslogix-profile-container)<br/>
16.1.3. [Windows File Server](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-host-pools-user-profile)<br/>
17.1.4. [Azure Files and Azure Active Directory Domain Services](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-profile-container-adds)<br/>
18. **FSLogix General Configuration:**<br/>
19.1. [Use FSLogix Group Policy Template Files](https://docs.microsoft.com/en-us/fslogix/use-group-policy-templates-ht)<br/>
20.2. [Profile Container registry configuration reference](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference)<br/>
21.3. [Antivirus exclusions](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#antivirus-exclusions)<br/>
22.4. **FSLogix Reference Links:**<br/>
23.4.1. [Azure Academy - FSLogix with Azure Fileshare](https://www.youtube.com/watch?v=9S5A1IJqfOQ&t=647s)<br/>
24.4.2. [Azure Academy - NetApp](https://www.youtube.com/watch?v=bswIbTB62mY)<br/>
25.5. **GPO Recommendations:**<br/>
26.5.1. [Enabled *** - Mandatory](https://docs.microsoft.com/en-us/fslogix/configure-profile-container-tutorial#configure-profile-container-registry-settings)<br/>
27.5.2. [VHD Location *** - Mandatory](https://docs.microsoft.com/en-us/fslogix/configure-profile-container-tutorial#configure-profile-container-registry-settings)<br/>
28.5.3. [Initiate definition update on start up](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-event-based-updates-microsoft-defender-antivirus#use-group-policy-to-download-updates-when-microsoft-defender-antivirus-is-not-present)<br/>
29.5.4. [Specify interval to check for definition updates](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-protection-update-schedule-microsoft-defender-antivirus#use-group-policy-to-schedule-protection-updates)<br/>
30.5.5. [Define number of days before virus definitions are considered out of date](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-outdated-endpoints-microsoft-defender-antivirus#use-group-policy-to-specify-the-number-of-days-before-protection-is-considered-out-of-date)<br/>
31.5.6. [Define the number of days before spyware definitions are considered out of date](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-outdated-endpoints-microsoft-defender-antivirus#use-group-policy-to-specify-the-number-of-days-before-protection-is-considered-out-of-date)<br/>
32.5.7. [Define the number of days before a catchup day is required](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-outdated-endpoints-microsoft-defender-antivirus#use-group-policy-to-enable-and-configure-the-catch-up-update-feature)<br/>
33.5.8. [Check for latest virus and spyware definitions on startup](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-event-based-updates-microsoft-defender-antivirus#check-for-protection-updates-on-startup)<br/>
34.5.9. [Allow real time definition updates on report to microsoft MAPS](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-event-based-updates-microsoft-defender-antivirus#use-group-policy-to-automatically-download-recent-updates-based-on-cloud-delivered-protection)<br/>
35.5.10. [Allow definition updates from microsoft update](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-updates-mobile-devices-vms-microsoft-defender-antivirus#use-group-policy-to-opt-in-to-microsoft-update)<br/>
36.5.11. [Dynamic VHDX allocation](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#isdynamic)<br/>
37.5.12. [Extension Exclusions](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus#use-group-policy-to-configure-folder-or-file-extension-exclusions)<br/>
38.5.13. [SID directory name matching string](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#siddirnamematch)<br/>
39.5.14. [SID directory name pattern string](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#siddirnamepattern)<br/>
40.5.15. [Swap directory name components](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#flipflopprofiledirectoryname)<br/>
41.5.16. [Virtual disk type should be VHDX](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#volumetype)<br/>
42.5.17. [Size in Mbs](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#sizeinmbs)<br/>
43.5.18. [Delete local profile when FsLogix Profile should apply - Optional*](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#deletelocalprofilewhenvhdshouldapply)<br/>
44.5.19. [Prevent Login with failure - Optional*](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#preventloginwithfailure)<br/>
45.5.20. [Prevent login with temp profile -Optional](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#preventloginwithtempprofile)<br/>
46. **Using MSIX app attach:**<br/>
47.1. [What is MSIX app attach](https://docs.microsoft.com/en-us/azure/virtual-desktop/what-is-app-attach)<br/>
48.2. [Set up MSIX app attach](https://docs.microsoft.com/en-us/azure/virtual-desktop/app-attach)<br/>
49.3. [MSIX app attach FAQ](https://docs.microsoft.com/en-us/azure/virtual-desktop/app-attach-faq)<br/>
50. [**Create a Host Pool for Pooled Personal Desktops**](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-host-pools-azure-marketplace)<br/>
51. **Create a Host Pool for Pooled Remote Apps:**<br/>
52.1. [Publish built-in apps in Windows Virtual Desktop](https://docs.microsoft.com/en-us/azure/virtual-desktop/publish-apps)<br/>
53.3. [Manage app groups with the Azure portal] (https://docs.microsoft.com/en-us/azure/virtual-desktop/manage-app-groups)<br/>
54. **Configure host pool settings:**<br/>
55.1. [RDP Properties](https://docs.microsoft.com/en-us/azure/virtual-desktop/customize-rdp-properties)<br/>
56.2. [Configure device redirections (Mic, Speaker, Camera, Printer, Clipboard, USB, Local Drive, Plug and Play Devices)](https://docs.microsoft.com/en-us/azure/virtual-desktop/configure-device-redirections)<br/>
57.3. [Host pool load-balancing methods](https://docs.microsoft.com/en-us/azure/virtual-desktop/host-pool-load-balancing)<br/>
58.4. [Configure the Windows Virtual Desktop load-balancing method](https://docs.microsoft.com/en-us/azure/virtual-desktop/configure-host-pool-load-balancing)<br/>
59.5. [Personal desktop assignment type](https://docs.microsoft.com/en-us/azure/virtual-desktop/configure-host-pool-personal-desktop-assignment-type)<br/>
60. **Connect WVD with clients:**<br/>
61.1. [Windows Desktop Client](https://docs.microsoft.com/en-us/azure/virtual-desktop/connect-windows-7-10)<br/>
62.2. [HTML5 Web Client](https://docs.microsoft.com/en-us/azure/virtual-desktop/connect-web)<br/>
63.3. [Android Client](https://docs.microsoft.com/en-us/azure/virtual-desktop/connect-android)<br/>
64.4. [macOS Client](https://docs.microsoft.com/en-us/azure/virtual-desktop/connect-macos)<br/>
65.5. [iOS Client](https://docs.microsoft.com/en-us/azure/virtual-desktop/connect-ios)<br/>
66. [**Setup e-mail discovery to RDS feed**](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/rds-email-discovery)<br/>
67. **Setup Monitoring for WVD:**<br/>
68.1. [Azure Log Analytics and Azure Monitor](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/proactively-monitor-arm-based-windows-virtual-desktop-with-azure/ba-p/1508735)<br/>
69.2. [Sepago Solution](https://github.com/MarcelMeurer/LogAnalytics-for-Citrix-and-RDS)<br/>
70.3. [Azure Academy - Monitoring Workbook](https://www.youtube.com/watch?v=ERftVHEy5A4)<br/>
71.4. [Use Azure Monitor for Windows Virtual Desktop to monitor your deployment](https://docs.microsoft.com/en-us/azure/virtual-desktop/azure-monitor)
72. **Setup the WVD Scaling Tool:**<br/>
73.1. [Azure Automation](https://docs.microsoft.com/en-us/azure/virtual-desktop/set-up-scaling-script)<br/>
74.2. [Azure Academy - Scaling Automation](https://www.youtube.com/watch?v=4zDazJsa2Zk&t=604s)<br/>
75. **WVD Security:**<br/>
76.1. [Enabling MFA to WVD](https://docs.microsoft.com/en-us/azure/virtual-desktop/set-up-mfa)<br/>
77.2. [Azure Academy - Session Host Security](https://www.youtube.com/watch?v=5aK6BoXcZnU&t=328s)<br/>
78.3. [Security Best practices for WVD](https://docs.microsoft.com/en-us/azure/virtual-desktop/security-guide)<br/>
79.4. [Safe URL List](https://docs.microsoft.com/en-us/azure/virtual-desktop/safe-url-list)<br/>
80.5. [Use Azure Firewall to protect WVD](https://docs.microsoft.com/en-us/azure/firewall/protect-windows-virtual-desktop)<br/>
81. [**Configuring automatic updates using Endpoint Configuration Manager**](https://docs.microsoft.com/en-us/azure/virtual-desktop/configure-automatic-updates)
82. **WVD BCDR:**<br/>
83.1. [Setup BCDR Plan](https://docs.microsoft.com/en-us/azure/virtual-desktop/disaster-recovery)<br/>
84.2. [Disaster recovery considerations](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#disaster-recovery)<br/>
85.3. [Backup and restore considerations](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#backup-and-restore)<br/>
86. **GPO Suggestions:**<br/>
87.1. **Computer Configuration > Policies > Administrative Templates > Windows Components > Remote Desktop Services > Remote Desktop Session Host > Session Time Limits:**<br/>
88.1.1. Set time limit for active but idle Remote Desktop Services sessions: Enabled (e.g., 6 hours)<br/>
89.1.2. Set time limit for disconnected sessions: Enabled (e.g., 8 hours)<br/>
90.1.3. Set time limit for logoff of RemoteApp sessions: Enabled (e.g., 6 hours)<br/>
91.2. **User Configuration > Policies > Administrative Templates > Control Panel > Personalization:**<br/>
92.2.1. Force specific screen saver: Enabled (e.g., %winDir%\System32\ssText3d.scr)<br/>
93.2.2. Password protect the screen saver: Enabled<br/>
94.2.3. Prevent changing screen saver: Enabled<br/>
95.2.4. Screen saver timeout: Enabled (e.g., 80s)<br/>
