# specialsomeone_D.PRIMrose
Happy birthday, love!
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Birthday Surprise</title>
<style>
  body {
    background-color: #1E90FF; /* blue bg */
    font-family: 'Comic Sans MS', cursive, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    margin: 0;
    overflow: hidden;
    flex-direction: column;
  }

  h1 {
    color: #ff0066;
    font-size: 3em;
    opacity: 0;
    transform: scale(0.5);
    animation: popText 1s forwards;
  }

  @keyframes popText {
    to {
      opacity: 1;
      transform: scale(1);
    }
  }

  /* Cake */
  .cake {
    width: 120px;
    height: 80px;
    background: #FF9999;
    border-radius: 10px;
    margin-top: 20px;
    position: relative;
    opacity: 0;
    transform: scale(0);
    animation: showCake 1s forwards;
    animation-delay: 1s;
  }

  .cake::before {
    content: '';
    position: absolute;
    top: -20px;
    left: 50%;
    transform: translateX(-50%);
    width: 10px;
    height: 20px;
    background: #FFD700;
    border-radius: 2px;
  }

  @keyframes showCake {
    to {
      opacity: 1;
      transform: scale(1);
    }
  }

  /* Envelope */
  .envelope {
    width: 120px;
    height: 80px;
    background: #fff;
    border: 2px solid #000;
    margin-top: 20px;
    position: relative;
    opacity: 0;
    transform: translateY(100px);
    animation: slideEnvelope 1s forwards;
    animation-delay: 2s;
    border-radius: 5px;
  }

  .envelope::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 120px;
    height: 40px;
    background: #fff;
    border-bottom: 2px solid #000;
    clip-path: polygon(0% 0%, 50% 100%, 100% 0%);
    transform-origin: top center;
    transform: rotateX(0deg);
    transition: transform 0.6s ease;
  }

  /* Paper inside envelope */
  .paper {
    width: 110px;
    height: 150px;
    background: #FFFF66;
    position: absolute;
    top: 80px;
    left: 5px;
    border-radius: 5px;
    opacity: 0;
    padding: 10px;
    overflow-y: auto;
  }

  p {
    white-space: pre-wrap;
    font-size: 12px;
    line-height: 1.4em;
    margin: 0;
    color: #000;
  }
</style>
</head>
<body>

<h1>Happy Birthday!</h1>
<div class="cake"></div>
<div class="envelope">
  <div class="paper" id="paper">
    <p id="message"></p>
  </div>
</div>

<script>
const envelope = document.querySelector('.envelope');
const flap = envelope.querySelector('::before'); // we’ll animate manually with JS
const paper = document.getElementById('paper');
const messageEl = document.getElementById('message');

const message = `Happy birthday, baby.

If you’re wondering why I’m awake at this ungodly hour, it’s because my brain refuses to sleep without making sure I tell you how much I love you first. You’re probably already dreaming peacefully, and honestly, I’m a little upset because you forgot to say good night 😭 but it’s okay, baby, I understand. I know you’re tired, and I know I was being extra earlier. I’m sorry for nagging and for being clingy—it’s just my way of showing how much I care about you, even if it’s chaotic and a little annoying.

I love you, baby. Like, scientifically speaking, my limbic system lights up every time I think about you. My neurons literally fire dopamine and oxytocin whenever your name pops into my brain, and it’s not even fair because you weren’t made to be this good at making me feel every emotion at once. You’re the reason my heart—yeah, that literal muscle that pumps blood—is racing right now. And speaking of the heart, remember that argument we had? When I told you it’s “just a muscle, it literally pumps blood” and you were trying to explain it differently? Baby, I was so extra, but also, secretly, that was the moment I thought, wow… okay, I might be a little obsessed with you because you’re actually so smart and patient while I’m over here being ridiculous. That’s the thing with you—you’re amazing, and it’s not even a surprise anymore because you are always amazing.

Baby, I worry about you constantly. I worry if you’ve eaten, if you’re hydrated, if you’re sleeping enough, if you’re overworking yourself. I know you’re grown and capable, and I shouldn’t worry so much, but still, love me, I can’t help it. My love is basically like my own little research project on how much someone can care about another human being, and the data is conclusive: I care about you more than I should, and yes, it’s perfectly irrational but I’m embracing it fully.

I hope today is magical for you. I hope the universe conspires to give you peace, freedom, happiness, and all the good things you deserve. I hope the air you breathe feels lighter, the sun feels warmer, and every little thing reminds you that you are loved, baby. You deserve every joy, every success, every hug from your family, every silly moment, and every late-night talk or late-night movie watch we get to share, even if it’s just through a screen. Those moments, baby, are everything to me. They make me feel close to you, even across all the distance.

I want to say I love you a thousand times, baby, and it still wouldn’t be enough. I love you in every thought, every neuron, every heartbeat, every sigh, every giggle. I love you when I’m being clingy, when I’m being silly, when I’m overthinking, when I’m stubborn, when I’m quiet, when I’m loud. I love you in every possible way that a human brain and heart can process love. My existence right now basically revolves around loving you, and I wouldn’t have it any other way.

I pray for you, baby. I pray that God guides you, protects you, and keeps you safe. I pray that He blesses you with health, happiness, peace, and clarity in everything you do. I pray that He surrounds you with people who love you as much as I do, and that He continues to bless your family with love, safety, and joy. I pray that every path you choose is full of success, and that your dreams become reality. I pray that life treats you kindly, even when it’s hard, and that you always feel supported, loved, and celebrated.

You’re my person, baby. You’re the one I want to laugh with, cry with, debate with, and share every little detail of my life with. You make every ordinary moment extraordinary. You make my heart—yes, that muscle again—feel like it’s performing some high-level, super-efficient love-pumping function just for you. Every late-night talk, every late-night movie watch, every moment we share through texts and calls makes me feel closer to you, even though we’re far apart. Those moments are my favorite memories, and I look forward to making millions more with you, baby.

I’m rambling, I know, but that’s kind of the point. I want this message to feel like me being completely me, baby—all thoughts, all emotions, all love, all obsession, all science, all heart. I want you to read this and feel everything I feel when I think of you, when I miss you, when I worry about you, when I laugh at you being cute, when I just… love you endlessly.

So, happy birthday, baby. Thank you for being the one who makes my dopamine levels go wild, who makes me smile at my phone like a fool, who makes me think that love can be this scientific and this emotional at the same time. I love you more than all the words in the English language, more than all the science I can study, more than my brain can quantify, more than my heart can pump. Love me, baby, and let me keep loving you forever, okay?

Happy birthday again, baby. You are amazing. You are loved. You are my favorite human, my heart, my chaos, my calm, my baby. I love you, love mewhwhhehe.`;

function typeWriter(index = 0) {
  if(index < message.length) {
    messageEl.innerHTML += message.charAt(index);
    setTimeout(() => typeWriter(index+1), 25);
  }
}

// sequence: envelope flap open then show paper then type
setTimeout(() => {
  // show paper
  paper.style.opacity = '1';
  typeWriter();
}, 4000); // 4s after envelope slides in
</script>

</body>
</html>
