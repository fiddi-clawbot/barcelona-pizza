---
layout: default
---

<div class="hero">
    <h1>Barcelona's Finest Pizza</h1>
    <p>Discover trending and award-winning pizzerias reshaping Barcelona's food scene. From traditional Neapolitan to innovative modern styles.</p>
    <a href="/barcelona-pizza/pizzerias.html" class="btn" style="margin-top: var(--space-lg); display: inline-block;">View All Pizzerias</a>
</div>

<div class="grid">
    {% for pizzeria in site.pizzerias %}
    <a href="{{ pizzeria.url }}" style="text-decoration: none; color: inherit;">
        <div class="card">
            {% if pizzeria.image %}
            <div class="card-image">
                <img src="{{ pizzeria.image }}" alt="{{ pizzeria.name }}">
            </div>
            {% endif %}
            
            <div class="card-body">
                <h3 class="card-title">{{ pizzeria.name }}</h3>
                
                <div class="card-meta">
                    <span>📍 {{ pizzeria.neighborhood }}</span>
                    {% if pizzeria.award %}<span>🏆 {{ pizzeria.award }}</span>{% endif %}
                </div>
                
                {% if pizzeria.teaser %}
                <p class="card-description">{{ pizzeria.teaser }}</p>
                {% endif %}
            </div>
            
            <div class="card-footer">
                <span class="cta">Read More →</span>
            </div>
        </div>
    </a>
    {% endfor %}
</div>

{{ content }}
