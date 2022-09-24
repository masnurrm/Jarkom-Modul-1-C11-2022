# Jarkom-Modul-1-C11-2022

*Repository* ini berisi laporan resmi dari praktikum modul 1 dari mata kuliah Jaringan Komputer tahun 2022.

## **Data Diri**

| Nama                     | Kelas-Kelompok      | NRP      |
|--------------------------|------------|------------|
| Nur Muhammad Ainul Yaqin | C-11  | 5025201011         | 

</br>

Adapun laporan resmi terlampir sebagai berikut dengan total 10 *section* soal.

## **Soal 1**

**Sebutkan *web* *server* yang digunakan pada "monta.if.its.ac.id"!**

Dapat dilakukan dengan menggunakan *command* pada Wireshark, yaitu ***http***. Akan muncul beberapa paket, pilih paket yang berasal dari IP Server, yaitu **103.94.189.5** atau paket dengan *method* HTTP (bukan GET). Buka informasi paket, maka akan diketahui bahwa server menggunakan ***nginx/1.10.3\r\n***.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/2b90eb37-b8c0-4284-b892-d8858b54f6cb/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073108Z&X-Amz-Expires=86400&X-Amz-Signature=efd407ff4189263dfd68bed53f531894c6cb6407407b4623edfa1f0a81abada9&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

</br>

## **Soal 2**

**Ishaq sedang bingung mencari topik TA untuk semester ini, lalu ia datang ke *website* monta dan menemukan detail topik pada *website* “monta.if.its.ac.id”. Judul TA apa yang dibuka oleh Ishaq?**

Pertama, lakukan *tracking* dengan menggunakan ***http.host contains "monta.if.its.ac.id"***. Dapatkan sebuah paket dengan perintah GET dengan detailTopik. Diketahui bahwa Ishaq membuka folder 194.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/70e5c816-2baf-411e-9623-e8d4d7094ff7/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073136Z&X-Amz-Expires=86400&X-Amz-Signature=b283d14963ae424c6d92d6da7af8d68fac53ec88533e6d105d610a7e80cdc474&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Selanjutnya, dengan menggunakan perintah ***http***, buka paket dengan format html setelah detailTopik.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/1a24fe13-f852-4cf5-aca3-b583c374eff5/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073156Z&X-Amz-Expires=86400&X-Amz-Signature=dc648f2f361f27fd3d5d9ef8488813e5a8b9eb002acd4e586c4196eaf3f86240&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Diketahui, bahwa informasi paket sesuai dengan informasi yang didapatkan sebelumnya, yaitu terletak pada folder 194.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/1050541a-9336-4ae0-b8b2-bbacbc48efb2/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073200Z&X-Amz-Expires=86400&X-Amz-Signature=b990b238478af349b9de82cc3dbc6b0b5f1109e30d7492b3aa09a6ade2f6e552&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Kemudian, didapatkan judul TA dengan mencari pada file html, yaitu **Evaluasi untuk kerja User Space Filesystem FUSE**, oleh WAHYU SUADI, Rabu 17 Maret 2021.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/488ba085-b046-42c2-b6a6-90e0b27fc8bf/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073203Z&X-Amz-Expires=86400&X-Amz-Signature=5a853c1cad70c8743f2fff9ffafe77b5f52c4eb20675d2f6e2dd8f646d635b78&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


</br>

## **Soal 3**

**Filter sehingga Wireshark hanya menampilkan paket yang menuju port 80!**

Dapat dilakukan dengan menggunakan *command* pada Wireshark, yaitu ***tcp.dstport == 80*** sehingga didapatkan hasil sebagai berikut.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/364c8086-aa07-4763-af7e-2ca73c62d822/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073312Z&X-Amz-Expires=86400&X-Amz-Signature=f36fdb9df8c3fb847ea52a9ffa645d34d237ad72b8a243a25a3a3eb9483dfb3a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


</br>

## **Soal 4**

**Filter sehingga Wireshark hanya mengambil paket yang berasal dari port 21!**

Dapat dilakukan dengan menggunakan *command* pada Wireshark, yaitu ***tcp.srcport == 21*** sehingga didapatkan hasil sebagai berikut.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/00b72cf4-9da6-49ab-8962-bf82c948cc88/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073324Z&X-Amz-Expires=86400&X-Amz-Signature=f42ffc267e6bb14173e7059efb31cd096680323b22c29065c1774588f509bfe4&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


</br>

## **Soal 5**

**Filter sehingga Wireshark hanya mengambil paket yang berasal dari port 443!**

Dapat dilakukan dengan menggunakan *command* pada Wireshark, yaitu ***tcp.srcport == 443*** sehingga didapatkan hasil sebagai berikut.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/c8a259b0-0e13-4db8-9972-c837a102a616/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073333Z&X-Amz-Expires=86400&X-Amz-Signature=e919884e2633a2fcbba6753d3607557b4da4c8f0418c36b7c7010aab373b4339&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


