<!DOCTYPE html>
<html lang="en"><head>
<meta http-equiv="content-type" content="text/html; charset=UTF-8">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=0.5">
<meta property="og:title" content="EchoLog">
<meta property="og:description" content="United we command ">
<meta property="og:image" content="https://cdn.discordapp.com/avatars/1200458034573488168/2b2b1492430a325343c04f30cf2b6282.png?size=1024">
<meta property="og:type" content="profile">
<meta property="og:footer" content="EchoLog">
<title>EchoLog</title>
<link rel="stylesheet" href="echolog/tailwind.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
<link rel="stylesheet" href="echolog/all.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
<link rel="stylesheet" href="echolog/animate.min.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
<link rel="stylesheet" href="echolog/minecraftia.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
<link rel="stylesheet" href="echolog/were-beast-2.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
<noscript>
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
        <link rel="stylesheet" href="https://fonts.cdnfonts.com/css/minecraftia">
        <link rel="stylesheet" href="https://fonts.cdnfonts.com/css/were-beast-2">
    </noscript>
<script async="" src="echolog/browser.js" type="text/javascript"></script>
<script async="" src="echolog/gsap.min.js" type="text/javascript"></script>
<script async="" src="echolog/iconify.min.js" type="text/javascript"></script>
<script async="" src="echolog/typed.umd.js" type="text/javascript"></script>
<script src="echolog/jquery.min.js" type="text/javascript"></script>
<script async="" src="echolog/tilt.jquery.min.js" type="text/javascript"></script>
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
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
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
        
        .user-info {
            margin-left: 2rem;
            flex-grow: 1;
        }

        .rainbow2 {
            animation: rainbow2 5s linear infinite;
        }

        @keyframes rainbow2 {
            0% { border-color: red; }
            14% { border-color: orange; }
            28% { border-color: yellow; }
            42% { border-color: green; }
            57% { border-color: blue; }
            71% { border-color: indigo; }
            85% { border-color: violet; }
            100% { border-color: red; }
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

        .username-container {
            position: relative;
        }

        .username-container .tooltip {
            bottom: 100%;
            left: 50%;
            transform: translateX(-50%);
            margin-bottom: 10px; 
        }

        .badge-container .tooltip {
            top: -40px; 
            left: 50%;
            transform: translateX(-50%);
        }

        .view-count-container {
            position: relative;
        }

        .view-count-container .tooltip {
            bottom: 100%;
            left: 50%;
            transform: translateX(-50%);
            margin-bottom: 10px;
            width: max-content; 
        }
        
        .username-container {
            position: relative;
        }

        @keyframes shine {
            0% {
              background-position: 150%;
            }
            100% {
              background-position: -50%;
            }
          }

        .shine {
            background-size: 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: shine 3s linear infinite;
        }
        .shineslow {
            background-size: 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: shine 5s linear infinite;
        }

        /* animation: shine 3s linear infinite;      background: linear-gradient(to right, #ffffff 0%, #000000 50%, #ffffff 70%); */
        .username {
            font-size: 1.8rem;
            font-weight: bold;
            margin: 0;
            
            background: linear-gradient(to right, #000000 0%, #FFFFFF 50%, #000000 70%);
            background-size: 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            
        }

        
        .badge-container {
            display: flex;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            padding: 5px 10px;
            overflow: visible;
            
        }
        
        .badge {
            width: 28px;
            height: 28px;
            margin-right: 8px;
            transition: transform 0.2s ease;
            
        }
        
        .badge:hover {
            transform: scale(1.1);
        }
        
        .description {
            font-size: 1rem;
            line-height: 1.5;
            margin-bottom: 0.5rem;
            white-space: nowrap;
            
            background: linear-gradient(to right, #000000 0%, #FFFFFF 50%, #000000 70%);
            background-size: 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            
        }

        .description_container {
            display: flex;
            align-items: center;
            justify-content: space-between;
            min-height: 32px;
        }
        
        .joined-date {
            color: #000000;
            font-size: 0.9rem;
            
            background: linear-gradient(to right, #000000 0%, #FFFFFF 50%, #000000 70%);
            background-size: 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            
        }
        
        .tooltip-trigger {
            position: relative; 
            display: inline-block;
        }
        .social-icons {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 50px;
            margin-top: 1rem;
            margin-bottom: 1rem;
            
            
        }
    
        .social-icon {
            
            font-size: 2.5rem;
            
            margin: 0 10px;
            color: #FFFFFFC7;
            transition: color 0.2s ease, transform 0.2s ease;
            padding-left: 0.5px;
            padding-right: 0.5px;
            display: inline-flex;
            align-items: center;
            justify-content: center;
        }

        .social-icon img {
            width: 2.5rem;
            height: 2.5rem;
            object-fit: contain; 
        }
        .social-icon2 {
            height: 51.2px;
            width: 51.2px;
            margin: 0 10px;
            color: #FFFFFFC7;
            transition: color 0.2s ease, transform 0.2s ease;
            padding-left: 0.5px;
            padding-right: 0.5px;
        }
        
        .social-icon2:hover {
            color: #000000;
            transform: scale(1.1);
        }

        .social-icon:hover {
            color: #000000;
            transform: scale(1.1);
        }

        .tooltip2-trigger {
            display: inline-flex;
            justify-content: center;
            align-items: center;
            width: 51.2px;
            height: 51.2px;
            position: relative;
        }

        .tooltip2 {
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
            left: 50%;
            transform: translateX(-50%);
            top: 100%; 
            margin-top: 5px; 
            
        }

        .tooltip2-trigger:hover .tooltip2 {
            opacity: 1;
            pointer-events: auto;
        }
        
        

        
        .tooltip-trigger:hover .tooltip {
            opacity: 1;
            pointer-events: auto;
        }
        

        
        

        
        
        
        .bottom-left-container {
            position: fixed;
            bottom: 0;
            left: 0;
            margin: 10px; 
            z-index: 1000; 
        }
        
        .eye-icon {
            margin-right: 5px; 
            
        }
        
        .view-count {
            font-size: 14px; 
        }
        
        #enterPage {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: black;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2em;
            cursor: pointer;
            z-index: 1000;
            opacity: 1;
            pointer-events: all;
            
        }
        
        .hidden {
            display: none;
        }
        
        .rpc-container {
            display: flex;
            align-items: center;
            width: 640px;
            height: 106px;
            overflow: hidden;
            margin-bottom: 1rem;
        }
        
        .avatar-container {
            position: relative;
            display: inline-block;
            scale: 1.1;
        }
        
        @keyframes fadeOut {
            from { opacity: 1; }
            to { opacity: 0; }
        }
        
        .fade-out {
            animation: fadeOut 1s forwards;
        }
        
        .rpc-avatar, .rpc-useravatar {
            width: 75px;
            height: 75px;
            min-width: 75px;
            border-radius: 25%;
            object-fit: cover;
        }

        .visualizer-border {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            border-radius: 20px;
            pointer-events: none;
            box-shadow: 0 0 0 rgba(255, 255, 255, 0.5);
            border: 4px solid transparent;
            transition: border 0.1s ease-in-out;
            box-sizing: border-box;
            
        }

        
        .rpc-avatar {
            margin-right: 5px;
            border: 4px solid rgba(255, 255, 255, 0.2);
        }

        .scalee {
            transform: scale(1.1);
            margin-left: 10px !important;
        }
        
        
        .rpc-useravatar {
            margin-left: 10px;
            border: 4px solid rgba(255, 255, 255, 0.2);
        }
        
        .status-container {
            position: absolute;
            bottom: 0;
            right: 0;
            width: 25px;
            height: 25px;
            transform: translate(25%, 25%);
        }
        
        .status-icon {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            scale: 0.8;
            transform: translate(-10px, -5px); 
        }
        
        .rpc-details {
            flex: 1;
            min-width: 0;
            overflow: hidden;
            
            padding-left: 10px;
        }
        
        .rpc-details h4, .rpc-details p {
            margin: 0;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }
        
        .rpc-details h4 {
            font-size: 1.2em;
            font-weight: bold;
        }
        
        .rpc-details p {
            font-size: 0.9em;
        }
        
        .rpc-username {
            font-size: 1em;
            font-weight: bold;
            margin: 0;
            padding-right: 10px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
            max-width: 150px;
            
        }
        
        .badgegrey {
            filter: grayscale(100) !important;
        }
        
        @media (max-width: 768px) {
            .rpc-container {
                width: 100%;
                height: auto;
                flex-direction: column;
                align-items: flex-start;
            }
        
            .rpc-avatar, .rpc-useravatar {
                margin-bottom: 0.5em;
            }
        
            .rpc-details, .rpc-username {
                width: 100%;
                max-width: 100%;
            }
        
            .rpc-details h4 {
                font-size: 1em;
            }
        
            .rpc-details p, .rpc-username {
                font-size: 0.8em;
            }
        }

        .social-icon-img {
            width: 51.2px;
            height: 51.2px;
            max-width: 9999999px !important;

        }
        
        .rainbow {
            animation: rainbow 5s linear infinite;
        }

        .discord-modal-content {
            background-color: black;
            margin: auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 500px;
            border-radius: 10px;
            box-shadow: inset 0px 0px 50px rgba(255, 255, 255, 0.35);
            position: relative;
        }

        .discord-close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }

        .discord-close:hover,
        .discord-close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }

        .discord-profile-container {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .discord-avatar {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            margin-right: 20px;
        }


        .discord-profile-info h2 {
            margin: 0;
            font-size: 1.5rem;
            font-weight: 600;
        }

        .discord-profile-info p {
            margin: 5px 0 0;
            color: #555;
        }

        .discord-button-container {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }

        .discord-modal-button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .discord-modal-button:hover {
            background-color: #45a049;
        }

        .discord-modal-button.discord-cancel {
            background-color: #f44336;
        }

        .discord-modal-button.discord-cancel:hover {
            background-color: #e53935;
        }
        
        .sparkles {
            animation: sparkle 1.5s infinite alternate;
        }
        
        .glow-text {
            text-shadow: 0 0 18px #000000;
        }
        
        .badge-glow {
            filter: drop-shadow(0 0 5px #000000);
        }
        
        .glass-effect {
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(5px);
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }
        
        .cursor-sparkle::after,
        .cursor-trail::after,
        .cursor-following-dot::after {
            content: '';
            display: block;
            position: fixed;
            pointer-events: none;
            transition: 0.1s;
        }
        
        .cursor-sparkle::after {
            width: 5px;
            height: 5px;
            background: #000000;
            border-radius: 50%;
        }
        
        .cursor-trail::after {
            width: 10px;
            height: 10px;
            border: 2px solid #000000;
            border-radius: 50%;
        }
        
        .cursor-following-dot::after {
            width: 20px;
            height: 20px;
            background: #000000;
            border-radius: 50%;
            opacity: 0.5;
        }
        
        .modal {
            display: none; 
            position: fixed; 
            z-index: 1000; 
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.6);
            display: flex; 
            align-items: center;
            justify-content: center;
            transition: opacity 0.3s ease-in-out;
            border-radius: 23px;
            animation: fadeIn 0.3s ease-in-out;
            box-shadow: inset 0px 0px 50px rgba(255, 255, 255, 0.35)
        }

        .modal-content {
            background-color: black;
            border-radius: 23px;
            padding: 30px;
            width: 90%;
            max-width: 400px;
            box-shadow: 0 15px 40px rgba(0,0,0,0.5); 
            position: relative;
            text-align: center;
            color: #f5f6fa; 
            box-shadow: inset 0px 0px 75px rgba(255, 255, 255, 0.35);
        }

        .close {
            position: absolute;
            top: 15px;
            right: 20px;
            color: #dcdde1;
            font-size: 22px;
            cursor: pointer;
            transition: color 0.3s ease;
        }

        .close:hover {
            color: #e74c3c; 
        }

        .modal-button {
            margin-top: 20px;
            padding: 12px 25px;
            background-color: #4CAF50; 
            color: white;
            border-radius: 30px;
            border: none;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }

        .modal-button:hover {
            background-color: #45a049;
            transform: scale(1.05);
        }

        .modal-button.cancel {
            background-color: #e74c3c; 
        }

        .modal-button.cancel:hover {
            background-color: #c0392b;
        }


        #modal-url {
            background-color: #2c3e50; 
            padding: 10px;
            border-radius: 8px;
            color: #ecf0f1; 
            font-weight: 600;
            word-break: break-word;
            margin-top: 10px;
            display: inline-block;
        }

        p {
            font-size: 18px;
            margin-bottom: 20px;
            line-height: 1.6;
        }


        .mutebutton {
            position: absolute;
            top: 10px; 
            left: 10px; 
            z-index: 1000; 
        }
        
        @keyframes rainbow {
            0% { color: red; }
            14% { color: orange; }
            28% { color: yellow; }
            42% { color: green; }
            57% { color: blue; }
            71% { color: indigo; }
            85% { color: violet; }
            100% { color: red; }
        }

        
        @keyframes sparkle {
            0% { text-shadow: 0 0 5px #fff, 0 0 10px #fff, 0 0 15px #fff; }
            100% { text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px #fff; }
        }
        
        .progress-bar-container {
            width: 100%;
            background-color: rgba(255, 255, 255, 0.2);
            border-radius: 5px;
            margin-top: 10px;
            height: 10px;
            overflow: hidden;
        }
        
        .progress-bar {
            height: 100%;
            width: 0;
            background-color: #1DB954;
            transition: width 0.75s ease-in-out;
        }
        
        .divide {
            position: absolute;
            top: 0;
            width: 100%;
            height: 3px;
            border-bottom: 1px solid #000;
            background: linear-gradient(to right, #1e5799 0%, #f300ff 50%, #e0ff00 100%);
            background-size: 100% 150%; 
            animation: moveGradient 3s linear infinite;
        }

        @keyframes moveGradient {
            0% {
                background-position: 0% 0%;
            }
            50% {
                background-position: 100% 100%;
            }
            100% {
                background-position: 0% 0%;
            }
        }
        

        #loading-screen {
            position: fixed;
            width: 100%;
            height: 100%;
            background-color: black;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 9999;
            pointer-events: none; 
            opacity: 0.95;
        }

        .loadingscreencard {
            background-color: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 1);
            text-align: center;
            color: white;
            
        }

        .loader {
            font-family: 'Arial', sans-serif;
            font-size: 28px;
            font-weight: bold;
            color: #ecf0f1; 
        }

        .fade-out {
            opacity: 0;
            transition: opacity 1s ease;
        }

        .welcome-text {
            font-size: 20px; 
            text-align: center; 
            display: block; 
        }

        #loading-text {
            font-size: 15px; 
            text-align: center; 
            display: block; 
        }



    </style>
</head>
<body class="bg-gray-900 flex items-center justify-center min-h-screen"><div id="loading-screen" class="fade-out" style="display: none;">
<div class="loader">
<div class="loadingscreencard">
<p class="welcome-text">Heil EchoLog.</p>
<span id="loading-text">Loading...</span>
</div>
</div>
</div>

<div class="divide"></div>
<div id="enterPage" class="fade-out" style="display: none;">CLICK CLICK CLICK !</div>
<div class="background-container">
<video id="backgroundVideo" loop="" playsinline="" style="display: none;" muted="muted" autoplay="autoplay" preload="auto">
<source src="echolog/7e11e373-6063-4911-8061-c990dd61a433.png" type="video/mp4">
</video>
<img id="backgroundImage" src="echolog/7e11e373-6063-4911-8061-c990dd61a433.png" alt="Background" style="display: block;">
</div>
<audio id="backgroundMusic" autoplay loop>
    <source src="echolog/Dorian.mp3" type="audio/mpeg">
</audio>

<script type="text/javascript">
    const backgroundMusic = document.getElementById('backgroundMusic');
    backgroundMusic.volume = 0.3; // Set volume to 30%

    // Add an error listener to debug any issues
    backgroundMusic.onerror = function () {
        console.error('Audio failed to load. Please check the file path or format.');
    };

    // Automatically play when the page loads
    window.addEventListener('DOMContentLoaded', () => {
        try {
            backgroundMusic.play();
        } catch (err) {
            console.error('Autoplay failed:', err);
        }
    });
</script>
<div class="flex flex-col space-y-8">
<div class="card" id="profileCard" style="will-change: transform; transform: perspective(300px) rotateX(0deg) rotateY(0deg);">
<div class="card-content">
<img src="https://leakz.win/Gentelo.jpg" alt="Avatar" class="avatar">
<div class="user-info">
<div class="username-badge-container">
<div class="username-container tooltip-trigger">
<h1 class="username shine glow-text">
EchoLog
</h1>
<div class="tooltip">
ID : 1
</div>
</div>
<div class="badge-container">
<div class="tooltip-trigger">
<img src="echolog/owner.gif" alt="Owner" class="badge badge-glow ">
<div class="tooltip">
CEO
</div>
</div>
<div class="tooltip-trigger">
<img src="echolog/verified.gif" alt="Verified" class="badge badge-glow ">
<div class="tooltip">
invuln rable
</div>
</div>
<div class="tooltip-trigger">
<img src="echolog/malware.gif" alt="Bug Hunter" class="badge badge-glow ">
<div class="tooltip">
3xploit Hunter !
</div>
</div>
<div class="tooltip-trigger">
<img src="echolog/leakz.png" alt="Leakz" class="badge badge-glow ">
<div class="tooltip">
Leakz"
</div>
</div>
</div>
</div>
<div class="description_container">
<p class="description shine">Echolog.ltd </p>
</div>
<p class="joined-date shine">Created 215 years ago.</p>
</div>
</div>
<div id="customlinkModal" class="modal" style="display: none;">
<div class="modal-content">
<span class="close" onclick="if (!window.__cfRLUnblockHandlers) return false; closeModal()"> </span>
<div id="modal-url"></div>
<div class="button-container">
<button class="modal-button" id="continue-button">Continue</button>
<button class="modal-button cancel" onclick="if (!window.__cfRLUnblockHandlers) return false; closeModal()">Cancel</button>
</div>
</div>
</div>
<div id="discordModal" class="modal" style="display: none;">
<div class="discord-modal-content">
<span class="discord-close" onclick="if (!window.__cfRLUnblockHandlers) return false; closeDiscordModal()"> </span>
<div class="discord-profile-container">
<img src="https://cdn.discordapp.com/avatars/1200458034573488168/2b2b1492430a325343c04f30cf2b6282.png?size=1024" alt="Avatar" class="discord-avatar">
<div class="discord-profile-info">
<h2>BusyBoxSatan</h2>
<p>ID: 1200458034573488168</p>
</div>
</div>
<div class="discord-button-container">
<button class="discord-modal-button" id="open-profile-button">Open Profile</button>
</div>
</div>
</div>
<div class="rpc-container glass-effect p-4" id="rpc-container">
<div class="avatar-container">
<img src="https://cdn.discordapp.com/avatars/1200458034573488168/2b2b1492430a325343c04f30cf2b6282.png?size=1024" onclick="if (!window.__cfRLUnblockHandlers) return false; ui.openDiscordModal()" alt="admin's Avatar" class="rpc-avatar" id="rpc-avataruser">
<div class="status-container">
<img src="echolog/dnd.webp" id="statusicon" alt="Status" class="status-icon">
</div>
</div>
<div class="rpc-details none">
<h4 id="rpc-details">EchoLog .</h4>
<p id="rpc-state" style="display: none;">.gg/telnet</p>
<p id="rpc-elapsedTime-container" style="display: none;">Elapsed: <span id="rpc-elapsedTime">00:00</span></p>
<div class="progress-bar-container hidden" style="display: none;">
<div class="progress-bar" id="progress-bar"></div>
</div>
</div>
<img src="echolog/None.htm" alt="RPC Avatar" class="rpc-avatar scalee" id="rpc-avatar" style="display: none;">
</div>
<div class="bottom-left-container">
<div class="view-count-container tooltip-trigger">
<label for="view-count" class="flex items-center mt-4">
<span id="view-count" class="view-count">666</span>
</label>
<div class="tooltip">
Body Count :
</div>
</div>
</div>
<div class="js-tilt-glare" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; overflow: hidden; pointer-events: none;"><div class="js-tilt-glare-inner" style="position: absolute; top: 50%; left: 50%; background-image: linear-gradient(0deg, rgba(255, 255, 255, 0) 0%, rgb(255, 255, 255) 100%); width: 1400px; height: 1400px; transform: rotate(180deg) translate(-50%, -50%); transform-origin: 0% 0% 0px; opacity: 0;"></div></div><div class="visualizer-border" style="box-shadow: rgb(255, 255, 255) 0px 0px 0px 0px;"></div><div class="visualizer-border" style="box-shadow: rgb(255, 255, 255) 0px 0px 0px 0px;"></div></div>
</div>
<script type="text/javascript">
        
        window.addEventListener('load', function() {
            const loadingScreen = document.getElementById('loading-screen');
            const content = document.getElementById('content');
            const loadingScreenText = document.getElementById('loading-text');
            const loadingDots = document.getElementById('loading-dots');
            
            loadingScreen.classList.add('fade-out');
            
            
            setTimeout(function() {
                loadingScreen.style.display = 'none';
                content.style.display = 'block';
                content.style.opacity = '1';
                
                document.body.style.overflow = 'auto';
            }, 750);  
        });

        (function animateLoading() {
            const loadingText = document.getElementById('loading-text');
            const loadingDots = document.getElementById('loading-dots');

            let dots = '';
            setInterval(function() {
                dots = dots.length >= 3 ? '' : dots + '.';
                loadingText.innerText = 'Loading' + dots;
            }, 500);
        })();
        (() => {
            const elements = {
                customlinkModal: document.getElementById('customlinkModal'),
                modalUrl: document.getElementById('modal-url'),
                continueButton: document.getElementById('continue-button'),
                discordModal: document.getElementById('discordModal'),
                openProfileButton: document.getElementById('open-profile-button'),
                rpcElements: {
                    avatar: document.getElementById('rpc-avatar'),
                    details: document.getElementById('rpc-details'),
                    state: document.getElementById('rpc-state'),
                    elapsedTime: document.getElementById('rpc-elapsedTime'),
                    elapsedTimeContainer: document.getElementById('rpc-elapsedTime-container'),
                    avatarUser: document.getElementById('rpc-avataruser'),
                    statusIcon: document.getElementById('statusicon'),
                    progressBarContainer: document.querySelector('.progress-bar-container')
                },
                enterPage: document.getElementById('enterPage'),
                backgroundVideo: document.getElementById('backgroundVideo'),
                backgroundImage: document.getElementById('backgroundImage'),
                backgroundMusic: document.getElementById('backgroundMusic'),
                viewCount: document.getElementById('view-count'),
                profileCard: document.getElementById('profileCard'),
                muteButton: document.getElementById('muteButton')
            };

            const state = {
                devToolsOpen: false,
                audioCurrentTime: 0,
                audioVolume: 0.30
            };

            const utils = {
                convertTimeToSeconds: (time) => {
                    const [minutes, seconds] = time.split(':').map(Number);
                    return minutes * 60 + seconds;
                },
                extractColorsFromAlbumArt: (imageUrl) => {
                    const img = new Image();
                    img.crossOrigin = "Anonymous";
                    img.src = imageUrl;
                    img.onload = () => {
                        const canvas = document.createElement('canvas');
                        const ctx = canvas.getContext('2d');
                        canvas.width = img.width;
                        canvas.height = img.height;
                        ctx.drawImage(img, 0, 0, img.width, img.height);

                        const imageData = ctx.getImageData(0, 0, canvas.width, canvas.height).data;
                        const colorCounts = {};

                        for (let i = 0; i < imageData.length; i += 4) {
                            const rgb = `rgb(${imageData[i]},${imageData[i + 1]},${imageData[i + 2]})`;
                            colorCounts[rgb] = (colorCounts[rgb] || 0) + 1;
                        }

                        const sortedColors = Object.entries(colorCounts).sort((a, b) => b[1] - a[1]);
                        const primaryColor = sortedColors[0][0];
                        const secondaryColor = sortedColors[Math.floor(sortedColors.length / 2)][0];

                        utils.applyColorsToProgressBar(primaryColor, secondaryColor);
                    };
                },
                applyColorsToProgressBar: (primaryColor, secondaryColor) => {
                    const progressBarFill = document.querySelector('.progress-bar');
                    progressBarFill.style.background = `linear-gradient(90deg, ${primaryColor}, ${secondaryColor})`;
                },
                copyToClipboard: (text, element) => {
                    navigator.clipboard.writeText(text).then(() => {   
                        const tooltip = element.nextElementSibling;
                        const originalText = tooltip.textContent;
                        tooltip.textContent = "Copied!";
                        tooltip.style.opacity = "1";
                        
                        setTimeout(() => {
                            tooltip.textContent = originalText;
                            tooltip.style.opacity = "0";
                        }, 2000);
                    }).catch(err => {
                        console.error('Failed to copy address:', err);
                        alert('Failed to copy address');
                    });
                }
            };

            const rpc = {
                fetchRPCData: async () => {
                    if ('1201465397988315158' === 'unset') {
                        console.log('discord_id is unset, not sending API call.');
                        return; 
                    }
                
                    try {
                        const response = await fetch('/api/rpc/1201465397988315158');
                        const data = await response.json();
                        console.log('Fetched RPC data:', data);
                        if (data.rpc) {
                            rpc.updateRPCDisplay(data.rpc);
                        }
                    } catch (error) {
                        console.error('Error fetching RPC data:', error);
                    }
                },
                updateRPCDisplay: (rpcData) => {
                    const e = elements.rpcElements;
                    if (rpcData.largeImage !== "None") {
                        e.avatar.src = rpcData.largeImage;
                        e.avatar.style.display = 'block';
                    } else {
                        e.avatar.style.display = 'none';
                    }
                    e.avatarUser.src = rpcData.avatarUrl;
                    e.statusIcon.src = rpcData.statusicon;

                    if (rpcData.details === rpcData.state) {
                        e.state.style.display = 'none';
                        e.details.textContent = rpcData.details;
                    } else {
                        e.details.style.display = 'block';
                        e.details.textContent = rpcData.details;
                        e.state.textContent = rpcData.state;
                    }

                    if (rpcData.spotify) {
                        e.elapsedTimeContainer.style.display = 'none';
                        e.progressBarContainer.style.display = 'block';
                        e.state.textContent = rpcData.state;
                        rpc.updateSpotifyProgress(rpcData.elapsedTime, rpcData.totalTime);
                        utils.extractColorsFromAlbumArt(rpcData.largeImage);
                    } else {
                        e.progressBarContainer.style.display = 'none';
                        if (rpcData.elapsedTime && rpcData.elapsedTime !== '00:00') {
                            e.elapsedTimeContainer.style.display = 'block';
                            e.elapsedTime.textContent = rpcData.elapsedTime;
                        } else {
                            e.elapsedTimeContainer.style.display = 'none';
                        }
                    }
                },
                updateSpotifyProgress: (elapsedTime, totalTime) => {
                    const elapsedSeconds = utils.convertTimeToSeconds(elapsedTime);
                    const totalSeconds = utils.convertTimeToSeconds(totalTime);
                    const progressPercentage = (elapsedSeconds / totalSeconds) * 100;
                    
                    const progressBar = document.getElementById('progress-bar');
                    progressBar.style.width = `${progressPercentage}%`;
                }
            };

            const ui = {
                openModal: (url) => {
                    elements.modalUrl.textContent = url;
                    elements.continueButton.onclick = () => {
                        window.open(url, '_blank');
                        ui.closeModal();
                    };
                    elements.customlinkModal.style.display = 'flex';
                },
                closeModal: () => {
                    elements.customlinkModal.style.display = 'none';
                },
                openDiscordModal: () => {
                    elements.discordModal.style.display = 'flex';
                },
                closeDiscordModal: () => {
                    elements.discordModal.style.display = 'none';
                },
        
        
                toggleMute: () => {
                    elements.backgroundMusic.muted = !elements.backgroundMusic.muted;
                    elements.muteButton.textContent = elements.backgroundMusic.muted ? 'Unmute' : 'Mute';
                },
                initEnterPage: () => {
                    elements.enterPage.addEventListener('click', () => {
                        elements.enterPage.classList.add('fade-out');
                        setTimeout(() => {
                            elements.enterPage.style.display = 'none';
                        }, 750);

                        
                        const ext = 'png';
                        if (ext === 'mp4' || ext === 'webm') {
                            elements.backgroundVideo.style.display = 'block';
                            elements.backgroundVideo.play();
                        } else {
                            elements.backgroundImage.style.display = 'block';
                        }
                        

                        
                        elements.backgroundMusic.volume = state.audioVolume;
                        elements.backgroundMusic.play();
                        

                        ui.animateViewCount();
                        
                        ui.initVisualizer();
                        
                    });
                },
                animateViewCount: () => {
                    let count = 0;
                    const target = 1139;
                    const duration = 3500; 
                    const increment = target / (duration / 50);

                    const counter = setInterval(() => {
                        count += increment;
                        if (count >= target) {
                            count = target;
                            clearInterval(counter);
                        }
                        elements.viewCount.textContent = Math.floor(count);
                    }, 50);
                },
                initVisualizer: () => {
                    const mediaElement = elements.backgroundMusic;
                    mediaElement.crossOrigin = "anonymous";
                
                    const context = new (window.AudioContext || window.webkitAudioContext)();
                    const src = context.createMediaElementSource(mediaElement);
                    const analyser = context.createAnalyser();
                
                    src.connect(analyser);
                    analyser.connect(context.destination);
                
                    analyser.fftSize = 2048;
                    analyser.minDecibels = -90;
                    analyser.maxDecibels = -10;
                    analyser.smoothingTimeConstant = 0.75;
                    const bufferLength = analyser.frequencyBinCount;
                    const dataArray = new Uint8Array(bufferLength);
                
                    const visualizerBorder = document.createElement('div');
                    visualizerBorder.className = 'visualizer-border';
                    elements.profileCard.appendChild(visualizerBorder);
                
                    const renderFrame = () => {
                        requestAnimationFrame(renderFrame);
                        analyser.getByteFrequencyData(dataArray);
                
                        const bassFrequencies = dataArray.slice(0, 10);
                        const sumBass = bassFrequencies.reduce((a, b) => a + b, 0);
                        const averageBass = sumBass / bassFrequencies.length;
                        const userDefinedIntensity = 200; 
                        const borderIntensity = Math.max(0, (averageBass / 400) * userDefinedIntensity);
                
                        visualizerBorder.style.boxShadow = `0 0 ${borderIntensity}px ${borderIntensity * 0.5}px #FFFFFF`;
                    };
                
                    mediaElement.play().then(() => {
                        console.log('Media playing');
                        renderFrame();
                    }).catch(e => console.error('Error playing media:', e));
                }
            };

            elements.openProfileButton.onclick = () => {
                window.open('https://discord.com/users/1200458034573488168', '_blank');
                ui.closeDiscordModal();
            };

            const security = {
                detectDevTools: () => {
                    const threshold = 200;
                    const widthThreshold = window.outerWidth - window.innerWidth > threshold;
                    const heightThreshold = window.outerHeight - window.innerHeight > threshold;
                    if (widthThreshold || heightThreshold) {
                        if (!state.devToolsOpen) {
                            if (elements.backgroundMusic) {
                                state.audioCurrentTime = elements.backgroundMusic.currentTime;
                                elements.backgroundMusic.pause();
                            }
                            state.cache = document.body.innerHTML;
                            document.body.innerHTML = '';
                            debugger;
                            state.devToolsOpen = true;
                        }
                    } else if (state.devToolsOpen) {
                        document.body.innerHTML = state.cache;
                        if (elements.backgroundMusic) {
                            elements.backgroundMusic.currentTime = state.audioCurrentTime;
                            elements.backgroundMusic.volume = state.audioVolume;
                            elements.backgroundMusic.play();
                        }
                        state.devToolsOpen = false;
                    }
                },
                preventDefaultActions: () => {
                    document.addEventListener('contextmenu', e => e.preventDefault());
                    document.addEventListener('keydown', e => {
                        if ((e.ctrlKey && e.shiftKey && ['I', 'C', 'J'].includes(e.key)) ||
                            (e.ctrlKey && ['U', 'S'].includes(e.key)) || e.key === 'F12') {
                            e.preventDefault();
                        }
                    });
                    document.addEventListener('dragstart', e => e.preventDefault());
                    document.addEventListener('selectstart', e => e.preventDefault());
                }
            };

            const init = () => {
            if (
                typeof cursoreffects !== 'undefined' &&
                typeof Typed !== 'undefined' &&
                typeof $ !== 'undefined' &&
                $.fn.tilt
            ) {
                elements.customlinkModal.style.display = 'none';
                elements.discordModal.style.display = 'none';
                
                setInterval(rpc.fetchRPCData, 5000);
                rpc.fetchRPCData();
                

                security.preventDefaultActions();
                setInterval(security.detectDevTools, 500);

                window.onclick = event => {
                    if (event.target == elements.customlinkModal) {
                        ui.closeModal();
                    }
                    if (event.target == elements.discordModal) {
                        ui.closeDiscordModal();
                    }
                };

                ui.initEnterPage();

                
                new Typed('.description', {
                    strings: ["https://leakz.win/"],
                    typeSpeed: 100,
                    backSpeed: 50,
                    loop: true,
                    startDelay: 500,
                    backDelay: 2000,
                    cursorChar: "|",
                    autoInsertCss: false,
                    showCursor: false,
                });
                

                
                $('.card').tilt({
                    maxTilt: 7,
                    speed: 1000,
                    perspective: 300,
                    easing: "cubic-bezier(.03,.98,.52,.99)",
                    glare: true,
                    maxGlare: 0.1
                });
                

                
                if ("sparkles".includes("sparkle")) {
                    new cursoreffects.fairyDustCursor({
                        colors: ["#000000"],
                    });
                }
                if ("sparkles".includes("following-dot")) {
                    new cursoreffects.followingDotCursor({ color: ["#000000"] });
                }
                if ("sparkles".includes("trail")) {
                    new cursoreffects.trailingCursor({particles: 15, rate: 0.8});
                }
                
            } else {
                setTimeout(init, 100);
            }
        };

        if (document.readyState === 'loading') {
            ui.initEnterPage();
            document.addEventListener('DOMContentLoaded', init);
        } else {
            init();
        }

        window.openModal = ui.openModal;
        window.closeModal = ui.closeModal;
        window.copyToClipboard = utils.copyToClipboard;
        window.toggleMute = ui.toggleMute;
        document.querySelector('.discord-close').onclick = ui.closeDiscordModal;
        document.getElementById('rpc-avataruser').onclick = ui.openDiscordModal;
        })();


    </script>
<script defer="defer" src="echolog/vcd15cbe7772f49c399c6a5babf22c1241717689176015" integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ==" data-cf-beacon="{&quot;rayId&quot;:&quot;8cc55c279dbb657c&quot;,&quot;version&quot;:&quot;2024.8.0&quot;,&quot;r&quot;:1,&quot;token&quot;:&quot;8744020a8bd24cd9ae7f1f7f7cf3518a&quot;,&quot;serverTiming&quot;:{&quot;name&quot;:{&quot;cfExtPri&quot;:true,&quot;cfL4&quot;:true}}}" crossorigin="anonymous"></script>

<canvas style="top: 0px; left: 0px; pointer-events: none; position: fixed;" width="1920" height="955"></canvas></body></html>
