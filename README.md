# DearLaura.github.io
Dearkamu
<html>
<meta charset='UTF-8' />
<meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5'
  name='viewport' />
<meta content='IE=edge' http-equiv='X-UA-Compatible' />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Ubuntu:wght@400;700&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script>
<link href="https://drive.google.com/uc?export=view&id=1UL3xEyWfQmzDQhkQ_hkB_gTpWsvue7IJ" rel="stylesheet"
  type="text/css" />
<script src="https://milihdiem.feeldream.repl.co/script.js"></script>

<head>
  <title>Dear Kamu</title>
  <!-- 

-->
</head>
<style>
  :root {
    --warna-bg: rgba(0, 0, 0, .5);
    --warna-teks: white;
    --warna-bingkai: rgba(255, 255, 255, .5);
    --bingkai: 20px;
    --gaya-font: 'Ubuntu', sans-serif;
  }

  body {
    background-image: url("https://i.postimg.cc/W4sxgKtQ/Fg-N0-MMIa-EAAGet-W.jpg");
    background-repeat: no-repeat;
    background-size: 110% 110%;
    animation: none;
    transition: all .3s ease;
  }
</style>

<body>
  <div id="bodyblur"></div>

  <div id='Content'>
    <!-- Foto Atas -->
    <div><img id="fotosatu" src="" /><img id="fotodua" src="" /><img id="fototiga" src="" /><img id="fotoempat"
        src="" /></div>
    <div>
      <blockquote id='bq'>
        <p id="kalimat">...</p>
      </blockquote>
    </div>

    <!-- Tombol Kirim Pesan -->
    <div id="contTom"><a class='button' onClick="sjawab()"></i>Kirim Pesan</a></div>
  </div>

  <!-- Jangan Edit Bagian Ini -->
  <script>
    function showDiv() {setTimeout(setel, 50); pergantian(); setTimeout(kpemb, 100); document.getElementById('Content').style = "opacity:1;margin-top:4vh;animation:kont 5s infinite;"; document.querySelector("body").style.animation = "none 8s ease infinite";} function kpemb() {bq.style = "opacity:1;visibility:visible;margin-top:5px";}
    function loadfoto() {fotosatu.style = "display:inline-flex"; fotosatu.src = gambar1; fotodua.src = gambar2; fototiga.src = gambar3; fotoempat.src = gambar4;}
    function tombol() {contTom.style = "margin-top:50px;opacity:1;transform: scale(1);"; ftom = 1;} ftom = 0; function fakhiran() {document.getElementById("akhiran").style = "display:inline-flex";}
    const swals = Swal.mixin({allowOutsideClick: false, cancelButtonColor: '#FF0040', }); const swalsy = Swal.mixin({confirmButtonText: 'Iya', allowOutsideClick: false, }); const swalst = Swal.mixin({allowOutsideClick: false, showConfirmButton: false, timer: 1000, timerProgressBar: true, didOpen: () => {Swal.showLoading(); const b = Swal.getHtmlContainer().querySelector('b'); timerInterval = setInterval(() => {Swal.getTimerLeft()}, 100)}, willClose: () => {clearInterval(timerInterval)}}); const style = document.createElement('style'); var today = new Date(); var dd = String(today.getDate()).padStart(2, '0'); var mm = String(today.getMonth() + 1).padStart(2, '0'); var yyyy = today.getFullYear(); const monthNames = ["Januari", "Februari", "Maret", "April", "Mei", "Juni", "Juli", "Agustus", "September", "Oktober", "November", "Desember"]; today = dd + ' ' + monthNames[today.getMonth()] + ' ' + yyyy;
    function play() {var audio = new Audio(''); audio.play();} function sjawab() {if (ftom == 1) {contTom.style = "display:none"; jawab();} }
    function otomatis() {befanimkata(); setTimeout(animkata, 300);} function befanimkata() {kalimat.style = "transform:scale(.3);";} function animkata() {kalimat.style = "transform:scale(1);";}
    function finalakhir() {bodyblur.style = "-webkit-backdrop-filter:blur(5px); backdrop-filter:blur(5px);"; bq.style = "display:none;"; fotoatas.style = "animation:aniopa .8s"; idpertama.style = "opacity:1;transform: scale(1);margin-top:30px"; setTimeout(aksiakhir, 400); idkedua.innerHTML = katakedua; idketiga.innerHTML = kataketiga;}
    function setel() {audio.play();} function setel2() {bgm.play();}
    var aa = 0, katadelapan; function ngetik() {
      if (aa < katadelapan.length) {kalimat.innerHTML += katadelapan.charAt(aa); aa++; setTimeout(ngetik, 75);}
      if (aa == katadelapan.length) {kalimat.innerHTML = katadelapan + emot; setTimeout(tombol, 1000);}
    }
    function showpalingakhir() {idketiga.style = "font-weight:700;opacity:1;font-size:16px;margin-top:20px;animation:rto .6s infinite alternate;"; setTimeout(tombol, 1000);}

    function pergantian() {setTimeout(gantikata, 500); setTimeout(gantikata, 2300); setTimeout(gantikata, 3500); setTimeout(gantikata, 6000); setTimeout(gantikata, 7000); setTimeout(gantikata, 8300); setTimeout(gantikata, 9999);}
    function tfkata() {fkata += 1;} function bersihkan() {kalimat.innerHTML = ""; fototiga.style = "display:none"; fotoempat.style = "display:inline-flex";}
    fkata = 1; function gantikata() {
      if (fkata == 1) {otomatis(); kalimat.innerHTML = katasatu;}
      if (fkata == 2) {otomatis(); kalimat.innerHTML = katadua;}
      if (fkata == 3) {otomatis(); kalimat.innerHTML = katatiga; fotosatu.style = "display:none"; fotodua.style = "display:inline-flex";}
      if (fkata == 4) {otomatis(); kalimat.innerHTML = kataempat;}
      if (fkata == 5) {otomatis(); kalimat.innerHTML = katalima;}
      if (fkata == 6) {otomatis(); kalimat.innerHTML = kataenam; fotodua.style = "display:none"; fototiga.style = "display:inline-flex";}
      if (fkata == 7) {otomatis(); kalimat.innerHTML = katatujuh; setTimeout(bersihkan, 1700); setTimeout(ngetik, 1750)}
      setTimeout(tfkata, 300);
    }
  </script> <!-- Sampai Sini -->

  <!-- Ganti Kata², Foto, Lagu di bawah ya
