<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Just One Question ❤️</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0;
      overflow: hidden;
      position: relative;
    }

    .card {
      background: white;
      padding: 2.5rem;
      border-radius: 20px;
      max-width: 500px;
      width: 90%;
      text-align: center;
      box-shadow: 0 20px 40px rgba(0,0,0,0.15);
      position: relative;
      z-index: 10;
    }

    h1 {
      color: #e75480;
      font-size: 2rem;
    }

    h2 {
      font-size: 1.6rem;
      margin-top: 1.5rem;
    }

    h3 {
      font-size: 1.4rem;
      margin-top: 1rem;
    }

    p {
      font-size: 1.1rem;
      line-height: 1.6;
      margin: 0.8rem 0;
    }

    .buttons {
      margin-top: 2rem;
      display: flex;
      justify-content: center;
      gap: 1rem;
    }

    button {
      padding: 0.85rem 1.8rem;
      border-radius: 999px;
      border: none;
      font-size: 1.1rem;
      cursor: pointer;
    }

    #yesBtn { background: #ff5f8a; color: white; }
    #noBtn { background: #ddd; }

    .hidden { display: none; }

    #giftSection, #yesMessage {
      margin-top: 2rem;
      animation: fadeIn 0.6s ease;
    }

    #giftSection a {
      display: inline-block;
      margin-top: 1rem;
      padding: 0.85rem 1.8rem;
      background: #ff5f8a;
      color: white;
      text-decoration: none;
      border-radius: 999px;
      font-size: 1.1rem;
    }

    .confetti, .heart {
      position: fixed;
      z-index: 5;
      pointer-events: none;
    }

    .confetti {
      width: 10px;
      height: 10px;
      animation: fall 3s linear forwards;
    }

    .heart {
      width: 20px;
      height: 20px;
      background: url('data:image/svg+xml;utf8,<svg fill="red" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32"><path d="M23.6 4c-2.2 0-4.2 1-5.6 2.6C16.6 5 14.6 4 12.4 4 8.6 4 5.6 7 5.6 10.8c0 5.2 10.4 14.4 10.4 14.4s10.4-9.2 10.4-14.4C28.4 7 25.4 4 23.6 4z"/></svg>') no-repeat center/contain;
      animation: floatUp linear infinite;
      opacity: 0.7;
    }

    @keyframes fall {
      to { transform: translateY(100vh) rotate(360deg); opacity: 0; }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.95); }
      to { opacity: 1; transform: scale(1); }
    }

    @keyframes floatUp {
      0% { transform: translateY(100vh) translateX(0) scale(0.8); opacity: 0; }
      10% { opacity: 1; }
      100% { transform: translateY(-10vh) translateX(50px) scale(1); opacity: 0; }
    }
  </style>
</head>
<body>

  <div class="card" id="mainCard">
    <!-- First screen content -->
    <div id="questionScreen">
      <h1>Hewwo there pwincess ❤️</h1>
      <p>Its been long overdue and something Ive been meaning to do, but i haven't done yet and that is to officially make you mine.</p>
      <p>I don't want blurred lines of what you mean to me. i want it to be as clear to you and everyone else that i am committed to loving you.</p>
      <p>i want to go through the boring days, the hard days, and the days where we love each other the most. I want to live every day from now on knowing Im yours and you are mine and that we can rely on each other and place our emotions, and our hearts in one another.</p>
      <p>So even if we do get hurt sometimes, its a promise that we will work through it together. It was my mistake to let you doubt for so long... but all thats left now is form me to ask you one question baby.</p>

      <h2>Will you make me the happiest man in in the world and allow me ot be your boyfriend? 💕</h2>

      <div class="buttons" id="questionButtons">
        <button id="yesBtn">Yes make me an oxford study plss 💖</button>
        <button id="noBtn">No you must remain a cuck! 🙈</button>
      </div>
    </div>
    
<!-- Inside your .card div, at the very end -->
<div id="footnote" style="
    font-size: 0.9rem;
    color: #888;
    margin-top: 2rem;
    text-align: center;
">
  * Come and get this 8 inch
</div>


    <!-- Second screen content -->
    <div id="yesMessage" class="hidden">
      <h2>LESGOO BABBYYY</h2>
      <p>YES YES YES YES BABES THIS WAS ALL ME SO DON'T GO AND TAKE THE CREDIT BY SAYING I ONLY DID THIS FOR YOU AND WHAT NOT YADDA YADDA YADDA</p>
	  <p>but on a more serious note baby i appreciate you so much and I am SOOO excited for this chapter we have ahead of us! I can't wait for all the sweet sweet memories( and esex) we will get to make together. And maybe, JUST MAYBE ill be able to take you on our very first date sooner than we hoped!</p>
      <p>I can't believer I FINALLY GET TO CALL YOU MY GIRL.. WAIT FOR IT.. FRIEND!<p>
      <div id="giftSection">
        <h3>And yess heres your reward for being such a good girl for me baby</h3>
        <a href="https://share.icloud.com/photos/078R_v6XCBbGcxp4R-ll-0jrg" target="_blank">SPANK BANK 💕</a>
      </div>
    </div>
  </div>

  <script>
    const yesBtn = document.getElementById('yesBtn');
    const noBtn = document.getElementById('noBtn');
    const questionScreen = document.getElementById('questionScreen');
    const yesMessage = document.getElementById('yesMessage');

    // No button dodge
    noBtn.addEventListener('mouseover', () => {
      noBtn.style.position = 'absolute';
      noBtn.style.top = Math.random() * 80 + '%';
      noBtn.style.left = Math.random() * 80 + '%';
    });

    // Yes button click
    yesBtn.addEventListener('click', () => {
      questionScreen.classList.add('hidden');
      yesMessage.classList.remove('hidden');

      // Confetti
      for (let i = 0; i < 80; i++) {
        const confetti = document.createElement('div');
        confetti.className = 'confetti';
        confetti.style.left = Math.random() * 100 + 'vw';
        confetti.style.background = `hsl(${Math.random() * 360}, 100%, 70%)`;
        document.body.appendChild(confetti);
        setTimeout(() => confetti.remove(), 3000);
      }
    });

    // Floating hearts
    function createHeart() {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = 5 + Math.random() * 5 + 's';
      heart.style.transform = `scale(${0.5 + Math.random() * 0.8})`;
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 10000);
    }

    // Create hearts continuously
    setInterval(createHeart, 500);
  </script>

</body>
</html>
