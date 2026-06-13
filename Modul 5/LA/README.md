Tugas Modul Praktikum Jaringan Komputer Modul 5

**1. Topologi Jaringan & Addressing Plan**
<img width="539" height="402" alt="Topologi tumod 5" src="https://github.com/user-attachments/assets/b33aa84e-3385-48a9-a74d-41f0caa2a453" />

**1.1 Alokasi IP Jaringan Internal Jakarta (HQ)**
| VLAN | Nama VLAN | Network         | Gateway Virtual | Keterangan                      |
| ---- | --------- | --------------- | --------------- | ------------------------------- |
|   10 | FINANCE   | 192.168.10.0/24 | 192.168.10.1    | DHCP dari Ubuntu Server Jakarta |
|   20 | IT        | 192.168.20.0/24 | 192.168.20.1    | DHCP dari Ubuntu Server Jakarta |
|   60 | SERVER-HQ | 192.168.60.0/24 | 192.168.60.1    | VLAN server Ubuntu Jakarta      |

**1.2 Alokasi IP Jaringan Internal Surabaya (Branch)**
| VLAN | Nama VLAN  | Network         | Gateway      | Keterangan                  |
| ---- | ---------- | --------------- | ------------ | --------------------------- |
|   30 | SALES      | 192.168.30.0/24 | 192.168.30.1 | DHCP dari MikroTik Surabaya |
|   40 | OPERATIONS | 192.168.40.0/24 | 192.168.40.1 | IP static manual            |

**2. Bukti Konfigurasi per Tugas Modul**
**Tugas Modul 1 - Konfigurasi Cisco Switch Jakarta**
1. Screenshot 'show vlan brief'
   
<img width="903" height="504" alt="d75ddee2-1792-43d8-b715-d4ccdb87c82a" src="https://github.com/user-attachments/assets/3f777ff3-af3c-46a2-bd4b-0b6e1a61c37c" />
3. Screenshot 'show interfaces trunk'
<img width="901" height="499" alt="5a94c4f1-ecfd-4f9e-aa78-9edb0743ef54" src="https://github.com/user-attachments/assets/c6d804bc-41f5-4cca-b746-21a89e187434" />

**Tugas Modul 2 - Konfigurasi Cisco Router Jakarta**
1. Screenshot 'show ip interface brief'
<img width="903" height="507" alt="7f9c8130-3daa-43c1-a8aa-94ac5b473523" src="https://github.com/user-attachments/assets/a3e87aa1-1b94-4e15-a6ec-df277194ef83" />
2. Screenshot 'show vrrp brief'
<img width="909" height="510" alt="2c87651d-ce08-430d-90c4-f0a0ea366c9b" src="https://github.com/user-attachments/assets/0efc67c3-78db-4b8f-a858-fc5b1bd81097" />
3. Screenshot Ping dari Cisco Router ke FortiGate Jakarta
<img width="900" height="507" alt="7edeb0e5-a50f-462e-9455-e3b7def43df4" src="https://github.com/user-attachments/assets/45d08c59-2951-41dd-8c87-c846879556bc" />

**Tugas Modul 3 - Konfigurasi MikroTik Router Jakarta**
1. Screenshot '/ip address print'
<img width="904" height="507" alt="c991a352-f3cd-4153-a56f-49c7a32f15ed" src="https://github.com/user-attachments/assets/0263d334-5773-45e8-bf39-4567eb92796e" />
2. Screenshot '/interface vrrp print'
<img width="900" height="513" alt="cf7ad770-b42e-4f69-aa94-c723404deb96" src="https://github.com/user-attachments/assets/7dac6e66-4962-44b2-8218-12f3a62e9d23" />
3. Screenshot '/ip-dhcp relay print'
<img width="903" height="502" alt="426968e2-f001-4deb-9019-c58a585a68af" src="https://github.com/user-attachments/assets/15786248-6eeb-4a4e-b0ca-29159da33eb3" />
4. Screenshot '/ip route print'
<img width="903" height="510" alt="53984d4d-2594-4028-9660-844d1f0f4684" src="https://github.com/user-attachments/assets/f7c87c91-da05-413b-a891-c4181474302a" />
5. Screenshot Ping dari MikroTik ke FortiGate Jakarta
<img width="898" height="505" alt="6c97065d-35a1-43ed-b067-6e9beceb98f6" src="https://github.com/user-attachments/assets/d4f867bc-7427-4b62-abac-aca8ed8695c4" />

