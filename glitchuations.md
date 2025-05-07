---
layout: default
title: Glitchuations
permalink: /glitchuations/
---
<!-- Inline CSS for glitch effect (just on this page) -->
<style>
    <!-- Background glitch effect. -->
body {
  background: #0d0d0d;
  color: white;
  overflow-x: hidden;
  animation: bgFlicker 8s infinite linear;
  background-image: repeating-linear-gradient(
    0deg,
    rgba(0, 255, 255, 0.03),
    rgba(0, 255, 255, 0.03) 1px,
    transparent 1px,
    transparent 2px
  );
}

@keyframes bgFlicker {
  0%, 100% {
    filter: hue-rotate(0deg) brightness(1);
  }
  25% {
    filter: hue-rotate(20deg) brightness(1.1);
  }
  50% {
    filter: hue-rotate(-20deg) brightness(0.9);
  }
  75% {
    filter: hue-rotate(10deg) brightness(1.05);
  }
}

.glitch {
  font-family: monospace;
  position: relative;
  display: inline-block;
  color: white;
  font-size: 48px;
}

.glitch::before,
.glitch::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  overflow: hidden;
}

.glitch::before {
  left: 1px;
  text-shadow: -1px 0 lime;
  animation: glitch 2s infinite linear alternate-reverse;
}

.glitch::after {
  left: -1px;
  text-shadow: -1px 0 cyan;
  animation: glitch 2.5s infinite linear alternate-reverse;
}

@keyframes glitch {
  0% {
    clip: rect(0, 9999px, 0, 0);
  }
  10% {
    clip: rect(0, 9999px, 20px, 0);
  }
  20% {
    clip: rect(0, 9999px, 5px, 0);
  }
  30% {
    clip: rect(0, 9999px, 10px, 0);
  }
  100% {
    clip: rect(0, 9999px, 0, 0);
  }
}

<!-- Heading glitch effect-->
.glitch {
  font-family: monospace;
  position: relative;
  display: inline-block;
  color: white;
  font-size: 48px;
}
.glitch::before,
.glitch::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  overflow: hidden;
}
.glitch::before {
  left: 1px;
  text-shadow: -1px 0 lime;
  animation: glitch 2s infinite linear alternate-reverse;
}
.glitch::after {
  left: -1px;
  text-shadow: -1px 0 cyan;
  animation: glitch 2.5s infinite linear alternate-reverse;
}
@keyframes glitch {
  0% {
    clip: rect(0, 9999px, 0, 0);
  }
  10% {
    clip: rect(0, 9999px, 20px, 0);
  }
  20% {
    clip: rect(0, 9999px, 5px, 0);
  }
  30% {
    clip: rect(0, 9999px, 10px, 0);
  }
  100% {
    clip: rect(0, 9999px, 0, 0);
  }
}
</style>

# <span class="glitch" data-text="Glitchuations">Glitchuations</span>


Welcome to the Glitch Tower. Every step forward is a risk — do you dare?

<button onclick="moveFloor()">Try Moving to the Next Floor</button>
<p id="result"></p>

<script>
function moveFloor() {
  const chance = Math.random();
  if (chance > 0.6) {
    document.getElementById("result").innerText = "✨ You move up a floor!";
  } else {
    document.getElementById("result").innerText = "💥 Glitch! You’re stuck.";
  }
}
</script>

# My Project

<!-- This section is for the introduction, which is still being written. -->
This is a project started in Mr.Norris C++ class. Look forward to the completed version...

## Glitchuations Game

<!-- The next section will explain the gameplay mechanics. -->
Glitchuations: A Choose-Your-Own Adventure Game
Step into a mysterious glitch tower where every floor is a new challenge! In Glitchuations, you must navigate through an ever-changing digital environment filled with unexpected glitches and mind-bending decisions.

Game Mechanics
Choose Your Path: At each floor, you’re faced with a mathmatical equation. Where you go detemines what kind of questions you'll find  — so choose wisely!

Glitchy Obstacles: As you attempt to climb the tower, you'll encounter random glitches that may halt your progress, sending you back to previous floors.

Random Chance: Even when you make the right choices, the tower isn’t always predictable. Sometimes, it’s all about luck! The chances of moving to the next floor are determined randomly.

Endless Replayability: With every playthrough offering new answers and paths, Glitchuations invites you to test your decision-making skills and see how far you can ascend the glitch tower.

Can you beat the tower and escape the endless cycle of glitches? Start your journey now and see if you have what it takes to reach the top!
