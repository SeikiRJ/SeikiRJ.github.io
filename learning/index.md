---
layout: home
title: Learning
description: Learning notes and tutorials collected by SeikiRJ.
---

<div class="index-content learning">
    <div class="section">
        <ul class="artical-cate">
            <li><a href="/"><span>Blog</span></a></li>
            <li class="on" style="text-align:center"><a href="/learning"><span>Learning</span></a></li>
            <li style="text-align:right"><a href="/project"><span>Project</span></a></li>
        </ul>

        <div class="cate-bar"><span id="cateBar"></span></div>

        <ul class="artical-list">
        {% for post in site.categories.learning %}
            <li>
                <h2>
                    <a href="{{ post.url }}">{{ post.title }}</a>
                </h2>
                <div class="title-desc">{{ post.description }}</div>
            </li>
        {% endfor %}
        </ul>

        <div class="tagged-posts">
            <h2>Posts by Tag</h2>
            {% for tag in site.tags %}
                {% assign tag_name = tag[0] | remove: "#" %}
                {% assign tag_posts = tag[1] | where: "category", "learning" %}
                {% if tag_posts.size > 0 %}
                <section id="tag-{{ tag_name | slugify }}" class="tag-group">
                    <h3>#{{ tag_name }}</h3>
                    <ul>
                    {% for post in tag_posts %}
                        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
                    {% endfor %}
                    </ul>
                </section>
                {% endif %}
            {% endfor %}
        </div>
    </div>
    <div class="aside">
        <div class="tag-sidebar">
            <h3>Tags</h3>
            <ul>
            {% for tag in site.tags %}
                {% assign tag_name = tag[0] | remove: "#" %}
                {% assign tag_posts = tag[1] | where: "category", "learning" %}
                {% if tag_posts.size > 0 %}
                <li><a href="#tag-{{ tag_name | slugify }}">#{{ tag_name }} <span>({{ tag_posts.size }})</span></a></li>
                {% endif %}
            {% endfor %}
            </ul>
        </div>
    </div>
</div>
