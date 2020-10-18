# Jarkom_Modul1_Lapres_T21

praktikan
- Achsan Noorsalam (021)
- I Komang Aditya Mahadiharja (042)


## Display Filter

### soal 1 

Sebutkan webserver yang digunakan pada "testing.mekanis.me"!

jawab :
 pertama melakukan ping pada web tersebut 
 
 (photo)
 
 lalu menggunakan filter ip.src 
 
 (photo)
 
 ### soal 2 
 
 menyimpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"
 
 jawab :
 buka menu FILE dan pilih submenu export ke dalam http
 
 lalu seach nama gambar yang ingin dicari dan disimpan
 
 ### soal 3 
 
 Cari username dan password ketika login di "ppid.dpr.go.id"!
 
 jawab :
 username dan password dapat ditemukan dengan pertama menggunakan filter http.host == ppid.dpr.go.id
 salah satu packet akan memiliki aplication form yang didalamnya berisikan username dan password
 
 (photo)
 
 
 ### soal 4 
 
 Temukan paket dari web-web yang menggunakan basic authentication method!

jawab :
dengan menggunakan filter http.authbasic

(photo)


### soal 5

Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!

jawab : 
pertama melakukan filter http.host == aku.pengen.pw
lalu pada paket yang terfilter pada bagian authorization -> credential akan terlihat password dan usernamenya 

(photo)

lalu masukkan password dan username pada aku.pengen.pw

(photo)

jawab pertanyaan yang ada pada web tersebut 

(photo)

### soal 6

Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).

jawab : 
menggunakan filter ftp-data dan menggunakan menu find(ctrl+f) untuk mencari answer.zip dan zipkeynya 
baca paket zipkeynya dengan follow -> tcp stream
download answer.zip dengan follow-> tcp stream lalu ubah ascii menjadi raw
buka anwer.zip dengan kunci dari zipkey

(photo)

### soal 7




 

 
