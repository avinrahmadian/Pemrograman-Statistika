# 📖 **Pertemuan 1 : Pengantar Algoritma dan Pemrograman** 
## link Rpubs Syafiq: https://rpubs.com/syafiq/pengantaralgoritmadanpemrograman

## A. Apa itu Algoritma dan Pemrograman
Algoritma adalah urutan instruksi atau langkah-langkah logis untuk menyelesaikan suatu masalah. <br>
Program adalah kumpulan instruksi yang merupakan penyelesaian masalah dalam bahasa pemrograman tertentu. <br>
- 5 Ciri Penting Algoritma : <br>
1. Finiteness (Keterbatasan): Harus berakhir setelah sejumlah langkah. <br>
2. Definiteness (Kepastian): Setiap langkah harus jelas dan tidak bermakna ganda. <br>
3. Input (Masukan): Memiliki nol atau lebih data masukan. <br>
4. Output (Keluaran): Menghasilkan nol atau lebih hasil. <br>
5. Effectiveness (Efektivitas): Langkah-langkah harus efektif, wajar dan dapat dikerjakan. <br>

## B. Menggambarkan Algoritma
Untuk menuangkan ide penyelesaian masalah, terdapat beberapa notasi standar :
1. Pseudocode: Deskripsi algoritma yang menyerupai kode program tapi lebih mudah dibaca manusia. <br>
2. Flowchart (Diagram Alir): Representasi visual menggunakan simbol grafis untuk menunjukkan aliran proses dan logika keputusan. <br>
3. DFD (Data Flow Diagram): Fokus menggambarkan aliran data dari sistem, bukan kontrol atau logikanya. <br>

## C. Struktur Algoritma
Struktur algoritma terbagi kedalam 3 bagian yaitu:
1. Runtunan: instruksi sederhana berurutan (contoh: menghitung luas lingkaran). <br>
<div align="center" style="background-color:#0f1419; padding:12px; border-radius:8px; width:70%; margin:auto;">
  <img src="Image/Pertemuan 1/Runtunan.png" style="width:50%; max-width:40px;">
</div>
<div align="center" style="background-color:#0f1419; padding:12px; border-radius:8px; width:70%; margin:auto;">
  <img src="Image/Pertemuan 1/Runtunan 1.png" style="width:50%; max-width:40px;">
</div>

2. Pemilihan/percabangan: aksi hanya dijalankan jika syarat terpenuhi (if, if-else, case). <br>
3. Perulangan (loop): instruksi dengan pola yang sama secara berulang-ulang (for, while, repeat). <br>
- For : jika jumlah perulangan sudah diketahui
- While : jika jumlah perulangan tidak diketahui dan mungkin tidak pernah ada
- Repeat : jika jumlah perulangan tidak diketahui dan minimal sekali dilakukan

## D. Fungsi Dan Prosedur
## E. Teladan
- Misalkan akan dibuat algoritma kembalian uang dari suatu vending machine. Pecahan Uang yang tersedia pada mesin tersebut terdiri dari pecahan 10, 5, dan 1.
- Untuk keperluan ini, kita akan menggunakan diagram alir untuk algoritmanya. Asumsi dalam algoritma ini adalah pecahan 10, 5, dan 1 yang tersedia di vending machine tidak terbatas.
<div align="center" style="background-color:#0f1419; padding:12px; border-radius:8px; width:70%; margin:auto;">
  <img src="Image/Pertemuan 1/Teladan.png" style="width:50%; max-width:40px;">
</div>

```r
x <- 28 #sejumlah uang yang akan dipecah

# --- Bagian Pecahan 10 ---
i <- 0
y <- x - 10

while(y >= 0) {
  i <- i + 1
  x <- y
  y <- y - 10}

# --- Bagian Pecahan 5 ---
j <- 0
y <- x - 5

while(y >= 0) {
  j <- j + 1
  x <- y
  y <- y - 5}

# --- Bagian Pecahan 1 ---
k <- 0
y <- x - 1

while(y >= 0) {
  k <- k + 1
  x <- y
  y <- y - 1}

# --- Output ---
print(paste("Uang 10 sebanyak", i, "lembar"))
print(paste("Uang 5 sebanyak", j, "lembar"))
print(paste("Uang 1 sebanyak", k, "lembar"))
```


