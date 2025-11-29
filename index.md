---
layout: default
title: Accueil
---

<section class="hero">
  <h1>Pipou Pixel Works</h1>
  <p>Studio indépendant — jeux mobiles en pixel art.</p>
</section>

<section class="games-list">
  {% for game in site.games %}
    <article class="card">
      <img class="card-art" src="{{ game.cover | relative_url }}" alt="{{ game.title }}">
      <div class="card-info">
        <h2>{{ game.title }}</h2>
        <p>{{ game.description }}</p>
        <a class="btn" href="{{ game.url | relative_url }}">Voir le jeu</a>
      </div>
    </article>
  {% endfor %}
</section>