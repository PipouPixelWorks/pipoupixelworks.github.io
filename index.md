---
layout: default
title: Accueil
---

<!-- Section présentation du studio -->
<section class="hero">
  <h1>Pipou Pixel Works</h1>
  <p>Je suis Olivier Jimenez, développeur solo sur mon temps libre, passionné par la création de jeux mobiles originaux.</p>
  <p>Mon objectif : concevoir des expériences rapides, immersives et uniques. Découvrez mes projets ci-dessous !</p>
</section>

<!-- Liste des jeux -->
<section class="games-list">
  {% for game in site.games %}
    <article class="card">
      <img class="card-art" src="{{ game.cover | relative_url }}" alt="{{ game.title }}">
      <div class="card-info">
        <h2>{{ game.title }}</h2>
        {% if game.short_description %}
          <p class="game-short-description">{{ game.short_description }}</p>
        {% else %}
          <p class="game-short-description">{{ game.description }}</p>
        {% endif %}
        <a class="btn" href="{{ game.url | relative_url }}">Voir le jeu</a>
      </div>
    </article>
  {% endfor %}
</section>
