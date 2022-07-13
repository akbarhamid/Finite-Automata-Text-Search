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
![Tampilan Awal (Home page)](https://user-images.githubusercontent.com/72149133/178647723-2e605f86-1784-4ec1-987e-058ad7514555.png)

### Tampilan Upload Doc (Mengupload Dokumen yang Dicari)
![Tampilan Upload Doc (Mengupload Dokumen yang Dicari)](https://user-images.githubusercontent.com/72149133/178647739-6f08da29-f4b7-46db-aa98-435c13a25c8e.png)


### Tampilan Hasil Pencarian (Teks yang Dicari) 
![Tampilan Hasil Pencarian (Teks yang Dicari)](https://user-images.githubusercontent.com/72149133/178647753-bfab568f-772c-4cdd-b42a-8846b5e566e6.png)


### Tampilan Quintuple
![Tampilan Quintuple](https://user-images.githubusercontent.com/72149133/178647770-0f93c87d-213a-41b0-89f5-a8d4cc754398.png)


### Tampilan Dokumen Ful Teks
<img width="960" alt="Tampilan Dokumen Ful Teks" src="https://user-images.githubusercontent.com/72149133/178647778-1b85820a-b4d7-41f9-a1d0-0bc69d53f00d.png">


### Tampilan My Files (Dokumen yang Sudah Diupload)
![gambar](https://user-images.githubusercontent.com/72149133/178647850-ca687d4b-cc1b-40c8-a5b4-d90b33ae1e1c.png)




## Pengujian


## Kesimpulan
