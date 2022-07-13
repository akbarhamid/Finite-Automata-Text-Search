# Finite Automata Text Search

## Deskripsi
Aplikas Finite Automata Text Search menggunakan mesin nondeterministik finite automata (NFA) dengan menerapkan extended transition function (delta topi). Dalam text search, penerapan konsep NFA (Non-deterministic Finite Automata) dapat digambarkan saat kita diberi satu set string yang akan disebut dengan kata kunci (keyword), kemudian NFA akan menemukan kemunculan kata-kata yang akan kita inputkan.<br/>
Dalam hal ini, selanjutnya akan dirancang NFA yang memberi sinyal dengan memasukkan kondisi penerimaan bahwa NFA telah melihat atau menemukan salah satu kata kunci tersebut. Akan diinputkan satu karakter pada satu waktu ke dalam NFA ini yang kemudian dapat mengenali kemunculan kata kunci (keyword) dalam teks ini.<br/>
Terdapat bentuk sederhana bagi sebuah NFA untuk dapat mengenali satu set string, diantaranya:
1. Terdapat state awal dengan transition ke dirinya sendiri pada setiap simbol yang diinputkan, setiap karakter ASCII yang dapat dicetak jika kita memeriksa teks. Secara intuitif, keadaan awal menunjukkan "tebakan" bahwa NFA belum mulai melihat salah satu kata kunci, bahkan jika NFA telah melihat beberapa huruf dari salah satu kata ini.<br/>
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
