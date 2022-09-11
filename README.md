# Proposal
<h2>Permasalahan</h2>
<span>Data keuangan kost yang masih dilakukan secara manual (tulis tangan) dapat mengakibatkan beberapa data hilang karena terlalu banyak data yang tidak disimpan secara komputerisasi</span>

<h2>Rancangan Solusi</h2>
<ul>
  <li>Buat laporan penghasilan kost</li>
  <li>Buat pengingat jatuh tempo untuk member kost</li>
  <li>Buat riwayat pembayaran member kost</li>
</ul>
<h2>Use Case</h2>
<ul>
  <li>User admin dapat menambah member (penghuni kost)</li>
  <li>User admin dapat mengubah data member (penghuni kost)</li>
  <li>User admin dapat menginput pembayaran member (penghuni kost)</li>
  <li>User admin dapat melihat riwayat pembayaran member (penghuni kost)</li>
  <li>User admin dapat menghapus member (penghuni kost)</li>
  <li>User admin dapat melihat laporan penghasilan kost</li>
  <li>User admin dapat mencetak bukti pembayaran sewa kost</li>
  <li>User admin dapat mengelola data kamar kost</li>
  <li>User member (penghuni kost) dapat melihat riwayat pembayaran </li>
  <li>User member (penghuni kost) dapat melihat pembayaran selanjutnya </li>
</ul>

<h2>Struktur Data</h2>
<h3><li>member</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id_member</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>username</td>
        <td>string</td>
        <td>marsaa</td>
    </tr>
    <tr>
        <td>name</td>
        <td>string</td>
        <td>Marsa</td>
    </tr>
    <tr>
        <td>address</td>
        <td>text</td>
        <td>Cianjur</td>
    </tr>
    <tr>
        <td>phone_number</td>
        <td>string</td>
        <td>083868746352</td>
    </tr>
    <tr>
        <td>email</td>
        <td>string</td>
        <td>marsaaa04@gmail.com</td>
    </tr>
    <tr>
        <td>password</td>
        <td>string</td>
        <td>marsa0412</td>
    </tr>
    <tr>
        <td>id_room</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>date_of_entry</td>
        <td>date</td>
        <td>2022-08-20</td>
    </tr>
     <tr>
        <td>due_date</td>
        <td>date</td>
        <td>2022-09-20</td>
    </tr>
  </table>
  
<h3><li>admin</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id_admin</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>username</td>
        <td>string</td>
        <td>adminkos</td>
    </tr>
    <tr>
        <td>name</td>
        <td>string</td>
        <td>Sarah Yusti</td>
    </tr>
    <tr>
        <td>email</td>
        <td>string</td>
        <td>adminkos@gmail.com</td>
    </tr>
    <tr>
        <td>password</td>
        <td>string</td>
        <td>adminkosaja</td>
    </tr>
  </table>
  
<h3><li>room</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id_room</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>room_number</td>
        <td>string</td>
        <td>A1</td>
    </tr>
    <tr>
        <td>room_price</td>
        <td>integer</td>
        <td>550000</td>
    </tr>
    <tr>
        <td>floor</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>water</td>
        <td>integer</td>
        <td>25000</td>
    </tr>
    <tr>
        <td>electricity</td>
        <td>integer</td>
        <td>25000</td>
    </tr>
    <tr>
        <td>status</td>
        <td>string</td>
        <td>Sudah berpenghuni</td>
    </tr>
  </table>
  
<h3><li>payment</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id_payment</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>id_member</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>id_room</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>payment_date</td>
        <td>date</td>
        <td>2022-08-20</td>
    </tr>
    <tr>
        <td>nominal</td>
        <td>integer</td>
        <td>600000</td>
    </tr>
    <tr>
        <td>status</td>
        <td>string</td>
        <td>lunas</td>
    </tr>
  </table>


<h2>UX Wireframe</h2>
<h3><li>Login</li></h3>

![Login](https://user-images.githubusercontent.com/82995130/189541656-37064ed1-0416-4f74-9aeb-2785c679c444.png)

<h2>admin</h2>

<h3><li>Beranda admin</li></h3>

![Beranda (admin)](https://user-images.githubusercontent.com/82995130/189543768-e5177368-44dd-417c-a052-a9b535be4eed.png)

<h3><li>Profil admin</li></h3>

![Profil (admin)](https://user-images.githubusercontent.com/82995130/189543761-aa575cd6-3770-47ee-8f29-e5a60d766c97.png)

<h3><li>Edit Profil admin</li></h3>

![edit profil (admin)](https://user-images.githubusercontent.com/82995130/189543756-5e96c442-0b3e-423a-8518-1811d209f0d2.png)

<h3><li>Data member</li></h3>

![member](https://user-images.githubusercontent.com/82995130/189543741-d03ad821-e5b8-4224-ba2a-3dd6def557c0.png)

<h3><li>Tambah member</li></h3>

![tambah member](https://user-images.githubusercontent.com/82995130/189543735-9cf3ff23-4a60-4342-83a1-2a09a1a17fb5.png)

<h3><li>Edit member</li></h3>

![edit member](https://user-images.githubusercontent.com/82995130/189543723-7b213af7-995f-4a98-975c-f310bb65ac68.png)

<h3><li>Data Kamar Kost</li></h3>

![Tabel data kos](https://user-images.githubusercontent.com/82995130/189543716-f99406d1-35ee-47c5-96e2-612bce6c4494.png)

<h3><li>Tambah Kamar Kost</li></h3>

![Kamar kos](https://user-images.githubusercontent.com/82995130/189543705-6e22eac4-d937-45cf-a758-e04ff6dd18f1.png)

<h3><li>Edit Kamar Kost</li></h3>

![edit Kamar kos](https://user-images.githubusercontent.com/82995130/189543676-254c549c-5c43-4efc-86a3-a7fb5a3dab80.png)

<h3><li>Data Pembayaran</li></h3>

![Tabel Pembayaran](https://user-images.githubusercontent.com/82995130/189543669-bf4c2a6d-3d31-4432-b81c-f2f6b4bd074c.png)

<h3><li>Form Pembayaran</li></h3>

![Form Pembayaran](https://user-images.githubusercontent.com/82995130/189543656-3bf282b0-d6de-425f-96c6-e7ae929b7bf9.png)

<h3><li>Riwayat Pembayaran</li></h3>

![Tabel Riwayat Pembayaran](https://user-images.githubusercontent.com/82995130/189543648-f05337d5-1d8b-4c30-9f2a-89c2acf29500.png)


<br>


<h2>Member</h2>

<h3><li>Beranda member</li></h3>

![Beranda (member)](https://user-images.githubusercontent.com/82995130/189542205-7f3571a2-7f17-4097-ad4b-408e93fd06bc.png)

<h3><li>Profil member</li></h3>

![Profil (Member)](https://user-images.githubusercontent.com/82995130/189542224-d71b528a-6be9-4509-b1fc-55d50d1c9f8a.png)

<h3><li>Edit Password</li></h3>

![edit password (member)](https://user-images.githubusercontent.com/82995130/189542237-a9daff1d-6328-4676-b14d-545e6a7c71a0.png)

<h3><li>Riwayat Pembayaran</li></h3>

![Riwayat pembayaran (member)](https://user-images.githubusercontent.com/82995130/189543635-a995544f-0314-4508-88e3-9c268ce93a4f.png)









