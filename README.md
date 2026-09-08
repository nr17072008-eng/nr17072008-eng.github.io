# nr17072008-eng.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Happy Birthday Satyam 🎂</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      overflow-x: hidden;
      font-family: "Poppins", Arial, sans-serif;
      color: white;
      background: linear-gradient(
        135deg,
        #ff4ecd,
        #7b2ff7,
        #00c6ff,
        #00e5a8
      );
      background-size: 400% 400%;
      animation: gradient 10s ease infinite;
    }

    @keyframes gradient {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .container {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 30px 15px;
      text-align: center;
      position: relative;
      z-index: 2;
    }

    .card {
      width: min(650px, 95%);
      padding: 45px 25px;
      border-radius: 30px;
      background: rgba(255, 255, 255, 0.16);
      backdrop-filter: blur(15px);
      border: 2px solid rgba(255,255,255,0.3);
      box-shadow: 0 25px 60px rgba(0,0,0,0.25);
    }

    .emoji {
      font-size: 70px;
      animation: bounce 1.5s infinite;
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    .small-title {
      margin-top: 10px;
      font-size: 18px;
      letter-spacing: 4px;
      text-transform: uppercase;
    }

    h1 {
      margin: 12px 0;
      font-size: clamp(42px, 9vw, 80px);
      line-height: 1;
      font-weight: 900;
      color: #fff;
      text-shadow:
        0 0 10px #ffeb3b,
        0 0 25px #ff00c8,
        0 0 45px #00e5ff;
      animation: glow 2s ease-in-out infinite alternate;
    }

    @keyframes glow {
      from {
        transform: scale(1);
      }
      to {
        transform: scale(1.04);
      }
    }

    .name {
      color: #ffe600;
    }

    .message {
      margin: 25px auto;
      max-width: 530px;
      font-size: 18px;
      line-height: 1.8;
    }

    .cake {
      font-size: 80px;
      margin: 15px;
      animation: cake 2s ease-in-out infinite;
    }

    @keyframes cake {
      0%, 100% { transform: rotate(-3deg); }
      50% { transform: rotate(3deg) scale(1.08); }
    }

    .surprise-btn {
      border: none;
      padding: 16px 30px;
      border-radius: 50px;
      font-size: 17px;
      font-weight: bold;
      color: #7b2ff7;
      background: #fff;
      cursor: pointer;
      box-shadow: 0 8px 25px rgba(0,0,0,0.25);
      transition: 0.3s;
    }

    .surprise-btn:hover {
      transform: scale(1.08);
      background: #ffe600;
      color: #ff1493;
    }

    .surprise {
      display: none;
      margin-top: 25px;
      padding: 25px;
      border-radius: 20px;
      background: rgba(0,0,0,0.18);
      animation: appear 0.8s ease;
    }

    .surprise.show {
      display: block;
    }

    @keyframes appear {
      from {
        opacity: 0;
        transform: translateY(20px) scale(.9);
      }
      to {
        opacity: 1;
        transform: translateY(0) scale(1);
      }
    }

    .surprise h2 {
      color: #ffe600;
      margin-bottom: 12px;
      font-size: 30px;
    }

    .surprise p {
      line-height: 1.8;
      font-size: 17px;
    }

    .footer {
      margin-top: 25px;
      font-size: 14px;
      opacity: .9;
    }

    /* Balloons */
    .balloon {
      position: fixed;
      bottom: -120px;
      width: 55px;
      height: 70px;
      border-radius: 50%;
      z-index: 1;
      animation: fly linear infinite;
    }

    .balloon::after {
      content: "";
      position: absolute;
      width: 2px;
      height: 100px;
      background: rgba(255,255,255,.7);
      top: 68px;
      left: 50%;
    }

    .balloon::before {
      content: "";
      position: absolute;
      bottom: -8px;
      left: 22px;
      border-left: 6px solid transparent;
      border-right: 6px solid transparent;
      border-top: 10px solid currentColor;
    }

    @keyframes fly {
      from {
        transform: translateY(0) rotate(0deg);
      }
      to {
        transform: translateY(-120vh) rotate(20deg);
      }
    }

    .b1 {
      left: 5%;
      background: #ff1744;
      color: #ff1744;
      animation-duration: 9s;
    }

    .b2 {
      left: 18%;
      background: #ffe600;
      color: #ffe600;
      animation-duration: 12s;
      animation-delay: 2s;
    }

    .b3 {
      left: 80%;
      background: #00e5ff;
      color: #00e5ff;
      animation-duration: 10s;
      animation-delay: 1s;
    }

    .b4 {
      left: 92%;
      background: #76ff03;
      color: #76ff03;
      animation-duration: 13s;
      animation-delay: 3s;
    }

    .b5 {
      left: 45%;
      background: #ff00c8;
      color: #ff00c8;
      animation-duration: 11s;
      animation-delay: 4s;
    }

    /* Confetti */
    .confetti {
      position: fixed;
      top: -20px;
      width: 10px;
      height: 16px;
      z-index: 10;
      animation: fall 3s linear forwards;
    }

    @keyframes fall {
      to {
        transform: translateY(110vh) rotate(720deg);
      }
    }

    @media (max-width: 500px) {
      .card {
        padding: 35px 18px;
      }

      .emoji {
        font-size: 55px;
      }

      .message {
        font-size: 16px;
      }

      .cake {
        font-size: 65px;
      }
    }
  </style>
</head>

<body>

  <!-- Balloons -->
  <div class="balloon b1"></div>
  <div class="balloon b2"></div>
  <div class="balloon b3"></div>
  <div class="balloon b4"></div>
  <div class="balloon b5"></div>

  <main class="container">

    <
