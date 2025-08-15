---
layout: default
title: Projects
permalink: /projects/
---

<section class="section">
    <div class="container">
        <h1 class="text-center mb-4">My Projects</h1>
        <p class="text-center mb-4">A collection of my creative and technical work</p>
        
        <div class="grid grid-2">
            {% for project in site.projects %}
            <div class="card">
                {% if project.image %}
                <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="card-image">
                {% endif %}
                <div class="card-content">
                    <h3 class="card-title">{{ project.title }}</h3>
                    <p class="card-description">{{ project.excerpt | strip_html | truncate: 150 }}</p>
                    {% if project.technologies %}
                    <div class="tags">
                        {% for tech in project.technologies %}
                        <span class="tag">{{ tech }}</span>
                        {% endfor %}
                    </div>
                    {% endif %}
                    <a href="{{ project.url | relative_url }}" class="btn">View Project</a>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</section>