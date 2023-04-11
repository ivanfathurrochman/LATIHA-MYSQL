# LATIHAN-MYSQL
# 1. Membuat database latihan2:
# MENAMPILKAN DAFTAR BASIS DATA
CREATE DATABASE latihan2;
![image](https://user-images.githubusercontent.com/115911604/231225213-567742c6-9e0f-4061-a86f-450f4950e390.png)

# MENAMPILKAN DAFTAR BASIS DATA
![image](https://user-images.githubusercontent.com/115911604/231226946-ee3a9fb5-1767-44ba-a63a-14fa99c5716e.png)

# 2. Membuat tabel biodata di dalam database latihan2:
USE latihan2; CREATE TABLE biodata (nama VARCHAR(15),alamat VARCHAR(15));
![image](https://user-images.githubusercontent.com/115911604/231227242-2489da4e-2352-4f17-975e-c8ad7c346c1c.png)
# 3. Menambahkan kolom keterangan:
ALTER TABLE biodata ADD keterangan VARCHAR(15);
![image](https://user-images.githubusercontent.com/115911604/231227428-430ec28b-6261-4e56-8adb-1c024530779a.png)
# 4. Menambahkan kolom id di awal:
ALTER TABLE biodata ADD id INT(11) FIRST;

![image](https://user-images.githubusercontent.com/115911604/231227645-5936de43-53b8-462f-a215-ce03b4e17807.png)
# 5. Menambahkan kolom phone setelah kolom alamat:
ALTER TABLE biodata ADD phone VARCHAR(15) AFTER alamat;
![image](https://user-images.githubusercontent.com/115911604/231227883-dfae5ee0-9d3a-4b7f-afaa-f354b12f7472.png)
# 6. Mengubah tipe data kolom id menjadi char(11)
ALTER TABLE biodata MODIFY id CHAR(11);

![image](https://user-images.githubusercontent.com/115911604/231228038-f1c680a4-316c-4863-9ca5-0a6a891968df.png)

# 7. Mengubah nama kolom phone menjadi hp (varchar 20):
ALTER TABLE biodata CHANGE phone hp VARCHAR(20);
![image](https://user-images.githubusercontent.com/115911604/231228182-9e9d9906-cb25-496c-86a8-975009e94905.png)
# 8. Menambahkan kolom email setelah kolom hp:
ALTER TABLE biodata ADD email VARCHAR(15) AFTER hp;
![image](https://user-images.githubusercontent.com/115911604/231228615-7aa01cc6-6f23-4844-9909-22c7a3e54b98.png)
# 9 . Menghapus kolom keterangan:
ALTER TABLE biodata DROP COLUMN keterangan;
![image](https://user-images.githubusercontent.com/115911604/231228699-e1598dc9-f2cd-48b3-8365-bcd0c5de7900.png)
# 10. Mengganti nama tabel menjadi data_mahasiswa:
ALTER TABLE biodata RENAME TO data_mahasiswa;
![image](https://user-images.githubusercontent.com/115911604/231228814-33e2deee-8b5a-4e1d-8530-b94006b64cd9.png)
# 11. Mengganti nama field id menjadi nim:
LTER TABLE data_mahasiswa CHANGE id nim CHAR(11);
![image](https://user-images.githubusercontent.com/115911604/231229460-fd9526b5-80e5-4503-ac98-f2c665a9866f.png)
# 12 .Menjadikan nim sebagai PRIMARY KEY:
ALTER TABLE data_mahasiswa ADD PRIMARY KEY (nim);
![image](https://user-images.githubusercontent.com/115911604/231228992-65dcfcbf-3e38-480d-8074-d5cb5385a785.png)
# 13. Menjadikan kolom email sebagai UNIQUE KEY:
ALTER TABLE data_mahasiswa ADD UNIQUE KEY (email);
![image](https://user-images.githubusercontent.com/115911604/231229607-0eeba32f-0fdc-4530-8271-d890c3a626a6.png)
#








# 1. MEMBUAT DATABASE LATIHAN 1
![image](https://user-images.githubusercontent.com/115911604/231231472-da5465c0-7fce-4d66-a16d-dd279e84f919.png)
# 2. Membuat Tabel
CREATE TABLE siswa (nama VARCHAR(100),alamat TEXT);
![image](https://user-images.githubusercontent.com/115911604/231231511-6a3e62f6-299b-42be-be08-72534245cd89.png)
# 3. Menambahkan Kolom Di Awal
ALTER TABLE siswa ADD COLUMN id INT FIRST;

![image](https://user-images.githubusercontent.com/115911604/231231560-3890e327-3db3-4a5d-9874-aa9f598951b9.png)
# 4. Mengubah Nama Kolom
ALTER TABLE siswa CHANGE keterangan kelas VARCHAR(10);

![image](https://user-images.githubusercontent.com/115911604/231231618-2d2805dd-71d6-42f6-b2f0-ffde2bfee778.png)
# 5. Mengubah Tipe Data
VARCHAR(10) menjadi VARCHAR(11)

![image](https://user-images.githubusercontent.com/115911604/231232253-8201c9ef-4204-45d0-91f1-33b7214fd0c6.png)
# 6. Menghapus Kolom
ALTER TABLE siswa DROP COLUMN kelas;

![image](https://user-images.githubusercontent.com/115911604/231232281-98b521de-976f-4cd5-bcfc-2768a15ee6c6.png)
# 7. Menambahkan Primary Key Id
ALTER TABLE siswa ADD PRIMARY KEY(id);

![image](https://user-images.githubusercontent.com/115911604/231232306-e52912a4-c99f-4cb9-b27b-a2b6a141531f.png)
# 8. Menghapus Primary Key
ALTER TABLE siswa DROP PRIMARY KEY;

![image](https://user-images.githubusercontent.com/115911604/231232381-1b26d22f-4930-49a7-a30a-576c73073287.png)
# 9. Menambahkan Constraint
ALTER TABLE siswa ADD CONSTRAINT PK_siswa PRIMARY KEY(id);

![image](https://user-images.githubusercontent.com/115911604/231232381-1b26d22f-4930-49a7-a30a-576c73073287.png)

# 10. Menghapus Constraint Primary Key juga Bisa Seperti Ini:
ALTER TABLE siswa DROP PRIMARY KEY;

![image](https://user-images.githubusercontent.com/115911604/231232484-5f7e09da-2f90-4f73-970f-1d9ed3629e5d.png)
#
