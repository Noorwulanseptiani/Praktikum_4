# Praktikum-4

## TUGAS PRAKTIKUM 4 (TABEL PEGAWAI)
1.	Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !
2.	Tampilkan pegawai yang tunjangannya NULL!
3.	Tampilkan pegawai yang tunjangannya tidak NULL!
4.	Tampilkan/hitung jumlah baris/record tabel pegawai!
5.	Tampilkan/hitung jumlah total gaji di tabel pegawai!
6.	Tampilkan/hitung rata-rata gaji pegawai!
7.	Tampilkan gaji terkecil!
8.	Tampilkan gaji terbesar!

PENJELASAN


### 1.	Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT * FROM pegawai WHERE gajih NOT IN (2000000, 1250000);`

Dan hasilnya akan seperti ini :

![wulan](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/faa3ee4c-8079-4861-992a-c6533f04c308)

### 2.	Tampilkan pegawai yang tunjangannya NULL!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT * FROM pegawai WHERE tunjangan IS NULL; `

Dan hasilnya akan seperti ini :

![wulan2](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/24d5e10b-1340-4e94-a7fb-80653aca9a9f)

### 3.	Tampilkan pegawai yang tunjangannya tidak NULL!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :
	
`SELECT * FROM pegawai WHERE tunjangan IS NOT NULL;`

Dan hasilnya akan seperti ini :

![wulan3](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/e59f8d5e-542f-49b9-8904-fefa14317e12)

## HASIL DARI 1 - 3

![wulan4](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/ed702d22-a4a2-46ca-9d84-81812fad9563)

### 4.	Tampilkan/hitung jumlah baris/record tabel pegawai!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT COUNT(*) AS jumlah_baris FROM pegawai;`

Dan hasilnya akan seperti ini :

![wulan5](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/0ecdb760-aa30-410f-8a50-01c2699a6b53)

### 5.	Tampilkan/hitung jumlah total gaji di tabel pegawai!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :


`SELECT SUM(gaji) AS total_gaji FROM pegawai; `

Dan hasilnya akan seperti ini :

![wulan6](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/afe95447-6ab8-4fbe-8d3f-282d1ca3bede)

### 6.	Tampilkan/hitung rata-rata gaji pegawai!

Jawab 

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT AVG(gaji) AS rata_gaji FROM pegawai`

Dan hasilnya akan seperti ini :

![wulan7](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/381491e0-758a-43d6-9878-3490b0e84e23)

### 7.	Tampilkan gaji terkecil!

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT MIN(gaji) AS gaji_terkecil FROM pegawai;`

Dan hasilnya akan seperti ini :

![wulan8](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/d318a907-ff31-4f88-8871-abd3d68d8c2c)

### 8.	Tampilkan gaji terbesar!

Jawab 

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT MAX(gaji) AS gaji_terbesar FROM pegawai;`

Dan hasilnya akan seperti ini :

![wulan9](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/14ff088a-601c-4a84-bcc0-5c854057ecf8)

## TUGAS PRAKTIKUM 4 (TABEL HEWAN)
1.	Tampilkan jumlah hewan yang dimiliki setiap owner
2.	Tampilkan jumlah hewan berdasarkan spesies
3.	Tampilkan jumlah hewan berdasarkan jenis kelamin
4.	Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin
5.	Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja) dan jenis kelamin
6.	Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja

PENJELASAN

### 1. Tampilkan jumlah hewan yang dimiliki setiap owner

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT owner, COUNT(*) AS Jumlah_hewan_setiap_owner FROM hewan GROUP BY owner; `

Dan hasilnya akan seperti ini :

![wulan10](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/f0b4ad95-4a3f-4fc4-bae4-223da5c1ca7e)

### 2.	Tampilkan jumlah hewan berdasarkan spesies

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT Species, COUNT(*) AS Jumlah_hewan_berdasarkan_Species FROM hewan GROUP BY Species; `

Dan hasilnya akan seperti ini :

![wulan11](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/f013f38f-df16-45ad-9592-35c4ce0784eb)

### 3.	Tampilkan jumlah hewan berdasarkan jenis kelamin

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

`SELECT sex, COUNT(*) AS Jumlah_hewan_berdasarkan_jenis_kelamin FROM hewan GROUP BY sex; `

Dan hasilnya akan seperti ini :

![wulan12](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/5c27035a-c9ca-4691-9404-44d2c81f6f11)

### 4.	Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

` SELECT species, sex, COUNT(*) AS jumlah FROM hewan GROUP BY species, sex;  `

Dan hasilnya akan seperti ini :

![wulan13](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/1e6e4bba-3f0b-43a1-a025-2a4cb4db447f)

### 5.	Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja) dan jenis kelamin

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

` SELECT species, sex, COUNT(*) AS jumlah FROM hewan WHERE species IN ('cat', 'dog') GROUP BY species, sex;  `

Dan hasilnya akan seperti ini :

![wulan14](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/30f3b141-9e74-4b30-8123-d857f24aaac7)

### 6.	Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja

Jawab :

Untuk perintahnya bisa menggunkan perintah seperti ini :

` SELECT sex, COUNT(*) AS jumlah FROM hewan GROUP BY sex;   `

Dan hasilnya akan seperti ini :

![wulan15](https://github.com/Noorwulanseptiani/Praktikum_4/assets/170961002/3237c513-b9c8-4471-9d42-c5aa832369d8)
