---
layout: default
title: Accueil
---


<h1>🎮 Nos jeux</h1>
<div class="games-list">
{% for game in site.games %}
<div class="game-card">
<img src="{{ game.cover }}" alt="{{ game.title }}" class="game-logo">
<div class="game-info">
<h2>{{ game.title }}</h2>
<p>{{ game.description }}</p>
<a class="btn" href="{{ game.url }}">Voir le jeu</a>
</div>
</div>
{% endfor %}
</div>
