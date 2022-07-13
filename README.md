# Finite Automata Text Search

## Deskripsi
Aplikas Finite Automata Text Search menggunakan mesin nondeterministik finite automata (NFA) dengan menerapkan extended transition function (delta topi). Dalam text search, penerapan konsep NFA (Non-deterministic Finite Automata) dapat digambarkan saat kita diberi satu set string yang akan disebut dengan kata kunci (keyword), kemudian NFA akan menemukan kemunculan kata-kata yang akan kita inputkan.<br/>
Dalam hal ini, selanjutnya akan dirancang NFA yang memberi sinyal dengan memasukkan kondisi penerimaan bahwa NFA telah melihat atau menemukan salah satu kata kunci tersebut. Akan diinputkan satu karakter pada satu waktu ke dalam NFA ini yang kemudian dapat mengenali kemunculan kata kunci (keyword) dalam teks ini.

Terdapat bentuk sederhana bagi sebuah NFA untuk dapat mengenali satu set string, diantaranya:
1. Terdapat state awal dengan transition ke dirinya sendiri pada setiap simbol yang diinputkan, setiap karakter ASCII yang dapat dicetak jika kita memeriksa teks. Secara intuitif, keadaan awal menunjukkan "tebakan" bahwa NFA belum mulai melihat salah satu kata kunci, bahkan jika NFA telah melihat beberapa huruf dari salah satu kata ini.
2. Untuk setiap kata kunci a1, a2…. ak, ada state k, anggap saja q1, q2…. qk. Terdapat transition dari state awal ke q1 pada simbol a1, transition dari q1 ke q2 pada simbol a2, dan seterusnya. State qk adalah final state dan menunjukkan bahwa kata kunci (keyword) a1, a2…. ak telah ditemukan.

Nondeterministic Finite Automata (NFA) didefenisikan sebagai 5 tuple yang merupakan sebuah koleksi dari 5 obyek (Q, Σ, δ, q0, F) dimana :
- Q adalah seperangkat status/state yang jumlahnya terbatas.
- Σ adalah seperangkat simbol terbatas yang disebut alfabet.
- δ adalah fungsi transisi di mana δ: Q × Σ → 2Q
- Q →(2Q) digunakan karena dalam kasus NDFA, dari suatu keadaan, transisi dapat terjadi pada kombinasi dari keadaan Q)
- q0 adalah keadaan awal dari mana input diproses (q0 ∈ Q).
- F adalah seperangkat status akhir / status Q (F ⊆ Q).4
- ε – NFA (epsilon Non – deterministic Finitie Automata)

## Fitur
- Beranda : Menampilkan halaman depan website yang berisikan tampilan untuk mencari teks yang diinginkan dan upload doc. Pada bagian ini dirancang menggukan slider dengan bootsrap untuk lebih membuat website interaktif.
- Cari : Fitur ini dapat digunakan untuk melakukan pecarian dokumen bahasa Bali. Pada f ield atau kolom pencarian te ks yang akan dicari bisa diinputkan atau dimasukkan banyak kata sesuai dengan keinginan user dan juga tidak terbatas untuk penggunaan dari spasi.
- Upload doc : Berfungsi untuk mengupload file bahasa bali yang akan dicari teks atau kata kunci yang diinginkan.
- Hasil : Pada fitur atau bagian hasil sendiri disini akan menampilkan dokumen-dokumen yang dicari katanya yang telah diinputkan pada fitur cari. Bagian terpenting pada fitur hasil adalah terdapat Time Consumed yang mana menyatakan waktu berapa lama waktu teks yang dicari. Pada fitur ini juga kata yang dicari juga dapat dibuka dokumennya secara langsung melewati fitur ini.
- Quintuple : Fitur ini digunakan untuk menampilkan quintuple dan fungsi transisi dari teks yang akan dicari.

## Implementasi

### Tampilan Awal (Home page)
<p align="center">
<img src="https://user-images.githubusercontent.com/72149133/178647723-2e605f86-1784-4ec1-987e-058ad7514555.png" style="width: 50%;">
</p>

### Tampilan Upload Doc (Mengupload Dokumen yang Dicari)
<p align="center">
<img src="https://user-images.githubusercontent.com/72149133/178647739-6f08da29-f4b7-46db-aa98-435c13a25c8e.png" style="width: 50%;">
</p>

