---
layout: default
title: Home
---

<section class="hero">
    <div class="container">
        <h1>Welcome to My Portfolio</h1>
        <p>Showcasing my creative projects, designs, and engineering work</p>
        <a href="/projects/" class="btn">View My Projects</a>
    </div>
</section>

<section class="section">
    <div class="container">
        <h2 class="text-center mb-4">Featured Work</h2>
        
        <div class="grid grid-3">
            {% for project in site.projects limit:3 %}
            <div class="card">
                {% if project.image %}
                <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="card-image">
                {% endif %}
                <div class="card-content">
                    <h3 class="card-title">{{ project.title }}</h3>
                    <p class="card-description">{{ project.excerpt | strip_html | truncate: 100 }}</p>
                    <a href="{{ project.url | relative_url }}" class="btn btn-secondary">Learn More</a>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</section>