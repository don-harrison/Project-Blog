---
layout: default
title: Home
---

# Welcome to My Blog

<div class="container mt-4">
    <div class="row">
        {% for post in site.posts %}
        <div class="col-md-6 mb-4">
            <div class="card shadow-sm">
                <div class="card-body">
                    <p class="text-muted text-end">{{ post.date | date: "%B %d, %Y" }}</p>
                    <h5 class="card-title">
                        <a href="{{ post.url }}" class="text-decoration-none">{{ post.title }}</a>
                    </h5>
                    <p class="card-text">{{ post.excerpt }}</p>
                    <a href="{{ post.url }}" class="btn btn-primary">Read More</a>
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
</div>