**Tugas Modul 4 - Konfigurasi Ubuntu Server Jakarta**
1. Screenshot 'ip a'
<img width="898" height="505" alt="a5cca8b1-7f23-4a38-b684-dd65aedc2004" src="https://github.com/user-attachments/assets/990c1249-b955-45de-ae41-7041f0dc83f5" />
2. Screenshot 'ip route'
<img width="906" height="502" alt="e2d83293-2478-4a83-a899-38df506d26f8" src="https://github.com/user-attachments/assets/1cc442a8-60b0-4316-8454-d1ab083c8f11" />
3. Screenshot isi file `/etc/dhcp/dhcpd.conf`
<img width="907" height="511" alt="83745878-5b83-4652-81f6-0f5c2bcf09d8" src="https://github.com/user-attachments/assets/0ab87735-34d9-43f1-8d5d-bc6845e5aa63" />
4. Screenshot `ping 8.8.8.8` dari Ubuntu Server
<img width="903" height="504" alt="aa153280-44db-4560-8771-4b6322e2ac54" src="https://github.com/user-attachments/assets/671f4357-2f19-4fe8-b54c-3b99e38fa3bd" />

**Tugas Modul 5 - Konfigurasi FortiGate Jakarta**
1. Screenshot 'get system interface physical`
<img width="1243" height="787" alt="de1a6726-9759-4a71-8d20-7be10a9f6204" src="https://github.com/user-attachments/assets/2537bd68-b3a8-4a1f-ac75-9aff630b2fb5" />
2. get router info routing-table all
<img width="1248" height="790" alt="fe8e8bc1-f381-4f5d-afaa-f0fff7bbe5f6" src="https://github.com/user-attachments/assets/9040b292-fdd3-48c9-97da-9c0c9d5439cc" />
3. Screenshot Firewall Policy & NAT
<img width="634" height="441" alt="ce0ed76b-8e77-4a33-967e-62e1b7923d4f" src="https://github.com/user-attachments/assets/085d7292-3b2f-4b0f-af60-fcb13acdccd1" />
4. Screenshot ping ke 8.8.8.8
<img width="589" height="415" alt="92468332-7369-4fdf-8b5d-f4bb9f452e75" src="https://github.com/user-attachments/assets/8798a4dc-3b5e-46cf-9639-6fb284058f6a" />
5. Screenshot ping ke IP tunnel Surabaya.
<img width="742" height="513" alt="e0f0337a-941b-484c-869b-291b1c205889" src="https://github.com/user-attachments/assets/b8d23e07-679f-4a67-9b70-9ef3e84cd423" />
6. Screenshot get router info ospf neighbor.
<img width="742" height="516" alt="f77bb842-7ae7-47fd-817d-d1bdd8640d06" src="https://github.com/user-attachments/assets/dd67dac5-0eb5-43a3-98f0-ff17fe2f0ba8" />
7. Screenshot get router info routing-table ospf
<img width="751" height="517" alt="7398cbb2-1325-415d-93a6-fb37067d57f6" src="https://github.com/user-attachments/assets/8c7887ae-5b93-4588-9256-a345b4502f76" />

**Tugas Modul 6 - Konfigurasi MikroTik ISP**
1. Screenshot /ip address print hasil di ether 1 bisa saja berbeda karena emang dinamic.
<img width="615" height="366" alt="c51b8675-07ed-4708-a74e-66c86a71b43b" src="https://github.com/user-attachments/assets/73044fcf-d9c1-4702-894b-e9ecaf40301e" />
2. Screenshot /ip route print
<img width="775" height="532" alt="cc56c032-54b4-4405-abbd-20410ffca4e7" src="https://github.com/user-attachments/assets/9be69fb6-7e1d-4241-aef1-a346fbc14cab" />
3. Screenshot /ip firewall nat print
<img width="769" height="427" alt="750056a7-8cf4-4691-9112-080ab16fd998" src="https://github.com/user-attachments/assets/fff0a6f8-6e7b-46ca-8bea-9f6a5d3ccedb" />
4. Screenshot ping ke 8.8.8.8.
<img width="786" height="532" alt="0d4e8714-5fc5-44d5-8c03-7e4367745bb0" src="https://github.com/user-attachments/assets/61d63c4f-fadd-4cfb-bcdc-99f33ee8836c" />
5. Screenshot ping antar-WAN FortiGate.
<img width="775" height="529" alt="f1b85d63-38a2-4288-94a6-5177d4d3085a" src="https://github.com/user-attachments/assets/cb960e77-4b51-4733-a4f0-b0647a8dc439" />

