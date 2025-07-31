<!DOCTYPE html>
<html lang="en">
<head>
  <meta http-equiv="content-type" content="text/html; charset=UTF-8">
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=0.5">
  <meta property="og:title" content="EchoLog">
  <meta property="og:description" content="United we command">
  <meta property="og:image" content="https://cdn.discordapp.com/avatars/1200458034573488168/2b2b1492430a325343c04f30cf2b6282.png?size=1024">
  <meta property="og:type" content="profile">
  <meta property="og:footer" content="EchoLog">

  <title>EchoLog</title>

  <!-- Local styles -->
  <link rel="stylesheet" href="echolog/tailwind.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
  <link rel="stylesheet" href="echolog/all.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
  <link rel="stylesheet" href="echolog/animate.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
  <link rel="stylesheet" href="echolog/minecraftia.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
  <link rel="stylesheet" href="echolog/were-beast-2.css" as="style" onload="this.onload=null;this.rel='stylesheet'">

  <!-- External libraries -->
  <noscript>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
    <link rel="stylesheet" href="https://fonts.cdnfonts.com/css/minecraftia">
    <link rel="stylesheet" href="https://fonts.cdnfonts.com/css/were-beast-2">
  </noscript>

  <script src="echolog/browser.js" type="text/javascript"></script>
  <script src="echolog/gsap.min.js" type="text/javascript"></script>
  <script src="echolog/iconify.min.js" type="text/javascript"></script>
  <script src="echolog/typed.umd.js" type="text/javascript"></script>
  <script src="echolog/jquery.min.js" type="text/javascript"></script>
  <script src="echolog/tilt.jquery.min.js" type="text/javascript"></script>

  <style>
    @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@500&display=swap');

    body, html {
      -webkit-user-drag: none;
      -webkit-user-select: none;
      user-select: none;
      margin: 0;
      padding: 0;
      width: 100%;
      height: 100%;
      overflow: hidden;
      font-family: 'Were-Beast', sans-serif !important;
      font-size: 17px;
      color: #FFFFFF;
      cursor: url(https://cdn.death.ovh/c00b6dec-1cdd-4a0f-972e-138e42f8c2aa.cur), auto;
    }

    .background-container {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      overflow: hidden;
      z-index: -1;
    }

    #backgroundVideo, #backgroundImage {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .card {
      position: relative;
      width: 700px;
      padding: 2rem;
      background: rgba(0, 0, 0, 0.14);
      backdrop-filter: blur(15px);
      border-radius: 23px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
      border-style: ridge;
      border-color: #FFFFFF;
      border-width: 4px;
      transform-style: preserve-3d;
      transform: perspective(1000px);
    }

    .card-content {
      display: flex;
      align-items: flex-start;
      left: 5px;
      transform: translateZ(50px);
    }

    .avatar {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
      position: relative;
      z-index: 1;
      border: 4px solid rgba(255, 255, 255, 0.2);
      background: linear-gradient(to right, #000000 0%, #FFFFFF 50%, #000000 70%);
      background-size: 200%;
      -webkit-background-clip: border-box;
      background-clip: border-box;
      animation: shine 3s linear infinite;
    }

    .username-badge-container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 1rem;
    }

    .tooltip {
      position: absolute;
      background-color: rgba(0, 0, 0, 0.8);
      color: white;
      padding: 8px 12px;
      border-radius: 8px;
      font-size: 0.85rem;
      z-index: 10000;
      opacity: 0;
      transition: opacity 0.3s ease, transform 0.3s ease;
      pointer-events: none;
      white-space: nowrap;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .tooltip-trigger:hover .tooltip {
      opacity: 1;
      pointer-events: auto;
    }

    @keyframes shine {
      0% { background-position: 150%; }
      100% { background-position: -50%; }
    }

    .shine {
      background-size: 200%;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: shine 3s linear infinite;
    }
  </style>
</head>
<body>
  <div class="background-container">
    <video id="backgroundVideo" autoplay muted loop></video>
    <img id="backgroundImage" src="" alt="">
  </div>

  <div class="card">
    <div class="card-content">
      <img src="https://cdn.discordapp.com/avatars/1200458034573488168/2b2b1492430a325343c04f30cf2b6282.png?size=1024" class="avatar" alt="Avatar">
      <div class="username-container">
        <h1 class="shine">EchoLog</h1>
      </div>
    </div>
  </div>
</body>
</html>
