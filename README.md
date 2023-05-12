# Auto Install OS Windows VPS Digital Ocean

<h2 id=buat-droplet>Buat Droplet</h2>
<p>Kali ini saya memakai OS Ubuntu 20.04 dalam proses pembuatannya, dan jangan lupa untuk tidak mencentang pilihan User Data</p>
<h2 id=masuk-mode-recovery>Masuk Mode Recovery</h2>
<p>Setelah kita berhasil membuat sebuah VPS (droplet) selanjutnya kita ubah VPS kita ke mode recovery, caranya :</p>

![alt text](https://raw.githubusercontent.com/paratonsp/digital-ocean-windows/main/img/digitaloceanrecovery.png)

<ul>
<li>Matikan VPS kita.</li>
<li>Ubah ke recovery ke Boot from Recovery ISO.</li>
<li>Kemudian hidupkan kembali VPSnya</li>
<li>Lalu masuk ke console.<br>
Nanti akan muncul jendela browser dengan gambar di bawah ini, jika tidak muncul seperti gambar di bawah, silahkan tekan ENTER</li>
</ul>

![alt text](https://raw.githubusercontent.com/paratonsp/digital-ocean-windows/main/img/digitaloceanrecovery2.png)

<p>Kalian bisa login menggunakan Putty atau bisa juga login menggunakan console web browser dengan menekan / memilih angka 6 dan ENTER</p>
<h2 id=install-windows>Install Windows</h2>
<p>Kalau sudah berhasil masuk/login ke mode recovery, jalankan perintah dibawah ini untuk memulai proses install</p>
<div class=highlight><pre tabindex=0 style=color:#f8f8f2;background-color:#272822;-moz-tab-size:4;-o-tab-size:4;tab-size:4><code class=language-bash data-lang=bash>wget https://raw.githubusercontent.com/paratonsp/digital-ocean-windows/main/windows.sh
bash windows.sh
</code></pre></div><p>Kalian tinggal pilih OS yang ingin kalian install, kalian juga bisa menggunakan <em>mirror</em> atau kalau dirasa server tempat image yang saya sediakan kurang cepat, kalian bisa me-<em>mirror</em> file image yang saya buat di server kalian sendiri.</p>
<p>Setelah proses install selesai, script ini akan otomatis meng-shutdown VPS kalian.</p>
<h2 id=matikan-mode-recovery>Matikan Mode Recovery</h2>
<p>Setelah proses di atas selesai sekarang kita matikan mode recovery di VPS kita, caranya :</p>
<ul>
<li>Ubah recovery ke Boot from Hard Drive</li>
<li>Hidupkan kembali VPS</li>
</ul>
<p>RDP kalian siap dipakai! dan kalian bisa login menggunakan RDP tanpa harus melakukan konfigurasi IP di Windows</p>
<h2 id=catatan>Catatan</h2>
<ul>
<li>
<p>Windows 2019
Username : Adminstrator
Password : Botol123456789!</p>
</li>
<li>
<p>Windows 2012
Username : Administrator
Password : Nixpoin.com123!</p>
</li>
</ul>
<p><em><strong>SEGERA GANTI PASSWORD SETELAH PROSES INSTALL SELESAI!!!!!!</strong></em></p>
<p>Reference: https://nixpoin.com/tutorial/script-install-windows-digitalocean/</p>
