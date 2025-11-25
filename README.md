# Manajemen-File-Server-

Membuat Folder 
~~~~
mkdir project_manajemen
~~~~
~~~~
cd project_manajemen
~~~~

Membuat Folder dan Subfolder
~~~~
mkdir -p engineering/documents engineering/archives
mkdir -p marketing/documents marketing/archives
mkdir -p hr/documents hr/archives
ls
~~~~
Menyalin Folder Ke Lokasi Lain
~~~~
cp -r /home/gabby/project_manajemen/marketing/documents /home/gabby/project_manajemen/marketing/archives
~~~~
Mengelola User dan Permission Pada Direktori
~~~~
sudo adduser marketing
sudo chown -R marketing /home/gabby/project_manajemen/marketing
chmod -R 700 /home/gabby/project_manajemen/marketing
sudo adduser engineering
sudo chown -R engineering /home/gabby/project_manajemen/engineering
sudo chown -R 700 /home/gabby/project_manajemen/engineering
sudo adduser hr 
sudo chown -R hr /home/gabby/project_manajemen/hr
sudo -R 700 /home/gabby/project_manajemen/hr
~~~~
Menguji Login User di Terminal
~~~~
cd marketing
su marketing
ls
exit
~~~~
~~~~
su engineering
ls
exit
~~~~
~~~~
su hr
ls
exit
~~~~
Mencari File PDF dan Menyimpan Hasil
~~~~
sudo find /home/gabby/project_manajemen -type f -name "*.pdf" > daftar_pdf.txt
~~~~
Mencari semua file PDF di folder saat ini yang diubah dalam 7 hari terakhir, lalu menyimpan hasilnya ke file daftar_pdf.txt
~~~~
find . -type f -name "*pdf". -mtime -7 -print > daftar_pdf.txt
cat daftar_pdf.txt
~~~~




