## Dynamic Device Group – Autopilot Devices

**Path:**  
Groups → Autopilot Devices (Dynamic Device Group)

### Purpose
Dynamic device groups are used to automatically target Windows Autopilot
devices with deployment profiles, configuration policies, and applications
without manual assignment.

This approach enables scalable and repeatable Autopilot deployments.

---

### Dynamic Membership Rule (Example)

(device.devicePhysicalIds -any (_ -eq "[OrderID]:RALI_Testing")) 
and 
(device.devicePhysicalIds -any (_ -contains "[ZTDId]"))

