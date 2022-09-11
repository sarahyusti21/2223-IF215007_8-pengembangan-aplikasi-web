# Propsal
<h2>Permasalahan</h2>
<span>Data kosan yang masih dilakukan secara manual (tulis tangan) dapat mengakibatkan beberapa data hilang karena terlalu banyak data yang tidak disimpan secara komputerisasi</span>

<h2>Rancangan Solusi</h2>
Aplikasi Sistem Informasi Keuangan Kosan berbasis web adalah tawaran solusi yang saya ajukan untuk memudahkan pemilik kos mengetahui keuangan kosan tersebut.

<h2>Use Case</h2>
<ul>
  <li>User admin dapat menambah member (penghuni kos)</li>
  <li>User admin dapat mengubah data member (penghuni kos)</li>
  <li>User admin dapat menginput pembayaran member (penghuni kos)</li>
  <li>User admin dapat melihat riwayat pembayaran member (penghuni kos)</li>
  <li>User admin dapat menghapus member (penghuni kos)</li>
  <li>User admin dapat melihat laporan penghasilan kos</li>
  <li>User admin dapat mencetak bukti pembayaran sewa kos</li>
  <li>User admin dapat mengelola data kamar kos</li>
  <li>User member (penghuni kos) dapat melihat riwayat pembayaran </li>
  <li>User member (penghuni kos) dapat melihat pembayaran selanjutnya </li>
</ul>

<h2>Struktur Data</h2>
<b>member</b>
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
        <td>marsaulwan</td>
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
  
  <b>admin</b>
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
  
  <b>room</b>
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
  
  <b>payment</b>
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
