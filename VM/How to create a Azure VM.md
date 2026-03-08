SOP: How to Create an Azure Virtual Machine (VM)
🔹 Prerequisites
Active Azure subscription

Access to Azure Portal

Basic knowledge of VM requirements (OS, size, region)

🔹 Procedure
Step 1: Sign in
Go to portal.azure.com.

Log in with your Azure account credentials.

Step 2: Navigate to Virtual Machines
In the left-hand menu, click Virtual Machines.

Select Create → Azure Virtual Machine.

Step 3: Basics Tab
Subscription: Choose your subscription.

Resource Group: Select or create one.

VM Name: Enter a unique name.

Region: Pick the closest region (e.g., Central India).

Image: Select OS (Windows Server, Ubuntu, etc.).

Size: Choose based on CPU/RAM needs.

Authentication: Select Password or SSH Key.

Step 4: Disks Tab
Choose OS disk type (Premium SSD, Standard SSD, HDD).

Add data disks if required.

Step 5: Networking Tab
Select or create a Virtual Network and Subnet.

Assign a Public IP if external access is needed.

Configure inbound port rules (RDP for Windows, SSH for Linux).

Step 6: Management Tab
Enable Auto-shutdown to save costs.

Configure Backup policies if needed.

Enable Boot diagnostics for troubleshooting.

Step 7: Monitoring Tab
Enable Azure Monitor.

Connect to a Log Analytics workspace.

Turn on VM Insights for performance monitoring.

Step 8: Advanced Tab
Add VM extensions (e.g., antivirus, custom scripts).

Provide custom data (cloud-init, PowerShell).

Configure dedicated host if required.

Step 9: Tags Tab
Add tags for organization (e.g., Environment: Test, Owner: DevTeam).

Step 10: Review + Create
Azure validates your configuration.

If validation passes, click Create.

Deployment begins and VM is provisioned.

Step 11: Access the VM
Windows VM: Connect via Remote Desktop (RDP).

Linux VM: Connect via SSH using terminal.