</br>

## **Soal 6**

**Filter sehingga Wireshark hanya menampilkan paket yang menuju ke “go.id”!**

Pertama, adalah dengan mencari IP dari “lipi.go.id”, yaitu dengan menggunakan *command* ***http.host contains “lipi.go.id”*** sehingga didapatkan sebuah paket dengan informasi Dst: 203.160.128.158 yang merupakan IP dari “lipi.go.id”.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/a06692d3-e758-48db-a98e-351bd50fe81c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073345Z&X-Amz-Expires=86400&X-Amz-Signature=e048c154521f4f76c955a4a2a7303895fb595c4087f4473628cfee93f5e903e2&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Kedua, lakukan pencarian paket dengan menggunakan *command* ***ip.dst == 203.160.128.158***.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/cdaae4c7-4ea6-4cbe-8309-aaf7ffbc0e11/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073355Z&X-Amz-Expires=86400&X-Amz-Signature=e1bd4fc59bdd2bb0fa07d5f6103b4c8432ada78bdbabdccd5b5f3b617ce61f22&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


</br>

## **Soal 7**

**Filter sehingga Wireshark hanya mengambil paket yang berasal dari ip kalian!**

Pertama, temukan ip address device dengan menggunakan perintah ***ipconfig*** pada *command prompt*. Pilih alamat ip pada bagian WiFi (karena saat pengerjaan menggunakan jaringan Wifi).

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/e399c6db-3ddd-4219-88a9-a3bb77301ed1/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073407Z&X-Amz-Expires=86400&X-Amz-Signature=7ccb32d6914f6c391e26ea9c588b19c440bc89b6f8f25bc930f10d0ddc7b266c&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Kedua, lakukan pencarian paket dengan menggunakan *command* ***ip.src == 192.168.1.12***.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/af180bfb-6c54-4576-a18e-bffb5d6f6c4d/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073411Z&X-Amz-Expires=86400&X-Amz-Signature=4e2cbad4106845527427cb660fff5f5e88c734640545de7b6b18940f8ffc6eda&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


</br>

## **Soal 8**

**Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.**

Pengerjaan ini menggunakan referensi video berikut.

