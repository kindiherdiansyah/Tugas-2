
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

- <?xml version="1.0" encoding="UTF-8"?>
  = mendefinisikan bahwa dokumen ini dibuat dengan aturan XML versi 1.0. Encoding menunjukkan bahwa file XML ini ditulis dengan kode UTF-8. UTF-8 adalah kode-kode yang wajib didukung oleh semua aplikasi yang memproses dokumen XML.
  
- <baksokuat xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="ordermakanan.xsd">
  = mendefinisikan namespace, Namespace didefinisikan oleh attribute xmlns pada tag awal sebuah elemen.
  
-<order>
		<kd_customer>001</kd_customer>
		<nama_costumer>Kindi Herdiansyah</nama_costumer>
		<nama_paket>Paket A</nama_paket>
		<nama_pesanan>Bakso Exelent</nama_pesanan>
		<harga>Rp.20.000</harga>
		<jml>2</jml>
		<total>40000</total>
		<waktu_pesan>08.00</waktu_pesan>
		<alamat_kirim>Jln. Sariasih No.2</alamat_kirim>
		<telp>081232132244</telp>
		<email>kindiherdiansyah@gmail.com</email>
	</order>
	<order>
		<kd_customer>002</kd_customer>
		<nama_costumer>Nida Regita</nama_costumer>
		<nama_paket>Paket B</nama_paket>
		<nama_pesanan>Bakso Johan </nama_pesanan>
		<harga>Rp.18.000</harga>
		<jml>2</jml>
		<total>36000</total>
		<waktu_pesan>09.00</waktu_pesan>
		<alamat_kirim>Jln. Sariasih No.2</alamat_kirim>
		<telp>081232903141</telp>
		<email>nidaregita@gmail.com</email>
	</order>
	<order>
		<kd_customer>003</kd_customer>
		<nama_costumer>Ariyq Naufal</nama_costumer>
		<nama_paket>Paket C</nama_paket>
		<nama_pesanan>Bakso Friendly</nama_pesanan>
		<harga>Rp.45.000</harga>
		<jml>2</jml>
		<total>90000</total>
		<waktu_pesan>08.00</waktu_pesan>
		<alamat_kirim>Jln. Sariasih No.7</alamat_kirim>
		<telp>081232132522</telp>
		<email>ariyqnaufal@gmail.com</email>
	</order>
	<order>
		<kd_customer>004</kd_customer>
		<nama_costumer>Della</nama_costumer>
		<nama_paket>Paket D</nama_paket>
		<nama_pesanan>Bakso First</nama_pesanan>
		<harga>Rp.45.000</harga>
		<jml>2</jml>
		<total>90000</total>
		<waktu_pesan>08.00</waktu_pesan>
		<alamat_kirim>Jln. Sariasih No.7</alamat_kirim>
		<telp>08123216265</telp>
		<email>dellac@gmail.com</email>
	</order>
	<order>
		<kd_customer>005</kd_customer>
		<nama_costumer>M.Irvan</nama_costumer>
		<nama_paket>Paket E</nama_paket>
		<nama_pesanan>Bakso Kapten</nama_pesanan>
		<harga>Rp.30.000</harga>
		<jml>2</jml>
		<total>60000</total>
		<waktu_pesan>08.00</waktu_pesan>
		<alamat_kirim>Jln. Sariasih No.7</alamat_kirim>
		<telp>081232132423</telp>
		<email>mirvan@gmail.com</email>
	</order>
</baksokuat>
  = Merupakan element
        Elemen XML mempunyai aturan penamaan yaitu:
-Nama dapat berisi huruf, angka, dan karakter lain.
-Nama tidak boleh dimulai dengan angka ataupun tanda baca.
-Nama harus dimulai dengan huruf
-Nama tidak boleh mempunyai spasi.



