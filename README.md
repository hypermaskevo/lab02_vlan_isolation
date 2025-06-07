# Lab 02 – VLAN Isolation

## 🧠 Objective
Understand how to isolate devices in a network using VLANs and verify communication restrictions between different VLANs.

![image](https://github.com/user-attachments/assets/e5699bce-ca6f-4bd6-a8ae-0df8c30b66a9)


## 🛠️ Topology
- 1 Switch
- 4 PCs
  - PC1 and PC2 → VLAN 10 (Sales)
  - PC3 and PC4 → VLAN 20 (Engineering)




## ⚙️ IP Configuration

| Device | IP Address     | Subnet Mask       | VLAN  |
|--------|----------------|-------------------|--------|
| PC1    | 192.168.10.1   | 255.255.255.0     | 10     |
| PC2    | 192.168.10.2   | 255.255.255.0     | 10     |
| PC3    | 192.168.20.1   | 255.255.255.0     | 20     |
| PC4    | 192.168.20.2   | 255.255.255.0     | 20     |



## 📡 Ping Test Results

| From | To   | Result     |
|------|------|------------|
| PC1  | PC2  | ✅ Success |
| PC3  | PC4  | ✅ Success |
| PC1  | PC3  | ❌ Failed  |


## ✅ Conclusion

✔️ Devices in the same VLAN can communicate  
✔️ Devices in different VLANs are isolated by default  
✔️ VLANs help create logical network separation for better security and organization



## 📎 Files

- `lab02_vlan_isolation.pkt` – Cisco Packet Tracer project file  
- `README.md` – This documentation
