# Laporan Praktikum 2

## KASUS 1 : PROGRAM PEMESANAN TIKET BIOSKOP
Repository ini berisi program Python sederhana untuk menghitung harga tiket bioskop. Program ini memperhitungkan jenis tiket (Reguler atau VIP) dan memberikan diskon 20% untuk pengguna yang memiliki kartu member.

### Deskripsi Program
Program pemesanan tiket bioskop ini bertujuan untuk menghitung total harga tiket berdasarkan pilihan pengguna:
Tiket Reguler seharga Rp50.000
Tiket VIP seharga Rp100.000
Pengguna dengan kartu member mendapatkan diskon sebesar 20%.
Program akan meminta pengguna untuk memasukkan:

Tipe tiket (Reguler atau VIP).
Status member (Ya atau Tidak).
Kemudian, program akan menampilkan total harga yang harus dibayar.

### Algoritma
Berikut langkah-langkah dari algoritma program ini:

Program meminta pengguna untuk memilih tipe tiket: Reguler atau VIP.

Program meminta pengguna untuk mengonfirmasi apakah mereka memiliki kartu member.

Berdasarkan tipe tiket, program menetapkan harga awal.

Jika pengguna memiliki kartu member, program mengurangi harga dengan diskon sebesar 20%.

Program menampilkan total harga yang harus dibayar.
```phython
# Program menghitung harga tiket bioskop

# Harga tiket
harga_reguler = 50000
harga_vip = 100000
diskon_member = 0.20

# Meminta input dari user
tipe_tiket = input("Masukkan tipe tiket (reguler/vip): ").strip().lower()
status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ").strip().lower()

# Menentukan harga tiket sesuai tipe
if tipe_tiket == "reguler":
    harga_tiket = harga_reguler
elif tipe_tiket == "vip":
    harga_tiket = harga_vip
else:
    print("Tipe tiket tidak valid.")
    exit()

# Menghitung total harga dengan diskon jika user adalah member
if status_member == "ya":
    total_harga = harga_tiket * (1 - diskon_member)
else:
    total_harga = harga_tiket

# Menampilkan total harga yang harus dibayar
print(f"Total harga yang harus dibayar: Rp{total_harga:,}")

# Tampilkan hasil
if total_harga > 0:
    print(f"Total harga yang harus dibayar: Rp{harga_final:.2f}")

 
```
# KASUS 2 : KALKULATOR SEDERHANA
Repository ini juga mencakup program Kalkulator Sederhana yang dapat melakukan operasi aritmatika dasar. Program ini memungkinkan pengguna untuk memasukkan dua angka dan memilih jenis operasi (penjumlahan, pengurangan, perkalian, atau pembagian) yang akan diterapkan pada kedua angka tersebut.

Deskripsi Program
Kalkulator ini mendukung empat operasi aritmatika:

1.Penjumlahan (+)

2.Pengurangan (-)

3.Perkalian (*)

4.Pembagian (/)

Pengguna akan diminta untuk memasukkan dua angka dan operator aritmatika. Program kemudian akan menampilkan hasil dari operasi yang dipilih. Program ini juga menangani pembagian dengan nol dan akan memberikan pesan peringatan jika pembagian tidak bisa dilakukan.

Algoritma
Berikut langkah-langkah dari algoritma program kalkulator sederhana ini:

Program meminta pengguna untuk memasukkan angka pertama.

Program meminta pengguna untuk memasukkan operator aritmatika yang ingin digunakan (+, -, *, atau /).

Program meminta pengguna untuk memasukkan angka kedua.

Berdasarkan operator yang dimasukkan, program melakukan operasi aritmatika pada kedua angka.

Jika operasi adalah pembagian dan angka kedua adalah nol, program menampilkan pesan bahwa pembagian dengan nol tidak dapat dilakukan.

Program menampilkan hasil dari operasi yang dipilih atau pesan error jika operator tidak valid.