**Tugas Modul 7 - Konfigurasi Switch dan MikroTik Surabaya**
1. Screenshot show vlan brief
<img width="789" height="535" alt="0de98348-454e-48ce-ba92-e59c5cdb0ddb" src="https://github.com/user-attachments/assets/a20dbf92-968e-46bd-bbf2-0b355c8d1926" />
2. Screenshot show interfaces trunk
<img width="787" height="538" alt="721f3349-2f19-409c-9c17-8916c0524331" src="https://github.com/user-attachments/assets/da29bf32-5f12-49e8-8757-a299bbeee658" />
3. Screenshot /ip address print
<img width="783" height="535" alt="53f1317d-d951-4cbe-af34-52e4f2005c66" src="https://github.com/user-attachments/assets/f59da436-7419-4423-8dd8-2a8ef73e057a" />
4. Screenshot /ip dhcp-server print
<img width="780" height="538" alt="859683c2-59cd-44f8-9bad-58c14c651329" src="https://github.com/user-attachments/assets/443375fb-1a05-46ef-85c7-02dd2fdea246" />
5. Screenshot /ip pool print
<img width="784" height="577" alt="1a1b283e-b31e-44ad-b502-daa7f69b5e0b" src="https://github.com/user-attachments/assets/e14c8ff1-daf7-4e52-b34c-509e7c87112b" />
6. Screenshot /ip route print
<img width="781" height="532" alt="761992c2-fdd0-4e31-96e8-b195cc6ef0c0" src="https://github.com/user-attachments/assets/7ef5d01c-5769-488b-80b1-e99df2d5d391" />
7. Screenshot client VLAN 30 mendapat IP DHCP.
<img width="775" height="534" alt="8124dc61-a1f2-4c63-9ca5-a814991b336b" src="https://github.com/user-attachments/assets/56845b8d-24c6-4695-b429-99d0aa6fdae4" />
8. Screenshot ping client Surabaya ke 8.8.8.8.
<img width="778" height="540" alt="4f24d1fa-cadf-44af-9b57-5d306476da83" src="https://github.com/user-attachments/assets/c9968a8e-8422-4219-a9e5-d26c2b27f021" />

**Tugas Modul 8 - Konfigurasi FortiGate Surabaya**
1. Screenshot get system interface physical
<img width="610" height="742" alt="ed0096c6-d45c-4160-b437-5cb7d0d5fe5c" src="https://github.com/user-attachments/assets/7c97fb20-1e6e-4c25-8c51-f34d4f1b36fa" />
2. Screenshot get router info routing-table all.
<img width="690" height="708" alt="8229a2b0-7d0e-493f-ac7b-645f24556e95" src="https://github.com/user-attachments/assets/7f747bc7-c42e-42e2-acd4-852ff418a376" />
3. Screenshot firewall policy.
<img width="1072" height="856" alt="5818df52-691a-42d4-9643-a9f8dd25c65b" src="https://github.com/user-attachments/assets/19efea7f-e51d-4e39-84e6-981ec2be39b5" />
4. Screenshot ping ke 8.8.8.8.
<img width="775" height="505" alt="75fe175f-8dd4-4d5a-bfbc-33c7a20cc6f4" src="https://github.com/user-attachments/assets/90ac558e-7fd5-487e-8d34-1dc8b42965d0" />
5. Screenshot ping ke IP tunnel Jakarta.
<img width="709" height="499" alt="bfb7060b-fb5c-4c95-84e6-e71a0e2bbdd1" src="https://github.com/user-attachments/assets/febdfffe-d405-4d70-9a31-d918f5b18ecd" />
6. Screenshot get router info ospf neighbor
<img width="712" height="502" alt="8083b7f0-be88-44f0-b6c9-9440fff0eb60" src="https://github.com/user-attachments/assets/58bd139e-e0a8-4267-8d0e-a54d16105ae5" />
7. Screenshot get router info routing-table ospf
<img width="718" height="499" alt="3735ddfa-30be-45a9-9ac4-0bfbad59a13b" src="https://github.com/user-attachments/assets/84add16a-ff6c-4610-81d2-d7c1d7695a31" />

