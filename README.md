# Tugas_15_MySQL

### Kerjakan tugas berikut dengan menggunakan PHPMyadmin!
### 1. Buatlah database dengan nama niomic!
![DBNiomic](DBNiomic.PNG)

### 2. Perhatikan gambar dibawah ini:
![34Provinsi](34Provinsi.PNG)
### a. Buatlah tabel dengan nama demography dengan jumlah 6 kolom sesuai dengan gambar diatas. Teman-teman bebas untuk berkreasi tentang tipe data dan ukuran kolom.
![TabelDemography](TabelDemography.PNG)

![StrukturTabel](StrukturTabel.PNG)

### b. Masukan 34 data sesuai dengan gambar tersebut.
```mysql
INSERT INTO demography (kodeBPS, nama, ibukota, populasi, luas, pulau) VALUES
(11, 'Aceh', 'Banda Aceh',4494410, 56500.51, 'Sumatera'),
(12, 'Sumatera Utara', 'Medan',12982204, 72427.81, 'Sumatera'),
(13, 'Sumatera Barat', 'Padang',4846909, 42224.65, 'Sumatera'),
(14, 'Riau', 'Pekanbaru',5538367, 87844.23, 'Sumatera'),
(15, 'Jambi', 'Jambi',3092265, 45348.49, 'Sumatera'),
(16, 'Sumatera Selatan', 'Palembang',7450394, 60302.54, 'Sumatera'),
(17, 'Bengkulu', 'Bengkulu',1715518, 19795.15, 'Sumatera'),
(18, 'Lampung', 'Bandar Lampung',7608405, 37735.15, 'Sumatera'),
(19, 'Kepulauan Bangka Belitung', 'Pangkal Pinang',1223296, 16424.14, 'Sumatera'),
(21, 'Kepulauan Riau', 'Tanjung Pinang',1679163, 8084.01, 'Sumatera'),
(31, 'Daerah Khusus Ibukota Jakarta', 'Jakarta Pusat',9607787, 740.29, 'Jawa'),
(32, 'Jawa Barat', 'Bandung',43053732, 36925.05, 'Jawa'),
(33, 'Jawa Tengah', 'Semarang',32382657, 32799.71, 'Jawa'),
(34, 'Daerah Istimewa Yogyakarta', 'Yogyakarta',3457491, 3133.15, 'Jawa'),
(35, 'Jawa Timur', 'Surabaya',37476757, 46689.64, 'Jawa'),
(36, 'Banten', 'Serang',10632166, 9018.64, 'Jawa'),
(51, 'Bali', 'Denpasar',3890757, 5449.37, 'Nusa Tenggara'),
(52, 'Nusa Tenggara Barat', 'Mataram',4500212, 19708.79, 'Nusa Tenggara'),
(53, 'Nusa Tenggara Timur', 'Kupang',4683827, 46137.87, 'Nusa Tenggara'),
(61, 'Kalimantan Barat', 'Pontianak',4395983, 120114.32, 'Kalimantan'),
(62, 'Kalimantan Tengah', 'Palangkaraya',2212089, 153564.50, 'Kalimantan'),
(63, 'Kalimantan Selatan', 'Banjarmasin',3626616, 37530.52, 'Kalimantan'),
(64, 'Kalimantan Timur', 'Samarinda',3553143, 194849.08, 'Kalimantan'),
(65, 'Kalimantan Utara', 'Tanjung Selor',738163, 72567.49, 'Kalimantan'),
(71, 'Sulawesi Utara', 'Manado',2270596, 13930.73, 'Sulawesi')
```

![Nomor2a](Nomor2a.PNG)

![isiTabel2a](isiTabel2a.PNG)


### c. Kemudian hapus data dengan ketentuan pulau = Nusa Tenggara dan Kalimantan.
```mysql
DELETE FROM demography
WHERE pulau LIKE 'Nusa Tenggara' OR pulau LIKE 'Kalimantan'
```

![Nomor2b](Nomor2b.PNG)

![isiTabel2b](isiTabel2b.PNG)

### d. Tampilkan kolom nama, ibukota, populasi dan luas dari tabel demography berdasarkan urutan nama secara alphabet.
```mysql
SELECT nama, ibukota, populasi, luas FROM demography
ORDER BY nama ASC;
```

![Nomor2c](Nomor2c.PNG)
