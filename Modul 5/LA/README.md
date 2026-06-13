# Tugas Modul Praktikum Jaringan Komputer — Modul 5

---

## 1. Topologi Jaringan & Addressing Plan

![Topologi tumod 5](https://github.com/user-attachments/assets/b33aa84e-3385-48a9-a74d-41f0caa2a453)

### 1.1 Alokasi IP Jaringan Internal Jakarta (HQ)

| VLAN | Nama VLAN | Network | Gateway Virtual | Keterangan |
| :---: | :--- | :--- | :--- | :--- |
| 10 | FINANCE | 192.168.10.0/24 | 192.168.10.1 | DHCP dari Ubuntu Server Jakarta |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 | DHCP dari Ubuntu Server Jakarta |
| 60 | SERVER-HQ | 192.168.60.0/24 | 192.168.60.1 | VLAN server Ubuntu Jakarta |

### 1.2 Alokasi IP Jaringan Internal Surabaya (Branch)

| VLAN | Nama VLAN | Network | Gateway | Keterangan |
| :---: | :--- | :--- | :--- | :--- |
| 30 | SALES | 192.168.30.0/24 | 192.168.30.1 | DHCP dari MikroTik Surabaya |
| 40 | OPERATIONS | 192.168.40.0/24 | 192.168.40.1 | IP static manual |

---

## 2. Bukti Konfigurasi per Tugas Modul

### Tugas Modul 1 - Konfigurasi Cisco Switch Jakarta

1. **Screenshot `show vlan brief`**
   ![VLAN Brief Jakarta](https://github.com/user-attachments/assets/3f777ff3-af3c-46a2-bd4b-0b6e1a61c37c)

2. **Screenshot `show interfaces trunk`**
   ![Interfaces Trunk Jakarta](https://github.com/user-attachments/assets/c6d804bc-41f5-4cca-b746-21a89e187434)

### Tugas Modul 2 - Konfigurasi Cisco Router Jakarta

1. **Screenshot `show ip interface brief`**
   ![IP Interface Brief Cisco](https://github.com/user-attachments/assets/a3e87aa1-1b94-4e15-a6ec-df277194ef83)

2. **Screenshot `show vrrp brief`**
   ![VRRP Brief Cisco](https://github.com/user-attachments/assets/0efc67c3-78db-4b8f-a858-fc5b1bd81097)

3. **Screenshot Ping dari Cisco Router ke FortiGate Jakarta**
   ![Ping Cisco to FortiGate](https://github.com/user-attachments/assets/45d08c59-2951-41dd-8c87-c846879556bc)

### Tugas Modul 3 - Konfigurasi MikroTik Router Jakarta

1. **Screenshot `/ip address print`**
   ![IP Address MikroTik Jakarta](https://github.com/user-attachments/assets/0263d334-5773-45e8-bf39-4567eb92796e)

2. **Screenshot `/interface vrrp print`**
   ![VRRP MikroTik](https://github.com/user-attachments/assets/7dac6e66-4962-44b2-8218-12f3a62e9d23)

3. **Screenshot `/ip dhcp-relay print`**
   ![DHCP Relay MikroTik](https://github.com/user-attachments/assets/15786248-6eeb-4a4e-b0ca-29159da33eb3)

4. **Screenshot `/ip route print`**
   ![IP Route MikroTik Jakarta](https://github.com/user-attachments/assets/f7c87c91-da05-413b-a891-c4181474302a)

5. **Screenshot Ping dari MikroTik ke FortiGate Jakarta**
   ![Ping MikroTik to FortiGate](https://github.com/user-attachments/assets/d4f867bc-7427-4b62-abac-aca8ed8695c4)

### Tugas Modul 4 - Konfigurasi Ubuntu Server Jakarta

1. **Screenshot `ip a`**
   ![IP Address Ubuntu](https://github.com/user-attachments/assets/990c1249-b955-45de-ae41-7041f0dc83f5)

2. **Screenshot `ip route`**
   ![IP Route Ubuntu](https://github.com/user-attachments/assets/1cc442a8-60b0-4316-8454-d1ab083c8f11)

3. **Screenshot isi file `/etc/dhcp/dhcpd.conf`**
   ![DHCP Config Ubuntu](https://github.com/user-attachments/assets/0ab87735-34d9-43f1-8d5d-bc6845e5aa63)

4. **Screenshot `ping 8.8.8.8` dari Ubuntu Server**
   ![Ping Internet Ubuntu](https://github.com/user-attachments/assets/671f4357-2f19-4fe8-b54c-3b99e38fa3bd)

### Tugas Modul 5 - Konfigurasi FortiGate Jakarta

1. **Screenshot `get system interface physical`**
   ![FortiGate JKT Interfaces](https://github.com/user-attachments/assets/2537bd68-b3a8-4a1f-ac75-9aff630b2fb5)

2. **Screenshot `get router info routing-table all`**
   ![FortiGate JKT Routing Table](https://github.com/user-attachments/assets/9040b292-fdd3-48c9-97da-9c0c9d5439cc)

3. **Screenshot Firewall Policy & NAT**
   ![FortiGate JKT Policy](https://github.com/user-attachments/assets/085d7292-3b2f-4b0f-af60-fcb13acdccd1)

4. **Screenshot ping ke 8.8.8.8**
   ![FortiGate JKT Ping Internet](https://github.com/user-attachments/assets/8798a4dc-3b5e-46cf-9639-6fb284058f6a)

5. **Screenshot ping ke IP tunnel Surabaya**
   ![FortiGate JKT Ping Tunnel](https://github.com/user-attachments/assets/b8d23e07-679f-4a67-9b70-9ef3e84cd423)

6. **Screenshot `get router info ospf neighbor`**
   ![FortiGate JKT OSPF Neighbor](https://github.com/user-attachments/assets/dd67dac5-0eb5-43a3-98f0-ff17fe2f0ba8)

7. **Screenshot `get router info routing-table ospf`**
   ![FortiGate JKT OSPF Route](https://github.com/user-attachments/assets/8c7887ae-5b93-4588-9256-a345b4502f76)

### Tugas Modul 6 - Konfigurasi MikroTik ISP

1. **Screenshot `/ip address print`**
   ![ISP IP Address](https://github.com/user-attachments/assets/73044fcf-d9c1-4702-894b-e9ecaf40301e)

2. **Screenshot `/ip route print`**
   ![ISP Routing Table](https://github.com/user-attachments/assets/9be69fb6-7e1d-4241-aef1-a346fbc14cab)

3. **Screenshot `/ip firewall nat print`**
   ![ISP NAT Masquerade](https://github.com/user-attachments/assets/fff0a6f8-6e7b-46ca-8bea-9f6a5d3ccedb)

4. **Screenshot ping ke 8.8.8.8**
   ![ISP Ping Internet](https://github.com/user-attachments/assets/61d63c4f-fadd-4cfb-bcdc-99f33ee8836c)

5. **Screenshot ping antar-WAN FortiGate**
   ![ISP Ping Antar WAN](https://github.com/user-attachments/assets/cb960e77-4b51-4733-a4f0-b0647a8dc439)

### Tugas Modul 7 - Konfigurasi Switch dan MikroTik Surabaya

1. **Screenshot `show vlan brief` Switch Surabaya**
   ![Switch Surabaya VLAN](https://github.com/user-attachments/assets/a20dbf92-968e-46bd-bbf2-0b355c8d1926)

2. **Screenshot `show interfaces trunk` Switch Surabaya**
   ![Switch Surabaya Trunk](https://github.com/user-attachments/assets/da29bf32-5f12-49e8-8757-a299bbeee658)

3. **Screenshot `/ip address print` MikroTik Surabaya**
   ![MikroTik Surabaya IP](https://github.com/user-attachments/assets/f59da436-7419-4423-8dd8-2a8ef73e057a)

4. **Screenshot `/ip dhcp-server print` MikroTik Surabaya**
   ![MikroTik Surabaya DHCP Server](https://github.com/user-attachments/assets/443375fb-1a05-46ef-85c7-02dd2fdea246)

5. **Screenshot `/ip pool print` MikroTik Surabaya**
   ![MikroTik Surabaya IP Pool](https://github.com/user-attachments/assets/e14c8ff1-daf7-4e52-b34c-509e7c87112b)

6. **Screenshot `/ip route print` MikroTik Surabaya**
   ![MikroTik Surabaya Route](https://github.com/user-attachments/assets/7ef5d01c-5769-488b-80b1-e99df2d5d391)

7. **Screenshot Client VLAN 30 mendapat IP DHCP**
   ![Client Surabaya DHCP](https://github.com/user-attachments/assets/56845b8d-24c6-4695-b429-99d0aa6fdae4)

8. **Screenshot ping client Surabaya ke 8.8.8.8**
   ![Client Surabaya Ping Internet](https://github.com/user-attachments/assets/c9968a8e-8422-4219-a9e5-d26c2b27f021)

### Tugas Modul 8 & 9 - Konfigurasi FortiGate Surabaya & Jalur GRE OSPF

1. **Screenshot `get system interface physical`**
   ![FortiGate SBY Interfaces](https://github.com/user-attachments/assets/7c97fb20-1e6e-4c25-8c51-f34d4f1b36fa)

2. **Screenshot `get router info routing-table all`**
   ![FortiGate SBY Routing Table](https://github.com/user-attachments/assets/7f747bc7-c42e-42e2-acd4-852ff418a376)

3. **Screenshot Firewall Policy**
   ![FortiGate SBY Policy](https://github.com/user-attachments/assets/19efea7f-e51d-4e39-84e6-981ec2be39b5)

4. **Screenshot ping ke 8.8.8.8**
   ![FortiGate SBY Ping Internet](https://github.com/user-attachments/assets/90ac558e-7fd5-487e-8d34-1dc8b42965d0)

5. **Screenshot ping ke IP tunnel Jakarta**
   ![FortiGate SBY Ping Tunnel](https://github.com/user-attachments/assets/febdfffe-d405-4d70-9a31-d918f5b18ecd)

6. **Screenshot `get router info ospf neighbor` (Hubungan Adjacency)**
   ![OSPF Neighbor Full](https://github.com/user-attachments/assets/83614a68-d4ef-498f-90bd-92292759d844)

7. **Screenshot `get router info routing-table ospf` (Sisi Surabaya)**
   ![OSPF Table Surabaya](https://github.com/user-attachments/assets/ff3b1d33-9c15-4adc-b080-59dde63f2b91)

8. **Screenshot `get router info routing-table ospf` (Sisi Jakarta)**
   ![OSPF Table Jakarta](https://github.com/user-attachments/assets/64122300-2d34-4f15-8f7f-89e2b045efce)

---

## 3. Tugas Modul 10 - Pengujian Akhir End-to-End

### 3.1 Alokasi IP Otomatis Client (DHCP Verification)
* **Screenshot IP DHCP Client Jakarta (VLAN 10)**
  ![DHCP Client JKT](https://github.com/user-attachments/assets/3477626b-de9c-4dbd-b5f6-a9f93395f50e)
* **Screenshot IP DHCP Client Surabaya (VLAN 30)**
  ![DHCP Client SBY](https://github.com/user-attachments/assets/1fbd49bf-ede4-408b-9a5c-66fd2d50d2e1)

### 3.2 Verifikasi Akses Internet Internet (NAT Gateway)
* **Screenshot Ping Internet dari Jakarta (VLAN 10)**
  ![Ping Internet JKT](https://github.com/user-attachments/assets/80b1e761-664a-4545-b293-4b110d7a4527)
* **Screenshot Ping Internet dari Surabaya (VLAN 30)**
  ![Ping Internet SBY](https://github.com/user-attachments/assets/994ac599-80a2-47fc-b9c5-e0fbbdd2b218)

### 3.3 Uji Konektivitas Antar-Site Lewat Tunnel GRE & Routing OSPF
* **Screenshot Ping Client Jakarta ke Client Surabaya**
  ![Ping Client JKT to SBY](https://github.com/user-attachments/assets/889dbb24-a5b0-4c0f-96d6-2950750043cb)
* **Screenshot Ping Client Surabaya ke Client Jakarta**
  ![Ping Client SBY to JKT](https://github.com/user-attachments/assets/68b2ab17-fe5a-4af3-8919-5d09c8e55cc1)
* **Screenshot Ping Spesifik Antar-Site (VLAN 10 Jakarta ke VLAN 40 Surabaya)**
  ![Ping Spec JKT SBY](https://github.com/user-attachments/assets/33df47f8-294d-4d6d-b441-a7e935856287)

### 3.4 Pengujian Layanan Web Server Aplikasi (HTTP Protocol)
* **Screenshot Akses Web Server Jakarta dari Browser Client Surabaya**
  ![Akses Web Nginx](https://github.com/user-attachments/assets/610f851b-7140-4026-904c-7260acfbb350)
