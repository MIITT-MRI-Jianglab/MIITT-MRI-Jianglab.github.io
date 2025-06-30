---
title: News & Updates
layout: archive
permalink: /news/
author_profile: false
---

<div class="news-container">
  {% assign sorted_news = site.data.news | sort: 'date' | reverse %}
  {% for item in sorted_news %}
  <div class="news-item">
    <div class="news-image">
      <img src="{{ item.image | relative_url }}" alt="{{ item.title }}">
    </div>
    <div class="news-content">
      <h2 class="news-title">{{ item.title }}</h2>
      <div class="news-meta">
        <span class="news-date">{{ item.date | date: "%B %e, %Y" }}</span>
        {% if item.category %}
        <span class="news-category">{{ item.category }}</span>
        {% endif %}
      </div>
      <div class="news-text">
        {{ item.content | markdownify }}
      
      {% if item.link %}
      <a href="{{ item.link.url }}" class="news-link">{{ item.link.text }}</a>
      {% endif %}
      </div>
    </div>
  </div>
  {% endfor %}
</div>

<style>
  .news-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .news-item {
    display: flex;
    margin-bottom: 50px;
    padding: 25px;
    background: var(--global-bg-color);
    color: var(--global-text-color);
    border-radius: 8px;
    box-shadow: 0 4px 15px var(--global-border-color);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  
  .news-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 20px rgba(0,0,0,0.12);
  }
  
  .news-image {
    flex: 0 0 300px;
    margin-right: 30px;
    overflow: hidden;
    border-radius: 6px;
  }
  
  .news-image img {
    width: 100%;
    height: flex;
    object-fit: cover;
    transition: transform 0.5s ease;
  }
  
  .news-item:hover .news-image img {
    transform: scale(1.05);
  }
  
  .news-content {
    flex: 1;
  }
  
  .news-title {
    margin-top: 0;
    margin-bottom: 10px;
    color: var(--global-text-color);
    font-size: 22px;
  }
  
  .news-meta {
    display: flex;
    align-items: center;
    margin-bottom: 15px;
    font-size: 14px;
    color: #7f8c8d;
  }
  
  .news-date {
    margin-right: 15px;
    padding-right: 15px;
    border-right: 1px solid #e0e0e0;
  }
  
  .news-category {
    background-color: #f1f8ff;
    color: #1e6bb8;
    padding: 3px 8px;
    border-radius: 4px;
    font-weight: 500;
  }
  
  .news-text {
    margin-bottom: 15px;
    line-height: 1.6;
    color: var(--global-text-color);
  }
  
  .news-link {
    display: inline-block;
    color: #2980b9;
    font-weight: 600;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  
  .news-link:hover {
    color: #1a5276;
    text-decoration: underline;
  }
  
  /* Responsive design */
  @media (max-width: 768px) {
    .news-item {
      flex-direction: column;
    }
    
    .news-image {
      flex: none;
      width: 100%;
      margin-right: 0;
      margin-bottom: 20px;
    }
  }
</style>
