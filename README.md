# Tugas ke-4 Organisasi & Arsitektur Komputer

## 1. Jeelaskan Struktur Antar Hubungan dan Berikan Contohnya?
   - Struktur antar hubungan bisa disebut sebagai sistem Bus. Bus adalah suatu jalur penghubung antar perangkat pada komputer, bus ini digunakan sebagai media dalam proses melewatkan data pada suatu proses. Jadi bisa disimpulkan bahwa sistem bus adalah penghubung bagi keseluruhan komponen komputer dalam menjalankan tugasnya. Data atau program yang tersimpan dalam memori dapat diakses dan dieksekusi CPU melalui perantara bus,
     - Contohnya : 
       1. PCI (Peripheral Component Interconnect), adalah standar bus komputer yang memfasilitasi koneksi perangkat keras ke motherboard komputer. bus ini tidak tergantung pada prosesor yang dimiliki, berbandwith tinggi serta berfungsi sebagai bus mezzanine atau bus peripheral. Standar PCI adalah 64 saluran data pada kecepatan 33MHz, laju     transfer data 263 MB per detik atau 2,112 Gbps. Bus PCI ini memiliki kinerja yang tinggi dalam menyediakan sistem yang lebih baik bagi subsistem I/O berkecepatan tinggi, seperti : graphic display adapter, network interface controller, dan disc controller.
       2. Bus USB (Universal Serial Bus), USB merupakan suatu teknologi yang memungkinkan kita untuk menghubungkan alat eksternal (peripheral) seperti scanner, printer, mouse, papan ketik (keyboard), alat penyimpan data (zip drive), flash disk, kamera digital atau perangkat lainnya ke komputer kita. USB sangat mendukung transfer data sebesar 12 Mbps ( juta bit per detik). Semua perangkat peripheral tidak efektif apabila dipasang pada bus kecepatan tinggi PCI, sedangkan banyak peralatan yang memiliki kecepatan rendah maka itu merancang bus untuk peralatan I/O berkecepatan rendah, yang dinamakan USB. Keuntungan dari penerapan USB yaitu, Dapat mensuplai daya pada peralatan-peralatan I/O, hanya satu jenis kabel yang diperlukan sebagai penghubung, harga yang murah, dan memudahkan pemasangan peralatan-peralatan yang hanya sementara dipasang padakomputer.
       3. Bus ISA (Industry Standard Architecture), Bus ISA adalah bus komputer yang memungkinkan kartu ekspansi tambahan terhubung ke motherboard komputer, arsitektur bus standar untuk kompatibel IBM. bus ISA yang pada dasarnya adalah bus PC/AT yang beroperasi pada 8,33 MHz. Keuntungannya menggunakan bus ini adalah tetap mempertahankan kompatibiitas dengan mesin-mesin dan kartu-kartu yang ada. Setiap PC yang berbasiskan Intel masih menggunakan bus jenis ini, meskipun biasanya juga disertai dengan satu atau lebih bus lain.

## 2. Bila terlalu banyak modul atau perangkat dihubungkan pada bus maka akan terjadi penurunan kinerja, sebutkan penyebabnya?
Ketika beberapa perangkat mencoba berkomunikasi melalui bus secara bersamaan, dapat terjadi konflik karena bus hanya dapat melayani satu perangkat pada satu waktu. Hal ini menyebabkan perangkat lain harus menunggu giliran yang menyebabkan penundaan dan penurunan kinerja. 
Penyebab lainnya yaitu :
1) Antrian penggunaan bus semakin panjang, Hal ini sama seperti memperlambat data jika banyak banyaknya penggunaan bus maka data juga lambat data mentransfer.
2) Semakin besar delay propagasi untuk mengkoordinasikan penggunaan bus.
3) Kemungkinan Habisnya Kapasitas Transfer Bus, Jika terlalu banyak perangkat yang menggunakan bus secara bersamaan, kapasitas transfer bus dapat habis, yang memperlambat transfer data.

## 3. Umumnya perangkat berprioritas paling rendah memiliki waktu tunggu rata-rata yang paling singkat. Dengan dasar ini biasanya CPU diberi perioritas tertinggi pada SBI. Sebutkan alasan perangkat berprioritas 16 memiliki waktu tunggu rata-rata paling rendah? Dibawah kondisi seperti apa keadaan diatas tidak berlaku?
   
  Perangkat dengan prioritas 16 memiliki waktu tunggu rata-rata paling rendah karena dalam sistem penjadwalan multilevel queue atau priority scheduling, perangkat dengan prioritas lebih rendah cenderung lebih cepat diproses karena tugasnya biasanya lebih ringan atau lebih cepat dieksekusi dibandingkan perangkat dengan prioritas lebih tinggi. CPU sering kali diberi prioritas tertinggi dalam Sistem Basis Input (SBI) karena perannya yang krusial dalam menjalankan instruksi program dan mengoordinasikan operasi sistem. Namun, kondisi ini tidak selalu berlaku.
  
  
  Ada beberapa situasi di mana perangkat dengan prioritas lebih rendah tidak memiliki waktu tunggu rata-rata yang lebih singkat, misalnya:  Beban Kerja Tidak Merata, Sistem dengan Preemptive Scheduling, Ketergantungan Antar Proses, Interrupt dan I/O Blocking. Jadi, meskipun dalam kondisi normal perangkat berprioritas lebih rendah memiliki waktu tunggu rata-rata lebih singkat, ada banyak faktor yang bisa mempengaruhi skenario ini tergantung pada bagaimana sistem penjadwalan dan beban kerja dikonfigurasi.

## Jawaban tereferensi dari sumber:
1. http://sistembus.blogspot.com/2015/12/sistem-bus.html
2. http://tecnomasi.blogspot.com/2015/12/jawaban-organisasi-arsitektur-komputer.html
