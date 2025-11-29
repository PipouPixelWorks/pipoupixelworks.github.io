---
layout: default
title: Neon Rush
description: Shooter vertical en pixel art, rapide et nerveux.
platforms:
- Android
status: En développement
cover: /assets/img/neonrush_logo.png
privacy_policy: /privacy/neon-rush-privacy.html
---


<div class="game-page">
<img src="{{ page.cover }}" alt="{{ page.title }}" class="game-page-logo">
<div class="game-page-info">
<h2>{{ page.title }}</h2>
<p>{{ page.description }}</p>
<p><strong>Plateformes :</strong> {{ page.platforms | join: ", " }}</p>
<p><strong>Statut :</strong> {{ page.status }}</p>
<p class="privacy-link">🔒 <a href="{{ page.privacy_policy }}">Privacy Policy</a></p>
</div>
</div>
