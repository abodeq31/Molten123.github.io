
<html lang="en-US">
<meta http-equiv="content-type" content="text/html; charset=UTF-8">
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">

<!-- Begin Jekyll SEO tag v2.8.0 -->
<title>by Molten</title>
<meta name="generator" content="Jekyll v3.10.0">
<meta property="og:title" content="">
<meta property="og:locale" content="en_US">
<link rel="canonical" href="Molteng.github.io">
<meta property="og:url" content="Molteng.github.io/">
<meta property="og:site_name" content="Molteng.github.io">
<meta property="og:type" content="website">
<meta name="twitter:card" content="summary">
<meta property="twitter:title" content="Molteng.github.io">
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"WebSite","headline":"Molteng.github.io","name":"Molteng.github.io","url":"https://abodeq31.github.io/Molteng.github.io/"}</script>
<!-- End Jekyll SEO tag -->

    <link rel="stylesheet" href="Molteng321_files/style.css">
    <!-- start custom head snippets, customize with your own _includes/head-custom.html file -->

<!-- Setup Google Analytics -->



<!-- You can set your favicon here -->
<!-- link rel="shortcut icon" type="image/x-icon" href="/Molteng.github.io/favicon.ico" -->

<!-- end custom head snippets -->



    <div class="container-lg px-3 my-5 markdown-body">
      
      <h1><a></a></h1>
      

      <p></p>

  
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Molten WAS HERE!</title>
  
  
    <canvas id="myCanvas" width="1920" height="947"></canvas>

    <div class="custom-cursor" style="left: 782px; top: 425px;"></div>

    <style>
      #myCanvas {
        position: absolute;
      }

      .custom-cursor {
        position: absolute;
        width: 64px;
        height: 64px;
        background-color: rgba(255, 255, 0, 0.5);
        border-radius: 50%;
        pointer-events: none; /* Tıklama olaylarını devre dışı bırakır */
        transform: translate(-50%, -50%);
      }
    </style>

    <script>
      document.addEventListener("DOMContentLoaded", function () {
        const cursor = document.querySelector(".custom-cursor");

        document.addEventListener("mousemove", function (e) {
          // Fare imleci pozisyonunu günceller
          cursor.style.left = e.clientX + "px";
          cursor.style.top = e.clientY + "px";
        });

        document.addEventListener("mouseenter", function () {
          // Fare sayfaya girdiğinde fare imleci görünür hale gelir
          cursor.style.opacity = 1;
        });

        document.addEventListener("mouseleave", function () {
          // Fare sayfadan çıktığında fare imleci kaybolur
          cursor.style.opacity = 0;
        });
      });
    </script>

    <script>
      const canvas = document.getElementById("myCanvas");
      const ctx = canvas.getContext("2d");
      const points = [];

      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;

      function generateRandomPoint() {
        return {
          x: Math.random() * canvas.width,
          y: Math.random() * canvas.height,
          radius: Math.random() * 5 + 1, // Nokta yarıçapı
        };
      }

      function drawPoint(point) {
        ctx.beginPath();
        ctx.arc(point.x, point.y, point.radius, 0, Math.PI * 2);
        ctx.fillStyle = "white"; // Beyaz renk
        ctx.fill();
        ctx.closePath();
      }

      function update() {
        ctx.clearRect(0, 0, canvas.width, canvas.height);

        for (let i = 0; i < points.length; i++) {
          drawPoint(points[i]);
          points[i].x += (Math.random() - 0.5) * 2; // Rastgele x hareketi
          points[i].y += (Math.random() - 0.5) * 2; // Rastgele y hareketi

          // Ekrandan çıkan noktaları tekrar ekrana getir
          if (
            points[i].x < 0 ||
            points[i].x > canvas.width ||
            points[i].y < 0 ||
            points[i].y > canvas.height
          ) {
            points[i] = generateRandomPoint();
          }
        }

        requestAnimationFrame(update);
      }

      // İlk noktaları oluştur
      for (let i = 0; i < 100; i++) {
        points.push(generateRandomPoint());
      }

      // Tarayıcı boyutu değiştikçe canvas boyutunu güncelle
      window.addEventListener("resize", () => {
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;
      });

      update(); // HHa Fuck you 
    </script>

    <h1 class="nmt">https://discord.gg/LLLL  -   ALZAABI TEAM

    </h1><h1 class="name" data-value="Hacked By . /0Ld Scream and Molten">Hacked By . /0Ld Scream and Molten</h1>

    <div class="image"></div>

    <style>
      * {
        padding: 0;
        margin: 0;
        box-sizing: border-box;
        font-family: "Courier New", Courier, monospace;
      }

      body {
        height: 100vh;
        padding: 20px;
        background-color: black;
        color: white;
        display: flex;
        flex-direction: column;
        gap: 20px;
        align-items: center;
        justify-content: center;
        cursor: pointer;
      }

      ::-webkit-scrollbar {
        width: 0px;
        height: 0px;
      }

      .image {
        height: 450px;
        width: 1000px;
        background: url(https://i.postimg.cc/yxdcGTbc/hitlore.gif);
        border: 2px solid white;
        border-radius: 3px;
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
      }

      .name {
        color: white;
        padding: 0rem clamp(1rem, 2vw, 3rem);
        border-radius: clamp(0.4rem, 0.75vw, 1rem);
        z-index: 999;
      }

      .name:hover {
        background-color: white;
        color: black;
      }

      .nmt {
        color: red;
        text-shadow: 0px 0px 10px red;
      }

      @media (max-width: 1100px) {
        .image {
          width: 100%;
        }
      }
    </style>

    <script>
      const letters = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

      let interval = null;

      document.querySelector(".name").onmouseover = (event) => {
        let iteration = 0;

        clearInterval(interval);

        interval = setInterval(() => {
          event.target.innerText = event.target.innerText
            .split("")
            .map((letter, index) => {
              if (index < iteration) {
                return event.target.dataset.value[index];
              }

              return letters[Math.floor(Math.random() * 26)];
            })
            .join("");

          if (iteration >= event.target.dataset.value.length) {
            clearInterval(interval);
          }

          iteration += 1 / 3;
        }, 30);
      };
    </script></div>
    <script src="Molteng321_files/anchor.min.js" integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
    <script>anchors.add();</script>

     <!-- Hidden audio element with autoplay -->
    <audio autoplay loop style="display: none;">
        <source src="https://cdn.discordapp.com/attachments/1280294550841331845/1291870243374895186/-snap_mg.vc__ezmp3.cc_.mp3?ex=6701ab6b&is=670059eb&hm=2aa32f0e53ed132e5ceba27be241685125c9bccd071f259fbbe3f6ae0c9c727c&" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
  
