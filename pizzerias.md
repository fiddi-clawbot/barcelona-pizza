---
layout: default
title: All Pizzerias
---

<h1>All Pizzerias</h1>

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
                <span class="cta">Details →</span>
            </div>
        </div>
    </a>
    {% endfor %}
</div>
