# Proposal Aplikasi Billkost Berbasis Web
<h2>Author</h2>
<p>Nama  : Sarah Yusti Hamidah</p>
<p>NIM   : 1207050116</p>
<p>Kelas : IF-F</p>

<h2>Permasalahan</h2>
<span>Penagihan yang dilakukan secara manual membuat pemilik kost kesulitan untuk memberitahu tagihannya kepada penyewa kost</span>

<h2>Rancangan Solusi</h2>
<ul>
  <li>Buat pemberitahuan tagihan yang di kirim ke Whatsapp penyewa kost</li>
</ul>
<h2>Use Case</h2>
<ul>
  <li>User admin dapat menambah user pemilik kost</li>
  <li>User admin dapat melihat list pemilik kost</li>
  <li> User admin dapat mengubah user pemilik kost</ </li>
  <li> User admin dapat menghapus user pemilik kost</ </li>

 <li>User pemilik kost dapat mengelola data kamar</li>
<li>User pemilik kost dapat mengelola data penyewa</li>
<li>User pemilik kost dapat mengelola data sewa kamar kost</li>
<li>User pemilik kost dapat membuat tagihan kost</li>
</ul>

<h2>Struktur Data</h2>

<h3><li>users</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id </td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>first_name</td>
        <td>string</td>
        <td>Linda</td>
    </tr>
    <tr>
        <td>last_name</td>
        <td>string</td>
        <td>Hamidah</td>
    </tr>
    <tr>
        <td>email</td>
        <td>string</td>
        <td>linda08@gmail.com</td>
    </tr>
    <tr>
        <td>password</td>
        <td>string</td>
        <td>secret123</td>
    </tr>
    <tr>
        <td>role</td>
        <td>string</td>
        <td>owner</td>
    </tr>
</table>

<h3><li>rooms</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id </td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>number</td>
        <td>string</td>
        <td>A1</td>
    </tr>
    <tr>
        <td>length</td>
        <td>integer</td>
        <td>3</td>
    </tr>
    <tr>
        <td>width</td>
        <td>integer</td>
        <td>3</td>
    </tr>
    <tr>
        <td>facilities</td>
        <td>set</td>
        <td>AC</td>
    </tr>
    <tr>
        <td>cost_per_month</td>
        <td>integer</td>
        <td>600000</td>
    </tr>
  </table>
 
<h3><li>renters</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id </td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>nik</td>
        <td>string</td>
        <td>0156576435245375</td>
    </tr>
    <tr>
        <td>name</td>
        <td>string</td>
        <td>Linda Hamidah</td>
    </tr>
    <tr>
        <td>gender</td>
        <td>enum</td>
        <td>Perempuan</td>
    </tr>
    <tr>
        <td>phone_number</td>
        <td>string</td>
        <td>6285687856453</td>
    </tr>
    <tr>
        <td>address</td>
        <td>string</td>
        <td>Bandung</td>
    </tr>
  </table>
  
<h3><li>lodgings</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id </td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>renter_id</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>room_id</td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>start_at</td>
        <td>date</td>
        <td>2022-12-26</td>
    </tr>
    <tr>
        <td>end_at</td>
        <td>date</td>
        <td>2022-12-26</td>
    </tr>
  </table>
  
<h3><li>bills</li></h3>
  <table>
    <tr>
        <td>Atribut</td>
        <td>Tipe Data</td>
        <td>Contoh</td>
    </tr>
    <tr>
        <td>id </td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>lodging_id </td>
        <td>integer</td>
        <td>1</td>
    </tr>
    <tr>
        <td>name</td>
        <td>string</td>
        <td>listrik</td>
    </tr>
    <tr>
        <td>description</td>
        <td>text</td>
        <td>listrik bulanan</td>
    </tr>
    <tr>
        <td>amount</td>
        <td>integer</td>
        <td>40000</td>
    </tr>
    <tr>
        <td>per_month</td>
        <td>integer</td>
        <td>1</td>
    </tr>
  </table>


<h2>UX Wireframe</h2>
<h3><li>Login</li></h3>

![Login](https://user-images.githubusercontent.com/82995130/189541656-37064ed1-0416-4f74-9aeb-2785c679c444.png)

<h2>admin</h2>

<h3><li>Beranda admin</li></h3>

![Beranda Admin](https://user-images.githubusercontent.com/82995130/209595788-64a7246b-53c0-4520-b9c0-c0b3c59c4cb6.png)


<br>


<h2>Member</h2>

<h3><li>Beranda member</li></h3>

![Beranda pemilik kos](https://user-images.githubusercontent.com/82995130/209595809-bcaf7d03-0c46-4ba2-9870-463ba7e2f399.png)

