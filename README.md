      white-space: pre-line;
    }

    .love {
      font-size: 30px;
      margin-top: 20px;
      animation: beat 1s infinite;
    }

    .btn {
      margin-top: 20px;
      padding: 10px 20px;
      background: white;
      color: black;
      border-radius: 10px;
      cursor: pointer;
      display: inline-block;
    }

    @keyframes beat {
      0% {transform: scale(1);}
      50% {transform: scale(1.2);}
      100% {transform: scale(1);}
    }

    .heart {
      position: fixed;
      top: -10px;
      color: red;
      font-size: 20px;
      animation: fall linear infinite;
      z-index: 1;
    }

    @keyframes fall {
      0% {transform: translateY(-10px); opacity: 1;}
      100% {transform: translateY(100vh); opacity: 0;}
    }
  </style>
</head>
<body>

<script>
function createHeart() {
  const heart = document.createElement("div");
  heart.classList.add("heart");
  heart.innerHTML = "❤️";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.animationDuration = (Math.random() * 3 + 2) + "s";
  document.body.appendChild(heart);

  setTimeout(() => {
    heart.remove();
  }, 5000);
}
setInterval(createHeart, 300);
</script>

<div class="container">
  <h1>Happy Anniversary, Sayang ❤️</h1>

  <p>
Happy anniversary, sayang ❤️

Gak kerasa ya waktu jalan sejauh ini… dari dua orang asing, sampai sekarang kamu jadi rumah yang paling aku butuhin. Banyak banget momen yang kita lewatin bareng, tawa, air mata, dan semua cerita yang gak akan pernah aku lupain seumur hidup.

Jujur, aku sering takut… takut kehilangan kamu, takut suatu saat kamu pergi, karena buat aku kamu bukan cuma sekadar pasangan, tapi kamu adalah bagian dari hidup aku yang paling berharga.

Makasih ya udah selalu ada, udah sabar, udah nerima aku apa adanya, bahkan di saat aku lagi gak baik-baik aja. Aku tau aku belum sempurna, tapi satu hal yang pasti… perasaan aku ke kamu selalu tulus, dan gak pernah main-main.

Kalau suatu hari nanti kita diuji lagi, aku cuma berharap kita bisa tetep saling genggam, bukan saling lepas. Karena aku bener-bener mau kamu, bukan cuma hari ini, tapi untuk waktu yang lama.

Jujur, selama sama kamu aku ngerasain hal yang belum pernah aku rasain sebelumnya. Kamu bikin aku ngerasa cukup, ngerasa dihargai, dan ngerasa punya seseorang yang bener-bener aku perjuangin. Tapi di balik itu semua, aku juga sering ngerasa takut… takut kehilangan kamu, takut kalau suatu saat nanti aku gak bisa lagi manggil kamu “punya aku”.

Maaf ya kalau selama ini aku masih banyak kurangnya. Maaf kalau aku kadang bikin kamu capek, atau belum bisa jadi yang terbaik sepenuhnya buat kamu. Tapi percayalah, di setiap kurangnya aku, selalu ada usaha buat tetep jadi lebih baik… demi kamu, demi kita.

Aku gak pernah tau masa depan bakal gimana, tapi satu hal yang aku tau… aku selalu mau ada kamu di setiap langkah aku. Aku mau kita tetep bareng, tetep saling genggam, walaupun nanti jalannya gak selalu mudah. Karena buat aku, kehilangan kamu itu bukan hal yang bisa aku bayangin.

Kamu itu bukan cuma pasangan buat aku… kamu itu rumah. Tempat aku pulang, tempat aku cerita, tempat aku ngerasa tenang. Dan jujur aja, aku gak tau harus gimana kalau suatu hari nanti aku harus kehilangan semua itu.

Kalau kamu tanya seberapa besar aku sayang kamu… jawabannya lebih dari yang bisa aku jelasin. Lebih dari kata-kata ini, lebih dari yang bisa aku tunjukin. Aku sayang kamu dengan cara yang mungkin gak selalu sempurna, tapi selalu tulus dari hati yang paling dalam.

Aku harap kita gak cuma bertahan sampai hari ini, tapi bisa terus jalan bareng sampai waktu yang panjang… sampai kita bisa ngeliat ke belakang dan bilang, “ternyata kita berhasil lewatin semuanya bareng.”

Terima kasih udah jadi bagian terindah dalam hidup aku. Terima kasih udah tetap ada sampai sekarang. Dan tolong… tetap di sini ya, sama aku.

I love you, selalu ❤️

Dari orang favoritmu, Rayhan Surya
  </p>

  <div class="love">❤️</div>

  <div class="btn" onclick="playMusic()">Putar Musik 🎵</div>
</div>

<audio id="music" loop>
  <source src="https://www.bensound.com/bensound-music/bensound-romantic.mp3" type="audio/mp3">
</audio>

<script>
function playMusic() {
  document.getElementById("music").play();
}

window.onload = function() {
  let music = document.getElementById("music");
  music.play().catch(() => {});
}
</script>

</body>
</html>
