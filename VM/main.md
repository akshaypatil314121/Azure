# Azure Windows Virtual Machine Operations

This document provides step-by-step Standard Operating Procedures (SOPs) for common Azure VM tasks. Use it as a quick reference guide.

---

## 1. Create a VM on portal
- Go to [Azure Portal](https://portal.azure.com).
- Navigate to **Virtual Machines** → **Create**.
- Fill in **Basics, Disks, Networking, Management, Monitoring, Advanced, Tags**.
- Click **Review + Create** → **Create**.
- (docs/How to create a Azure VM.md)

---

## 2. Create and Attach Disk
- Open VM → **Disks** → **+ Add data disk**.
- Choose **Create disk** or **Select existing disk**.
- Save and Initialize Disk** → RDP → Disk Management → Initialize → Format.

---

## 3. Swap Disk
- Stop/deallocate the VM.
- Go to **Virtual Machines** → select your VM.
- In the left menu, click **Disks**.
- Under **OS Disk**, click **Swap OS Disk**.
- Select the replacement managed disk.
- Save changes.
- Start the VM again.

---

## 4. Take a Backup
- Go to **Backup center**.
- Configure Recovery Services vault.
- Enable backup for VM.

---

## 5. Resize the VM
- VM → **Size** → Select new size.
- Save and restart VM.

---

## 6. Take a Snapshot
- VM → **Disks** → Select OS/Data disk.
- Click **Create snapshot**.

---

## 7. Add Server into Patching
- Use **Update Management** in Azure Automation.
- Register VM for patching schedules.

---

## 8. Add Server into Monitoring
- Enable **Azure Monitor** and **Log Analytics**.
- Configure VM Insights.

---

## 9. Create Bastion to Login Server
- VM → **Connect** → **Bastion**.
- Deploy Bastion host in same VNet.
- Connect securely without public IP.

---

## 10. Patch the Server
- Use **Update Management** or manual OS updates.
- Verify compliance in Azure Monitor.

---

## 11. Expand Disk Size
- VM → **Disks** → Select disk → **Resize**.
- Update partition inside OS.

---

## 12. Create Alerts Rule
- Azure Monitor → **Alerts** → **New alert rule**.
- Define condition (CPU, memory, etc.).
- Assign action group.

---

## 13. Reserved Server Size
- Purchase **Reserved Instances** for cost savings.
- Apply to VM size/region.

---

## 14. Quota Management
- Check subscription quotas.
- Request quota increase if needed.

---

## 15. Auto Start/Stop Server
- Use **Automation Account** or **Azure DevTest Labs**.
- Configure schedules.

---

## 16. Decommissioning Server
- Backup data.
- Delete VM and associated resources.

---

## 17. Add Tags
- VM → **Tags** → Add key-value pairs.

---

## 18. Assign RBAC Role
- VM → **Access control (IAM)**.
- Add role assignment to user/group.

---

## 19. Create NSG Rule
- VM → **Networking** → NSG.
- Add inbound/outbound rules.

---

## 20. Install/Update Extensions (e.g., AMA)
- VM → **Extensions** → Add/Update extension.

---

## 21. Licensing
- Verify OS licensing (Windows/Linux).
- Apply hybrid benefit if eligible.

---

## 22. Azure Advisor Recommendations
- Open **Azure Advisor**.
- Review performance, cost, security recommendations.
- Apply fixes.

---

## 23. Apply Resource Lock
- VM → **Locks** → Add lock (Read-only/Delete).

---

## 24. Availability Set/Zone
- Configure during VM creation.
- Improves redundancy.

---

## 25. Enable System/User Identity
- VM → **Identity** → Enable system-assigned or user-assigned.

---

## 26. Onboard Server to Defender for Cloud
- Enable Defender for Cloud.
- Register VM for security monitoring.

---

## 27. Disaster Recovery
- Configure **Azure Site Recovery**.
- Replicate VM to secondary region.

---

## 28. Restore Points
- VM → **Backup** → Manage restore points.
- Delete unused restore points.

---

## 29. Run Commands
- VM → **Run command**.
- Execute scripts remotely.

---

## 30. One-Time Update
- Apply manual OS updates if required.

---

## 31. Apply Policy
- Use **Azure Policy** to enforce compliance.

---

## 32. Logs & Monitoring
- Use Log Analytics queries for heartbeat, tables, etc.
- Build workbooks for visualization.

---

## 33. Validate Resource Health
- VM → **Resource health**.
- Check availability status.

---

## 34. Boot Diagnostics
- VM → **Boot diagnostics**.
- Review screenshots/logs for startup issues.

---

## 35. Serial Console
- VM → **Serial console**.
- Access low-level troubleshooting.

---

## 36. Reset Admin Password
- VM → **Reset password** under Support + Troubleshooting.

---

## 37. Connection Troubleshoot
- VM → **Networking** → **Connection troubleshoot**.

---

## 38. Redeploy VM
- VM → **Redeploy**.
- Moves VM to new host.

---

## 39. Support Case
- Help + Support → **New support request**.

---

## 40. Move VM to Another Resource Group
- VM → **Move** → Select new resource group.

