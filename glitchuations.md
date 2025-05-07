---
layout: default
title: Glitchuations
permalink: /glitchuations/
---

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
