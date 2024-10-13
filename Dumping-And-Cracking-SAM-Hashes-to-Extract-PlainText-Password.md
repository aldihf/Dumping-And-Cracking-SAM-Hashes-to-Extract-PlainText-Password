# Aldi Hoirul Fatih_09011282126069
# KEAMANAN JARINGAN KOMPUTER
1.	Cari command prompt dan jalankan dengan run as administrator.

 ![image](https://github.com/user-attachments/assets/3c90df1a-9835-463c-93fe-2acaa8e28a98)
  
2.	Untuk kita mengetahui userID dengan username milik kita, dengan menggetikan “wmic useraccount get name,sid” maka akan menampilkan daftar akun yang ada di sistem kita beserta SID nya.
 ![image](https://github.com/user-attachments/assets/ca12c093-ca89-482d-81ae-1c62b6ccf3c5)
3.	Disini kita akan mendownload dan mengekstrak file pwdump dan ophcrack .
 ![image](https://github.com/user-attachments/assets/ffe34419-c8de-43cb-a60a-ef004675a4e8)

4.	Buka kembali cmd dan kita masuk ke dalam folder pwdump yang telah dibuat sebelumnya dengan cara “cd C:\folder\tempat\kita\meletakan\pwdump”. Setelah itu ketik “PwDump7.exe” untuk mendapatkan dan menampilkan password hashes dan userID.
 ![image](https://github.com/user-attachments/assets/caf9fc5d-0979-4743-8582-8d4fc45a30ce)

5.	Setelah itu kita memindahkan isi file dari PwDump7.exe ke dalam file hashes.tst dengan cara “PwDump7.exe > c:\hashes.txt”.
 ![image](https://github.com/user-attachments/assets/90065e08-1c34-4721-8468-6fc81cd65cca)

6.	Isi file didalam hashes.txt
 ![image](https://github.com/user-attachments/assets/08f5152e-f3ab-413a-8bac-c6304e1f91be)

7.	Setelah itu kita mengisi username yang kosong pada file tersebut dengan username yang telah kita lihat sebelumnya dengan cara “wmic useraccount get name,sid”.
 ![image](https://github.com/user-attachments/assets/e67749b2-032b-4b5d-a711-e01ac43a99ad)

8.	Membuka aplikasi ophcrack dan setelah itu memilih load -> PWDUMP file -> memilih file hashes.txt yang telah dibuat sebelumnya.
 ![image](https://github.com/user-attachments/assets/faa35c26-9d5b-473f-a412-7efbd0d1b51d)

9.	Maka akan tampil seperti dibawah ini setelah memilih file hashes.txt sbebelumnya.
 ![image](https://github.com/user-attachments/assets/9ae44fae-f537-4530-a060-987c3b4de1c9)

10.	Setelah itu klik tables dan pada halaman table tersebut pilih vista free kemudian download vista free tersebut di web ophcrack.
    
 ![image](https://github.com/user-attachments/assets/01b58893-f5a2-4d55-9d5d-3cdb8b4d684f)

 ![image](https://github.com/user-attachments/assets/a7e750c7-30e1-4b57-9d70-e6f8ecf4168b)


11.	Setelah memilih table sebelumnya maka akan muncul icon crack disebelah tables, kemudian ketika kita memilih icon tersebut maka akan langsung memecahkan kata sandi. Butuh waktu beberapa menit untuk ophcrack memecahkan kata sandi.
 ![image](https://github.com/user-attachments/assets/e10a614b-67c6-45a6-bcb3-945e004f2dd1)

12.	Setelah selesai maka password akan tampil, Jika hasilnya menunjukkan not found maka kemungkinan besar karena windows 10 terbaru secara default tidak lagi menyimpan password di hash LM karena kurang aman atau bisa juga karena beberapa akun (seperti "Guest" atau "DefaultAccount") mungkin tidak memiliki password atau sedang tidak aktif, sehingga Ophcrack tidak menemukan apa-apa.
 ![image](https://github.com/user-attachments/assets/a945c618-4658-488b-8aae-323f80c08355)