```phython
# Program Kalkulator Sederhana

# Meminta input dari pengguna
angka1 = float(input("Masukkan angka pertama: "))
operator = input("Masukkan operator (+, -, *, /): ").strip()
angka2 = float(input("Masukkan angka kedua: "))

# Menghitung hasil berdasarkan operator yang dipilih
if operator == "+":
    hasil = angka1 + angka2
elif operator == "-":
    hasil = angka1 - angka2
elif operator == "*":
    hasil = angka1 * angka2
elif operator == "/":
    if angka2 != 0:  # Menghindari pembagian dengan nol
        hasil = angka1 / angka2
    else:
        print("Error: Pembagian dengan nol tidak diperbolehkan.")
        exit()
else:
    print("Operator tidak valid.")
    exit()

# Menampilkan hasil
print(f"Hasil: {angka1} {operator} {angka2} = {hasil}")
```
## Flowchart
### Hasil Flowchart pesanan tiket bioskop
* "Yang asli cuman ada di pradyafatah"(https://drive.google.com/file/d/15mYmxXqmwoB1qGuOk2jHpTqvAMNGzBH8/view?usp=drive_link)
### Hasil dari flowchart kalkulator sederhana
* "Yang asli cuman ada di pradyafatah"(https://drive.google.com/file/d/1kp5YjJrerHzJ7BAugxo4Qfc0Ps4fzFWP/view?usp=drive_link)

## Screenshot Hasil Eksekusi Program
### Pembelian tiket bioskop

(![Cuplikan layar 2024-10-28 152255](https://github.com/user-attachments/assets/ed2a0669-a8aa-41ec-ab2c-b2f96da7edae)
)
#### Hasil

(![Cuplikan layar 2024-10-28 152530](https://github.com/user-attachments/assets/1032c18b-75c2-40d1-8384-963b1ad21df2)
)
## Kalkulator sederhana

(![Cuplikan layar 2024-10-28 152642](https://github.com/user-attachments/assets/aa1e1b24-41cb-465b-b0bc-693e1d5ca7d5)
)
#### Hasil

(![image](![Cuplikan layar 2024-10-28 152908](https://github.com/user-attachments/assets/5ca92658-94ba-4441-9062-2e4bb452af92)
)
## Kesimpulan dari Tugas Pemrograman
Program Pemesanan Tiket Bioskop:

Program ini dirancang untuk menghitung total harga tiket bioskop berdasarkan tipe tiket (reguler atau VIP) dan status keanggotaan pengguna (member atau non-member).
Dengan menggunakan struktur kontrol if-else, program dapat menentukan harga tiket dan menerapkan diskon jika pengguna adalah member.
Flowchart yang dibuat memberikan gambaran visual yang jelas tentang alur logika program, memudahkan pemahaman proses yang terjadi.
Program Kalkulator Sederhana:

Program ini menerima dua angka dan operator aritmatika, kemudian melakukan perhitungan sesuai dengan operator yang dipilih oleh pengguna.
Struktur if-elif-else digunakan untuk menentukan operasi yang akan dilakukan berdasarkan input pengguna.
Flowchart berfungsi untuk menjelaskan langkah-langkah dalam proses kalkulasi, dari pengambilan input hingga pengeluaran hasil.
### Manfaat:
Visualisasi: Flowchart membantu dalam memahami logika program secara keseluruhan, menjadikan debugging dan pengembangan lebih mudah.

Penguasaan Logika Pemrograman: Tugas ini memperkuat pemahaman mengenai penggunaan struktur kontrol, input/output, serta perhitungan matematis dalam pemrograman.

Penerapan Algoritma: Mengasah keterampilan dalam merancang algoritma yang efisien dan mudah dipahami, serta menerjemahkannya ke dalam kode.
### Langkah Selanjutnya:
Melakukan pengujian lebih lanjut untuk memastikan keandalan dan ketahanan program.
Menerapkan fitur tambahan, seperti pemilihan waktu tayang dan jumlah tiket untuk program pemesanan tiket.
Menambahkan lebih banyak operator atau fungsi dalam kalkulator sederhana untuk meningkatkan fungsionalitasnya.
Dengan menyelesaikan tugas ini, pengguna tidak hanya mendapatkan keterampilan teknis dalam pemrograman Python tetapi juga belajar cara merancang dan memahami algoritma serta alur program dengan lebih baik.

(Terimakasih :)
