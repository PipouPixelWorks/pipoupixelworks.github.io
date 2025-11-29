---
layout: default
title: "Jeux"
---

# Nos jeux

<div class="game-grid">
{% for game in site.games %}
  <div class="game-card">
    {% if game.cover %}
      <img src="{{ game.cover }}" alt="Cover {{ game.title }}">
    {% endif %}
    <h3>{{ game.title }}</h3>
    <p>{{ game.description }}</p>
    <a href="{{ game.url }}">Voir le jeu</a>
  </div>
{% endfor %}
</div>

