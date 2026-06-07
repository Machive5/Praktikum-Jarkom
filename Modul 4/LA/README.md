# Hasil Tugas Modul

Bagian ini memuat hasil dari pengerjaan tugas tambahan yang diberikan dalam modul praktikum serta penjelasan dari hasil konfigurasi yang sudah dilakukan.

## Topologi Jaringan

![Topologi jaringan pada PNETLab](topologi_pnetlab.jpeg)

## Konfigurasi MikroTik

![Konfigurasi IP address dan routing pada MikroTik](konfigurasi_mikrotik_ip_route.jpeg)

## Konfigurasi FortiGate

![Konfigurasi interface port1 pada FortiGate](konfigurasi_fortigate_port1_wan.jpeg)

## Konfigurasi Cisco Router

![Konfigurasi interface pada Cisco Router](konfigurasi_cisco_interface_brief.jpeg)

## Konfigurasi Web Server DMZ

![Konfigurasi halaman web server pada server DMZ](konfigurasi_web_server_dmz_index.jpeg)

## Hasil Pengujian

![Pengujian koneksi client LAN ke gateway LAN](hasil_ping_gateway_lan_192_168_10_1.jpeg)

![Pengujian koneksi Cisco Router ke FortiGate](hasil_ping_gateway_fortigate_lan_10_20_20_1.jpeg)

![Pengujian koneksi MikroTik ke FortiGate](hasil_ping_mikrotik_fortigate_10_10_10_2.jpeg)

![Pengujian koneksi client WAN ke gateway MikroTik](hasil_ping_client_wan_gateway_172_16_100_1.jpeg)

![Pengujian koneksi ke server DMZ](hasil_ping_dmz_192_168_20_10.jpeg)

![Hasil akses web server DMZ melalui alamat 192.168.20.10](hasil_web_dmz_via_192_168_20_10.jpeg)

![Hasil akses web server DMZ melalui VIP FortiGate](hasil_web_vip_via_10_10_10_2.jpeg)

Pada praktikum ini dilakukan konfigurasi jaringan menggunakan beberapa perangkat, yaitu MikroTik sebagai router ISP, FortiGate sebagai firewall utama, Cisco Router sebagai router internal, serta beberapa client pada jaringan LAN, WAN, dan DMZ.

Berdasarkan konfigurasi yang sudah dilakukan, jaringan berhasil dibagi menjadi beberapa segmen, yaitu WAN, LAN, dan DMZ dengan subnet yang berbeda. MikroTik digunakan sebagai router sisi ISP dan terhubung ke FortiGate melalui jaringan transit \texttt{10.10.10.0/30}. Selain itu, MikroTik juga digunakan sebagai gateway untuk client WAN.

FortiGate berperan sebagai firewall utama yang mengatur komunikasi antarjaringan menggunakan firewall policy. Jaringan LAN dapat mengakses jaringan WAN melalui NAT, sedangkan akses menuju DMZ diatur menggunakan policy khusus. Pada FortiGate juga dibuat konfigurasi VIP (Virtual IP) atau port forwarding agar layanan web pada server DMZ dapat diakses dari jaringan luar melalui alamat yang sudah ditentukan.

Hasil pengujian menunjukkan bahwa sebagian besar konektivitas antarperangkat berjalan dengan baik. Client LAN dapat terhubung ke gateway LAN, Cisco dapat terhubung ke FortiGate, MikroTik dapat terhubung ke FortiGate, dan FortiGate dapat mengakses server DMZ. Selain itu, halaman web pada server DMZ juga berhasil ditampilkan melalui browser.

Selama proses pengerjaan, terdapat beberapa kendala seperti kesalahan penulisan command, DHCP client MikroTik yang sempat belum mendapatkan IP, masalah login FortiGate, serta koneksi antarperangkat yang sempat tidak stabil. Kendala tersebut diselesaikan dengan mengecek ulang interface, IP address, routing, NAT, firewall policy, serta koneksi kabel pada topologi.

Berdasarkan hasil praktikum ini, dapat disimpulkan bahwa segmentasi jaringan menggunakan LAN, WAN, dan DMZ berhasil diterapkan. MikroTik, FortiGate, dan Cisco Router dapat dikonfigurasi untuk mendukung routing antarjaringan. NAT berhasil digunakan untuk akses keluar jaringan, sedangkan firewall policy pada FortiGate berhasil digunakan untuk mengontrol lalu lintas antarsegmen. Konfigurasi VIP juga berhasil digunakan untuk mengakses layanan web pada server DMZ. Secara keseluruhan, praktikum ini menunjukkan penerapan konsep routing, NAT, firewall, dan segmentasi jaringan dalam lingkungan simulasi PNETLab.

