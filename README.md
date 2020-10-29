# WVD Guidance Links  
This repository contains the information needed to describe the main topics on a wvd architecture design and implementation.

## WVD Architecture Guidance

1. [What is WVD](https://docs.microsoft.com/en-us/azure/virtual-desktop/overview)
2. [WVD Requirements](https://docs.microsoft.com/en-us/azure/virtual-desktop/overview#requirements)
3. [Supported OS images](https://docs.microsoft.com/en-us/azure/virtual-desktop/overview#supported-virtual-machine-os-images)
4. [Network guidelines](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/network-guidance?context=/azure/virtual-desktop/context/context)
5. [Windows Virtual Desktop experience estimator](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/network-guidance?context=/azure/virtual-desktop/context/context#windows-virtual-desktop-experience-estimator)
6. Virtual Machine Guidance<br/>
6.1. [Virtual machine sizing guidelines](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs?context=/azure/virtual-desktop/context/context)<br/>
6.2. [Multi-session recommendations](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs#multi-session-recommendations)<br/>
6.3. [Single-session recommendations](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs?context=/azure/virtual-desktop/context/context#single-session-recommendations)<br/>
6.4. [General virtual machine recommendations](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/virtual-machine-recs?context=/azure/virtual-desktop/context/context#general-virtual-machine-recommendations)<br/>
7. [WVD Architecture Sample](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop#architecture)
8. FSLogix<br/>
8.1. [FSLogix for enterprise](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix)<br/>
8.2. [Storage options for FSLogix profile containers](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#storage-options-for-fslogix-profile-containers)<br/>
8.3. [Azure Files Best practices](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#azure-files-best-practices)<br/>
8.4. [Azure NetApp Files Best Practices](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#azure-netapp-files-best-practices)<br/>
9. [Best Practices for WVD](https://docs.microsoft.com/en-us/azure/virtual-desktop/fslogix-containers-azure-files#best-practices-for-windows-virtual-desktop)


## WVD Deployment Guidance

1. [Deploy an Azure AD Tenant](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-create-new-tenant)
2. [Deploy an Azure Subscription](https://docs.microsoft.com/en-us/azure/cost-management-billing/manage/create-subscription)
3. Deploy Azure infrastructure and AD DS<br/>
3.1. [Virtual Network](https://docs.microsoft.com/en-us/azure/virtual-network/quick-create-portal)<br/>
3.2. [Subnet](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-network-manage-subnet#add-a-subnet)<br/>
3.3. [NSG](https://docs.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview) (Permits AD Traffic, RDP incoming traffic, restricts DMZ access)<br/>
3.4. [DNS configured to point to the domain controller](https://docs.microsoft.com/en-us/azure/virtual-network/manage-virtual-network#change-dns-servers)<br/>
3.5. [Virtual Machine](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/quick-create-portal)<br/>
3.5.1. Active Directory Domain Services installed and configured<br/>
3.5.2. Azure AD Connect installed and ready for configuration<br/>
4. Configure Azure AD Connect with AD DS<br/>
4.1. [What is Azure AD Connect](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-azure-ad-connect)<br/>
4.2. [Azure AD connect and Azure AD Connect Health installation](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-install-roadmap)<br/>
5. [Windows Virtual Desktop environment concepts](https://docs.microsoft.com/en-us/azure/virtual-desktop/environment-setup)<br/>
6. [Create Azure AD Security Groups for WVD](htps://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)<br/>
7. [Assign users to Groups](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/active-directory-groups-members-azure-portal)<br/>
8. Create a Master Image for WVD<br/>
8.1. [Create a Master Image for WVD](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/capture-image-resource)<br/>
8.1.2. [Install Office on a master VHD image](https://docs.microsoft.com/en-us/azure/virtual-desktop/install-office-on-wvd-master-image)<br/>
8.1.3. [Install Microsoft Teams on a WVD](https://docs.microsoft.com/en-us/azure/virtual-desktop/teams-on-wvd)<br/>
8.1.4. [Azure Academy - Teams AV Redirect](https://www.youtube.com/watch?v=RfbolIgPcBY&t=661s)<br/>
8.1.5. [Download and install FSLogix](https://docs.microsoft.com/en-us/fslogix/install-ht)<br/>
8.1.6. [OS Settings | Prepare and customize a master VHD image](https://docs.microsoft.com/en-us/azure/virtual-desktop/set-up-customize-master-image)<br/>
8.1.7. [OS Settings | Prepare a Windows VHD or VHDX to upload to Azure](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/prepare-for-upload-vhd-image)<br/>
8.1.8. [OS Settings | Run Disk Cleanup](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/cleanmgr)<br/>
9. Image Management<br/>
9.1. [Azure Academy - Image Management](https://www.youtube.com/watch?v=PCWJEoG8X-I)<br/>
9.1.2. [Azure Academy - Shared Image Gallery](https://www.youtube.com/watch?v=2LxvwR9LGWQ)<br/>
10. Define a strategy to store FSLogix profiles containers<br/>
10.1. [Storage options for FSLogix Profile containers](https://docs.microsoft.com/en-us/azure/virtual-desktop/store-fslogix-profile)<br/>
10.1.1. [Azure Files and Active Directory Domain Services](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-file-share)<br/>
10.1.2. [Azure NetApp Files](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-fslogix-profile-container)<br/>
10.1.3. [Windows File Server](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-host-pools-user-profile)<br/>
10.1.4. [Azure Files and Azure Active Directory Domain Services](https://docs.microsoft.com/en-us/azure/virtual-desktop/create-profile-container-adds)<br/>
11. FSLogix General Configuration<br/>
11.1. [Use FSLogix Group Policy Template Files](https://docs.microsoft.com/en-us/fslogix/use-group-policy-templates-ht)<br/>
11.2. [Profile Container registry configuration reference](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference)<br/>
11.3. [Antivirus exclusions](https://docs.microsoft.com/en-us/azure/architecture/example-scenario/wvd/windows-virtual-desktop-fslogix#antivirus-exclusions)
11.4. FSLogix Reference Links
11.4.1. [Azure Academy - FSLogix with Azure Fileshare](https://www.youtube.com/watch?v=9S5A1IJqfOQ&t=647s)
11.4.2. [Azure Academy - NetApp](https://www.youtube.com/watch?v=bswIbTB62mY)
11.5. GPO Recommendations
11.5.1. [Enabled *** - Mandatory](https://docs.microsoft.com/en-us/fslogix/configure-profile-container-tutorial#configure-profile-container-registry-settings)
11.5.2. [VHD Location *** - Mandatory](https://docs.microsoft.com/en-us/fslogix/configure-profile-container-tutorial#configure-profile-container-registry-settings)
11.5.3. [Initiate definition update on start up](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-event-based-updates-microsoft-defender-antivirus#use-group-policy-to-download-updates-when-microsoft-defender-antivirus-is-not-present)
11.5.4. [Specify interval to check for definition updates](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-protection-update-schedule-microsoft-defender-antivirus#use-group-policy-to-schedule-protection-updates)
11.5.5. [Define number of days before virus definitions are considered out of date](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-outdated-endpoints-microsoft-defender-antivirus#use-group-policy-to-specify-the-number-of-days-before-protection-is-considered-out-of-date)
11.5.6. [Define the number of days before spyware definitions are considered out of date](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-outdated-endpoints-microsoft-defender-antivirus#use-group-policy-to-specify-the-number-of-days-before-protection-is-considered-out-of-date)
11.5.7. [Define the number of days before a catchup day is required](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-outdated-endpoints-microsoft-defender-antivirus#use-group-policy-to-enable-and-configure-the-catch-up-update-feature)
11.5.8. [Check for latest virus and spyware definitions on startup](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-event-based-updates-microsoft-defender-antivirus#check-for-protection-updates-on-startup)
11.5.9. [Allow real time definition updates on report to microsoft MAPS](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-event-based-updates-microsoft-defender-antivirus#use-group-policy-to-automatically-download-recent-updates-based-on-cloud-delivered-protection)
11.5.10. [Allow definition updates from microsoft update](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/manage-updates-mobile-devices-vms-microsoft-defender-antivirus#use-group-policy-to-opt-in-to-microsoft-update)
11.5.11. [Dynamic VHDX allocation](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#isdynamic)
11.5.12. [Extension Exclusions](https://docs.microsoft.com/en-us/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus#use-group-policy-to-configure-folder-or-file-extension-exclusions)
11.5.13. [SID directory name matching string](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#siddirnamematch)
11.5.14. [SID directory name pattern string](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#siddirnamepattern)
11.5.15. [Swap directory name components](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#flipflopprofiledirectoryname)
11.5.16. [Virtual disk type should be VHDX](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#volumetype)
11.5.17. [Size in Mbs](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#sizeinmbs)
11.5.18. [Delete local profile when FsLogix Profile should apply - Optional*](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#deletelocalprofilewhenvhdshouldapply)
11.5.19. [Prevent Login with failure - Optional*](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#preventloginwithfailure)
11.5.20. [Prevent login with temp profile -Optional](https://docs.microsoft.com/en-us/fslogix/profile-container-configuration-reference#preventloginwithtempprofile)


12.
13.
14.
15.
16.
17.
18.
19.
20.
21. 
22.
23.

