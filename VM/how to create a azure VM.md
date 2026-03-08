# How to Create an Azure Virtual Machine (VM)

This guide explains the step-by-step process to create a Virtual Machine in Microsoft Azure using the Azure Portal.

---

## Prerequisites
- Active Azure subscription
- Access to [Azure Portal](https://portal.azure.com)
- Basic knowledge of VM requirements (OS, size, region)

---

## Steps to Create a VM

### 1. Sign in
- Go to [Azure Portal](https://portal.azure.com).
- Log in with your Azure account credentials.

### 2. Navigate to Virtual Machines
- In the left-hand menu, click **Virtual Machines**.
- Select **Create** → **Azure Virtual Machine**.

### 3. Basics Tab
- **Subscription**: Choose your subscription.
- **Resource Group**: Select or create one.
- **VM Name**: Enter a unique name.
- **Region**: Pick the closest region.
- **Image**: Select OS (Windows Server, Ubuntu, etc.).
- **Size**: Choose based on CPU/RAM needs.
- **Authentication**: Select **Password** or **SSH Key**.

### 4. Disks Tab
- Choose OS disk type (Premium SSD, Standard SSD, HDD).
- Add data disks if required.

### 5. Networking Tab
- Select or create a **Virtual Network** and **Subnet**.
- Assign a **Public IP** if external access is needed.
- Configure inbound port rules (RDP for Windows, SSH for Linux).

### 6. Management Tab
- Enable **Auto-shutdown** to save costs.
- Configure **Backup policies** if needed.
- Enable **Boot diagnostics** for troubleshooting.

### 7. Monitoring Tab
- Enable **Azure Monitor**.
- Connect to a **Log Analytics workspace**.
- Turn on **VM Insights** for performance monitoring.

### 8. Advanced Tab
- Add VM extensions (e.g., antivirus, custom scripts).
- Provide custom data (cloud-init, PowerShell).
- Configure dedicated host if required.

### 9. Tags Tab
- Add tags for organization (e.g., `Environment: Test`, `Owner: DevTeam`).

### 10. Review + Create
- Azure validates your configuration.
- If validation passes, click **Create**.
- Deployment begins and VM is provisioned.

---

## Accessing the VM
- **Windows VM**: Connect via **Remote Desktop (RDP)**.
- **Linux VM**: Connect via **SSH** using terminal.

---
![Basics Tab Screenshot](images/basics-tab.png)

