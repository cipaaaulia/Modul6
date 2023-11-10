# Modul6

1. **Enum `Seed` dan `GameState`:**
   - `Seed` adalah enumerasi untuk merepresentasikan isi dari setiap sel pada papan permainan (kosong, 'X', atau 'O').
   - `GameState` adalah enumerasi untuk merepresentasikan status permainan (sedang berlangsung, seri, 'X' menang, atau 'O' menang).

![image](https://github.com/cipaaaulia/Modul6/assets/149106143/87e8f2d5-7299-40f2-bc77-d0d7bf01ccec)
    

2. **Kelas `Cell`:**
   - Kelas ini merepresentasikan setiap sel pada papan permainan.
   - Setiap sel memiliki atribut `row` dan `col` untuk menyimpan posisinya, serta atribut `content` untuk menyimpan isinya (' ', 'X', atau 'O').
   - Metode `clear` digunakan untuk mengosongkan sel.

![image](https://github.com/cipaaaulia/Modul6/assets/149106143/c662e32e-b81d-4b7f-a7d5-ea8738000cd0)


3. **Kelas `Board`:**
   - Kelas ini merepresentasikan papan permainan dengan seluruh selnya.
   - Metode `init` digunakan untuk menginisialisasi papan permainan.
   - Metode `is_draw` mengecek apakah permainan berakhir dengan seri.
   - Metode `has_won` mengecek apakah pemain dengan tanda tertentu menang setelah melakukan langkah pada suatu sel.

![image](https://github.com/cipaaaulia/Modul6/assets/149106143/52c0d40e-dcec-4a75-9fa5-849bd8070192)


4. **Kelas `GameMain` (Turunan dari `tk.Canvas`):**
   - Kelas ini adalah antarmuka grafis permainan Tic Tac Toe menggunakan `tkinter`.
   - Inisialisasi dilakukan dengan mengatur lebar dan tinggi kanvas, menghubungkan metode `on_click` dengan event mouse click, dan memanggil metode `init_game`.
   - Metode `init_game` menginisialisasi permainan, termasuk menggambar papan dan menampilkan status.
   - Metode `on_click` dipanggil setiap kali pemain melakukan klik pada sel tertentu. Metode ini memproses langkah pemain, mengupdate permainan, dan menggambarkan ulang papan dan status.
   - Metode `update_game` memeriksa apakah pemain yang melakukan langkah menang atau apakah permainan berakhir seri.
   - Metode `draw_board`, `draw_grid`, `draw_cells`, dan `draw_cell` digunakan untuk menggambar elemen-elemen pada kanvas.
   - Metode `display_status` menampilkan status permainan di bagian bawah kanvas.

![image](https://github.com/cipaaaulia/Modul6/assets/149106143/fcc17ad3-a96f-491c-9b88-13d6115ec8d2)

lebih lengkapnya dapat dilihat pada code yang disediakan


5. **Menjalankan Aplikasi:**
   - Membuat instance `tk.Tk()` sebagai root window.
   - Membuat instance `GameMain` (turunan dari `tk.Canvas`) dan menampilkannya.
   - Memulai main loop menggunakan `root.mainloop()` untuk menjalankan aplikasi dan menanggapi event.

![image](https://github.com/cipaaaulia/Modul6/assets/149106143/07e5a8bf-38b6-4344-8c8e-de1694b17b79)

Hasil saat kode program dijalankan dan dimainkan adalah sebagai berikut :
![image](https://github.com/cipaaaulia/Modul6/assets/149106143/389edcd9-2fe2-44cd-b64b-5252eb1b86da)



Kode tersebut menggambarkan struktur dasar permainan Tic Tac Toe menggunakan modul `tkinter`.