**Tugas Modul 9 - Konfigurasi GRE Tunnel dan OSPF over GRE**
1. Screenshot ping WAN antar-FortiGate.
<img width="720" height="505" alt="271223e1-f7c7-49e1-a16d-4613f42208c7" src="https://github.com/user-attachments/assets/c9030f2f-786f-4a63-afd7-3d2fdcdcb9a9" />

2. Screenshot ping tunnel antar-FortiGate.
Fortigate sby Menembak IP Tunnel Jakarta
<img width="720" height="504" alt="c8f89135-4bd4-443f-ae2a-75daee5d140d" src="https://github.com/user-attachments/assets/a748200b-5ea0-42e9-b8ac-945cadd89026" />
fortigate jkt Menembak IP Tunnel Surabaya
<img width="714" height="502" alt="c1232c89-3039-4105-b6b6-331f743f7320" src="https://github.com/user-attachments/assets/5f6f96d9-62b0-4e2f-8ffb-a7dd5ba7555f" />

3. Screenshot get router info ospf neighbor
<img width="723" height="502" alt="277afa00-729e-4fbb-8404-fac3ad42a46f" src="https://github.com/user-attachments/assets/83614a68-d4ef-498f-90bd-92292759d844" />

4. Screenshot get router info routing-table ospf.
fortigate sby get router info routing-table ospf
<img width="714" height="514" alt="b1ef4b7d-0e68-4b8a-86a5-e79234a7da82" src="https://github.com/user-attachments/assets/ff3b1d33-9c15-4adc-b080-59dde63f2b91" />
fortigate jkt get router info routing-table ospf
<img width="717" height="495" alt="b72874c8-acc6-44d2-bc01-d5163190bc2b" src="https://github.com/user-attachments/assets/64122300-2d34-4f15-8f7f-89e2b045efce" />

5. Screenshot ping client Jakarta ke client Surabaya.
<img width="715" height="495" alt="d338bf5f-9861-4314-971e-8d594ad32700" src="https://github.com/user-attachments/assets/889dbb24-a5b0-4c0f-96d6-2950750043cb" />

6. Screenshot ping client Surabaya ke client Jakarta.
<img width="750" height="493" alt="d7158c51-ab10-4865-8c4a-e20d18986a04" src="https://github.com/user-attachments/assets/68b2ab17-fe5a-4af3-8919-5d09c8e55cc1" />

**Tugas Modul 10 - Pengujian Akhir**
1. Screenshot IP DHCP client Jakarta (Vlan 10).
<img width="718" height="502" alt="ada7d705-8268-4f5a-8e7b-f7e96619f210" src="https://github.com/user-attachments/assets/3477626b-de9c-4dbd-b5f6-a9f93395f50e" />

2. Screenshot IP DHCP client Surabaya (Vlan 20).
<img width="723" height="501" alt="82777189-3d8d-4211-8855-0510482fef5d" src="https://github.com/user-attachments/assets/1fbd49bf-ede4-408b-9a5c-66fd2d50d2e1" />

3. Screenshot ping internet dari Jakarta.
<img width="712" height="493" alt="55b70f32-3fea-49ef-ae84-c2967e4d1d59" src="https://github.com/user-attachments/assets/80b1e761-664a-4545-b293-4b110d7a4527" />

4. Screenshot ping internet dari Surabaya.
<img width="715" height="493" alt="e9a8bda4-fdcb-45b0-b471-dc48bf4d9d41" src="https://github.com/user-attachments/assets/994ac599-80a2-47fc-b9c5-e0fbbdd2b218" />

5. Screenshot ping antar-site (vlan 10 ke vlan 40)
<img width="706" height="489" alt="b0958c2e-c75d-45a1-9d27-5086bc39bbc5" src="https://github.com/user-attachments/assets/33df47f8-294d-4d6d-b441-a7e935856287" />

6. Screenshot akses web server Jakarta dari Surabaya.
<img width="709" height="498" alt="d6bc3202-7154-4811-8dac-1f87da095023" src="https://github.com/user-attachments/assets/610f851b-7140-4026-904c-7260acfbb350" />




















































