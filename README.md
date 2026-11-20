# Tugas_Besar_STD_Kelompok_J_Reseller.in
# Pengadaan produk (Reseller.in)

## Deskripsi
Aplikasi pengelolaan pengadaan produk mencatat reseller dan pemasok yang menjalin hubungan pemasokan. Seorang reseller dapat memperoleh produk dari beberapa pemasok dan satu pemasok dapat memasok banyak reseller. Setiap hubungan pemasokan dapat menghasilkan beberapa transaksi pengadaan. Data hubungan pemasok dikelola melalui Multi Linked List, sedangkan transaksi pengadaan dicatat dalam Binary Search Tree.
---

## Struktur Data

| List | Deskripsi |
|----------|--------|
| Reseller | Reseller (id reseller, nama, kontak) |
| Pemasok | Pemasok (id pemasok,namaperusahaan, kontak) |
| KerjaSamaPemasokan | Kerja Sama Pemasokan (tanggal mulai kerja sama, jenis produk yang dipasok, Stok, harga modal, ketentuan pembayaran) |
| Binary Search Tree | Transaksi pengadaan dengan key nomor PO (id reseller, id pemasok, nama produk, jumlah barang, total biaya, tanggal pengadaan, status pengadaan) |

---

## Fitur / Fungsional Program
### Fungsional Umum
Fungsionalitas yang harus terpenuhi untuk **Multi-Linked list** adalah 
1. Menyisipkan elemen Reseller, Pemasok dan KerjaSamaPemasokan (first, last, after)
2. Menghapus elemen Reseller, Pemasok dan KerjaSamaPemasokan (first, last, after)
3. Mencari elemen Reseller, Pemasok dan KerjaSamaPemasokan
4. Menampilkan seluruh data pada list (Reseller, Pemasok dan KerjaSamaPemasokan)
5. Membuat data dummy untuk masing-masing list minimal 5 data (Reseller, Pemasok) dan 10 data (KerjaSamaPemasokan)
6. Main Program (interface) 

Fungsionalitas yang harus terpenuhi untuk **Binary Search tree** adalah 
1. Menyisipkan node berisikan Transaksi pengadaan berdasarkan nomor PO
2. Menghapus node berisikan Transaksi pengadaan berdasarkan nomor PO 
3. Mencari node berisikan Transaksi pengadaan berdasarkan nomor PO
4. Menampilkan seluruh data secara traversal (in-order, pre-order, dan post-order).
5. Menampilkan nilai minimum, maksimum, tinggi pohon, dan jumlah node .
5. Membuat data dummy untuk BST minimal 10 node berisikan Transaksi pengadaan.
6. Melengkapi Main Program (interface)

### Fungsional khusus
1. Melakukan transaksi pengadaan dengan memilih reseller dan pemasok yang tersedia serta memperbaharui stok jika transaksi pengadaan berhasil.
2. Menyimpan transaksi pembelian ke BST berdasarkan nomor Pre-Order (Unik dan acak).
3. Menampilkan informasi reseller dengan pengadaan terbanyak serta total pengeluarannya.
4. Menampilkan total pendapatan aplikasi jika fee aplikasi sebesar 5% dari setiap pengadaan..

### Fungsional tambahan (Bonus)
Fungsionalitas / studi kasus bonus yang dipilih dari topik ini adalah
1. Menampilkan informasi pemasok dengan jumlah pengadaan terbanyak.
2. Menampilkan informasi produk dengan jumlah pengadaan terbanyak.
3. Menampilkan riwayat pengadaan berdasarkan pemasok atau reseller.

---

## Struktur Folder
```bash
├── Tugas-Besar-Kelompok_10
│   ResellerIn
│   │   interface.cpp
│   │   interface.h
│   │   main.cpp
│   │   Resellerin.cbp
│   │   Resellerin.layout
│   │
│   ├───Bonus
│   │   ├───header
│   │   │       bonus.h
│   │   │
│   │   └───implementation
│   │           bonus.cpp
│   │
│   ├───BST
│   │   ├───header 
│   │   │       nilaiBST.h
│   │   │
│   │   └───implementation
│   │           nilaiBST_[103012500113_anggota_1].cpp
│   │           nilaiBST_[103012500008_angggota_2].cpp
│   │
│   ├───Khusus
│   │   ├───header
│   │   │       khusus.h
│   │   │
│   │   └───implementation
│   │           khusus.cpp
│   │
│   └───MLL-02
│       ├───header
│       │       Reseller.h
│       │       KerjaSamaPemasokan.h
│       │       Pemasok.h
│       │
│       └───implementation
│           ├───Reseller
│           │       Reseller_[103012500113_anggota_1].cpp
│           │       Reseller_[103012500008_angggota_2].cpp
│           │
│           ├───KerjaSamaPemasokan
│           │       KerjaSamaPemasokan_[103012500113_anggota_1].cpp
│           │       KerjaSamaPemasokan_[103012500008_angggota_2].cpp
│           │
│           └───Pemasok
│                   Pemasok_[103012500113_anggota_1].cpp
│                   Pemasok_[103012500008_angggota_2].cpp
├── README.md
└── .gitignore
```