[https://www.youtube.com/watch?v=3Zb_EebU22o&ab_channel=danscourses](https://www.youtube.com/watch?v=3Zb_EebU22o&ab_channel=danscourses)

Untuk mendapatkan percakapan dengan tingkat keamanan tinggi, maka seharusnya *host* menggunakan protokol TCP. Sehingga, digunakan ***tcp.stream*** untuk mendapatkan paket-paket yang berisi interaksi *host*-*host*, atau *host*-*server*. Pilih paket dengan interaksi *host*-*host*.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/0aac164d-50d8-4295-9a09-767e9e740091/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073521Z&X-Amz-Expires=86400&X-Amz-Signature=7af56a88ae11e5fdb6b12d1c01c6d06bf98460dae61f3d4b177613eb163cb77f&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Kemudian, *follow* TCP Stream tersebut, sehingga didapatkan percakapan sebagai berikut.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/273f83f9-0494-402a-861a-630694c102a1/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073531Z&X-Amz-Expires=86400&X-Amz-Signature=f81a8498eefd8486bd4986003f05cbeaa2dc25ac03171dfce47964ce018f0015&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/45d13f36-36cd-49b1-a2a8-d50fe89b7d92/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073535Z&X-Amz-Expires=86400&X-Amz-Signature=39f6bb6421bc843b6371c39d4a33b08a0c8baefdcc54afa8ba5e76e8524aac4c&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

> Sebenarnya, terdapat 2 percakapan lain yang ditemukan, namun karena *clueless* dan tidak berguna, Saya tidak laporkan di laporan resmi ini.


</br>

## **Soal 9**

**Terdapat laporan adanya pertukaran *file* yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah *file* yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama *file* yang ditemukan dengan format [nama_kelompok].des3 dan simpan *output file* dengan nama “flag.txt”.**

Pengerjaan ini menggunakan referensi berikut untuk *decrypt* des3.

[https://gist.github.com/ayosec/11177563](https://gist.github.com/ayosec/11177563)

Pertama, ambil beberapa informasi dari nomor sebelumnya, yaitu *port* 9002, metode *decrypt*, dan petunjuk *password.*

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/54a479cc-e51f-4afc-9dc1-5fb15fb59cb2/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073556Z&X-Amz-Expires=86400&X-Amz-Signature=f41c956cfb7552eaf1c809fbb2752eb6b6f4b90a2d5f1fa74a8c6bd2d73b7f11&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/8757bd40-e2a5-4b86-972e-23c8fa1be587/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073559Z&X-Amz-Expires=86400&X-Amz-Signature=83d14f503b0b255064dd9430eab44777e5f941e88a4aa513254e209d9ede9a37&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/670dd5a5-1ef1-4843-a9c8-c1dbc7228e0c/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073603Z&X-Amz-Expires=86400&X-Amz-Signature=657311ea5659855a9db3b0b1108095e28768627ef97fb20b5b444e4ae07a4659&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Selanjutnya, cari paket dengan TCP *port* 9002, dengan menggunakan ***tcp.port == 9002***.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/1f62d684-0e9b-47f5-a152-18639f2f013f/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073629Z&X-Amz-Expires=86400&X-Amz-Signature=57a6c96ab8d114a24a17048184ad7d1816bbb6773d09c1f5181928817b539353&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Ambil paket dengan *length* terbesar. *Follow* paket tersebut sehingga didapatkan sebuah informasi *salted message*.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/502e9c73-d827-4d86-ba60-d5040e6a1722/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073631Z&X-Amz-Expires=86400&X-Amz-Signature=31b5216588b1a31d3afc715e7f4af041662e7cb10045f4c310b2152a7895a75d&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/e342f105-4a8c-483d-bf0d-d5ce02f57511/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073729Z&X-Amz-Expires=86400&X-Amz-Signature=190bedcbcd6568ca2edab5d20d967f378da10a91e8ed93a9f057b99cb60d97f1&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


> Terdapat 2 paket lain dengan *length* yang besar juga, namun hanya berisi tautan YouTube *clueless*.

Lakukan *export* dengan mengatur konten menjadi RAW terlebih dahulu. Simpan sebagai **C11.des3**.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/f0228be4-cbc5-4bc8-8eb8-278c62328036/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073650Z&X-Amz-Expires=86400&X-Amz-Signature=df21611678b8ed63687e7e9d686f888f6106746c76cbfa53521c6ca61b954430&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/dcfb8e6d-105f-4711-8fa3-473f249e9102/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073742Z&X-Amz-Expires=86400&X-Amz-Signature=e6a87bca5cafb739a0139506e544239d65b7b5c43745624b8196e55f7b5795a4&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Lakukan *decrypt* dengan menggunakan openSSL dengan *command* berikut.

```bash
**openssl des3** -d -salt -in **C11.des3** -out **flag.txt**
```

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/05af7471-6037-454f-8750-0b577d45f093/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073759Z&X-Amz-Expires=86400&X-Amz-Signature=6cd4f18656854488bf3275e87c137485367812964dc47c742415325e44ee0c2c&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Didapatkan pesan *flag*, yaitu **JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}**.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/15d95af7-fd29-480d-a409-793fde5406f1/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073803Z&X-Amz-Expires=86400&X-Amz-Signature=e4dc08a576dfc618e85a5e45e8f69dbc45eb08ca4701f78b85482e096903b906&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)


</br>

## **Soal 10**

**Temukan *password* rahasia (*flag*) dari organisasi bawah tanah yang disebutkan di atas!**

Sesuai referensi ([https://id.wikipedia.org/wiki/Daftar_karakter_The_Quintessential_Quintuplets](https://id.wikipedia.org/wiki/Daftar_karakter_The_Quintessential_Quintuplets)), *password* yang digunakan adalah **nakano**. 

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/003063fb-d7de-4fdd-9990-3c9d90653a69/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073821Z&X-Amz-Expires=86400&X-Amz-Signature=dc7819d51384074abf0c1b2073f85a0d4747f5ee4194610f3909b98bbe90b797&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Sedangkan untuk hasil dari *flag* adalah **JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}**.

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/15d95af7-fd29-480d-a409-793fde5406f1/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220924%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220924T073803Z&X-Amz-Expires=86400&X-Amz-Signature=e4dc08a576dfc618e85a5e45e8f69dbc45eb08ca4701f78b85482e096903b906&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

</br>

# **Kendala**

Terdapat beberapa kendala saat pengerjaan praktikum, antara lain sebagai berikut.

1. Tantangan dalam manajemen pekerjaan dan waktu, karena dikerjakan sendiri tanpa adanya pembagian *task*.
2. Terdapat kebimbangan dalam mengerjakan soal nomor 3 hingga 6, mengenai perbedaan maksud dari `mengambil` dan `menampilkan`. Namun akhirnya Saya putuskan hanya dengan menampilkan saja untuk kedua-duanya (*screenshot* dari hasil *filter*).
3. Terdapat *stuck* saat pengerjaan nomor 9, di mana proses *decrypt* gagal. Ternyata, *file* des3 harus berupa RAW, bukan ASCII.