### Tampilan Hasil Pencarian (Teks yang Dicari) 
<p align="center">
<img src="https://user-images.githubusercontent.com/72149133/178647753-bfab568f-772c-4cdd-b42a-8846b5e566e6.png" style="width: 50%;">
</p>

### Tampilan Quintuple
<p align="center">
<img src="https://user-images.githubusercontent.com/72149133/178647770-0f93c87d-213a-41b0-89f5-a8d4cc754398.png" style="width: 50%;">
</p>

### Tampilan Dokumen Ful Teks
<p align="center">
<img src="https://user-images.githubusercontent.com/72149133/178647778-1b85820a-b4d7-41f9-a1d0-0bc69d53f00d.png" style="width: 50%;">
</p>

### Tampilan My Files (Dokumen yang Sudah Diupload)
<p align="center">
<img src="https://user-images.githubusercontent.com/72149133/178647850-ca687d4b-cc1b-40c8-a5b4-d90b33ae1e1c.png">
</p>

## Pengujian
Disini aplikasi akan diuji dengan faktor waktu yang dibutuhkan apakah berbanding terbalik, berbanding lurus atau sebandingdengan banyaknya string atau kata yang di input dan dokumen yang diupload.
- Uji dengan banyaknya kata yang di input dengan kondisi jumlah dokumen yang sama, yaitu 50 dokumen.
  1. Pengujian testing waktu yang diperlukan menggunakan kata “pandemi”
     ![gambar](https://user-images.githubusercontent.com/72149133/178648829-b627b972-4f3b-46db-8e31-f7724457ad07.png)

  3. Pengujian testing waktu yang diperlukan menggunakan kata “pandemi covid”
     ![gambar](https://user-images.githubusercontent.com/72149133/178648854-eed36610-f45b-4e1b-b5af-4a54fe1d42f3.png)

  5. Pengujian testing waktu yang diperlukan menggunakan kata “pandemi covid-19”
     ![gambar](https://user-images.githubusercontent.com/72149133/178648877-14b1d230-ecfc-4d09-877c-f2d4b22a9169.png)
  
  Dengan ini kesimpulan yang diberikan adalah, banyaknya kata tidaklah berpengaruh pada penerapan pencarian teks pada mesin nfa menggunakan delta topi atau bisa dibilangwaktu yang dibutuhkan berbanding terbalik dengan banyaknya string atau kata pada inputan.
- Uji dengan jumlah dokumen yang di upload atau tersimpan dengan kondisi kata yang dicari adalah sama.
  1. Pada kondisi ini kata yang digunakan adalah kata “Pandemi” dengan dokumen yang di upload adalah 50 dokumen (doc1 – doc50)
     ![gambar](https://user-images.githubusercontent.com/72149133/178648910-8fc1dab3-7c3f-4b5f-a76d-8d58b9bffec2.png)

  3. Menambahkan 20 dokumen. Total 70 dokumen (doc1 – doc70)
     ![gambar](https://user-images.githubusercontent.com/72149133/178648932-c000e7ee-c425-49b1-91a5-6bb0db63ec1e.png)

  5. Menambahkan 20 dokumen . Total 90 dokumen (doc1 – doc90)
     ![gambar](https://user-images.githubusercontent.com/72149133/178648957-f2f8271d-04ee-4228-aca2-3af51b4b042d.png)
  
  Dengan ini kesimpulan yang diberikan adalah, banyaknya dokumen pada aplikasi yang diuji sangatlah berpengaruh pada waktu yang dibutuhkan dalam mencari seuatu teks atau string yang diberikan atau berbanding lurus dengan waktu yang dibutuhkan.

## Kesimpulan
Aplikasi Pencarian Teks Finite Automata menggunakan mesin Non-deterministic Finite Automata (NFA) merupakan aplikasi berbasis web yang mana dapat mencari teks kata (kata kunci sesuai keinginan user) dari sebuah teks file yang sudah diupload sebelumnya yang mana berekstensi .txt. Fitur-fitur yang disediakan juga tidak memiliki makna ganda dan memiliki fungsinya masing-masing. Semakin banyak dokumen yang ada didalam database akan mempengaruhi waktu yang dibutuhkan sistem untuk mencari dokumen-dokumen yang sesuai dengan kata kunci yang dimasukkan oleh user. Dan juga cepat lambatnya pencarian teks dalam dokumen tergantung juga pada posisi kata kunci yang dicari di dalam sebuah dokumen.
