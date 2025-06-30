---
title: Photos
layout: archive
permalink: /photos/
author_profile: false
---

<div class="gallery-intro">
  <p>Explore our lab's journey through these memorable moments from conferences, group activities, and research collaborations.</p>
</div>

<div class="gallery-container">
  {% assign sorted_photos = site.data.photos | sort: 'year' | reverse %}
  {% for photo in sorted_photos %}
  <div class="gallery-item">
    <img src="{{ photo.image | relative_url }}" alt="{{ photo.description }}">
    <div class="caption">
      <h3>{{ photo.title }}</h3>
      <p>{{ photo.description }} ({{ photo.year }})</p>
      {% if photo.location %}
        <p class="location">📍 {{ photo.location }}</p>
      {% endif %}
    </div>
  </div>
  {% endfor %}
</div>

<style>
  .gallery-intro {
    text-align: center;
    margin-bottom: 30px;
    font-size: 18px;
    color: #555;
  }
  
  .gallery-container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 25px;
    margin-top: 20px;
  }
  
  .gallery-item {
    background: white;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
  }
  
  .gallery-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0,0,0,0.15);
  }
  
  .gallery-item img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    border-bottom: 1px solid #eee;
  }
  
  .caption {
    padding: 15px;
  }
  
  .caption h3 {
    margin-top: 0;
    margin-bottom: 8px;
    font-size: 18px;
  }
  
  .caption p {
    margin: 5px 0;
    font-size: 14px;
    color: #555;
  }
  
  .location {
    display: flex;
    align-items: center;
    font-size: 13px;
    color: #777;
    margin-top: 8px;
  }
</style>
