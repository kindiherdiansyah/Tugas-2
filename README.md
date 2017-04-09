
Kindi Herdiansyah - 1154048
D4 TI 2A

Definisi SML Schema Definition (XSD)

  XML Schema Definition (XSD) language adalah bahasa skema standar untuk semua dokumen XML dan data. 
Pada tanggal 2 Mei 2001, World Wide Web Consortium (W3C) yang diterbitkan XSD dalam format versi 1.0-nya.

  Definisi bahasa XML Schema (XSD) memungkinkan Anda untuk menentukan struktur dan tipe data untuk dokumen XML. 
XML Schema mendefinisikan elemen, atribut, dan tipe data.

  XML Schema terdiri dari skema elemen tingkat atas. Definisi skema elemen harus menyertakan namespace berikut:
  " http://www.w3.org/2001/XMLSchema "
Skema elemen berisi tipe-tipe definisi (simpleType dan complexType elemen) dan mendeklarasikan atribut dan elemen.

Berikut Langkah-langkah untuk membuat file XML yang saya buat :
  1. Klik File -> New -> Project -> Plug-in Project
  2. Beri nama, Misal : Tugas2, lalu klik Next -> Finish
  3. Kemudian pada package yang telah dibuat klik kanan, pilih New -> Other -> XML file -> klik Next
     -> Beri nama: ordermakanan.xml -> Finish 
  4. Setelah file XML dibuat, kemudian mengisi data pada file XML tsb.contohnya buka file yang saya upload :"ordermakanan.xml"
  5. Setelah selesai, klik kanan pada ordermakanan.xml, lalu pilih Create XML Definition. Beri nama "ordermakanan.xsd". Klik Finish 
  6. Kemudian membuat reference file xsd pada file xml, pada ordermakanan.xsd klik kanan-> pilih Generate ->XML File
     -> beri nama ordermakanan.xml -> Next -> Finish. Lalu link reference tersebut di copy ke ordermakanan.xml
  7. Setelah itu membuat patterns pada atribut email dengan ketentuan @gmail.com
  8. Klik ordermakanan.xsd -> Pada Element email klik kanan ->Show Properties
     -> Pada constraint pilih pattern ->add -> beri nama ".+@gmail.com"
  9. Selanjutnya Validate, jika benar maka tidak akan muncul error
  
Analisis

=>	<?xml version="1.0" encoding="UTF-8"?>
= mendefinisikan bahwa dokumen ini dibuat dengan aturan XML versi 1.0. Encoding menunjukkan bahwa file XML 
ini ditulis dengan kode UTF-8. UTF-8 adalah kode-kode yang wajib didukung oleh semua aplikasi yang memproses dokumen XML.
  
=>	//<baksokuat xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="ordermakanan.xsd">
  = mendefinisikan namespace, Namespace didefinisikan oleh attribute xmlns pada tag awal sebuah elemen.//
  
=>	Semua tag pembuka dan penetup dibawah namespace
  = Merupakan element
        Elemen XML mempunyai aturan penamaan yaitu:
-Nama dapat berisi huruf, angka, dan karakter lain.
-Nama tidak boleh dimulai dengan angka ataupun tanda baca.
-Nama harus dimulai dengan huruf
-Nama tidak boleh mempunyai spasi.