1) Upload foto ke https://postimages.org
     buat dapetin linknya
2) Ganti Lagu Upload ke replit.com
     atau bisa juga ke mailboxdrive.com -->

  <script type="text/javascript">
    async function menuju() {await swals.fire('Kirim pesan ke Twitter aku, ya!'); window.location = "https://twitter.com/pimiipimii"}
    async function jawab() {
      var {value: jawaban} = await swals.fire({
        title: 'Isi Pesan Kamu &#128073;&#128072;', input: 'text', allowOutsideClick: false, showCancelButton: false,
      });
      if (jawaban && jawaban.length < 19) {
        window.jawaban = jawaban;
  
        menuju();
      } else {
        await swals.fire('Ups!', 'Jawaban tidak boleh kosong atau lebih dari 18 karakter, ya!'); jawab();
      }
    }

    async function pertama() {
      audio = new Audio('https://audio.jukehost.co.uk/q4E0AxjWVfcfIfhC9ASiIHjtNuYkAXbF');

      gambar1 = "https://i.postimg.cc/KYsx0F66/Fg-ZWTz5a-EAQBCp-K.jpg";
      gambar2 = "https://i.ibb.co/d4fJCXL/ntah.gif";
      gambar3 = "https://i.ibb.co/4Wh4mg7/wortel.gif";
      gambar4 = "https://i.ibb.co/9WT8Qcw/tos.gif";

      katasatu = "Dear,Laura!,";
      katadua = "Sebenernya aku suka sama kamu, Tapi,";
      katatiga = "Aku memilih untuk diem 🥺";
      kataempat = "Daripada";
      katalima = "Aku ungkapin";
      kataenam = "Terus, aku ditolak";
      katatujuh = "Malu deh :(";
      katadelapan = "Makanya aku memilih diem... ";
      emot = "🙂";

      loadfoto(); await swalst.fire('Tunggu'); await swals.fire('Selamat datang!', 'Sekarang lihat ini ya :)'); setTimeout(showDiv, 300);
    } pertama();
  </script>
</body>

</html>
