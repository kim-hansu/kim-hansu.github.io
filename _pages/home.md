---
layout: post
title: "Home"
author: "Hansu Kim"
permalink: /home/
---
   
## Welcome to the CODE Lab!   
   
<div style="display: flex; justify-content: center;">
  <img src="https://github.com/user-attachments/assets/2557bc6f-c0bf-47a5-b683-ac2cf1f2225a" 
       alt="Home" 
       style="max-width: 100%; height: auto; width: auto; max-height: 75vh; object-fit: contain;">
</div>      
   
The **Computational Optimum DEsign (CODE) Lab** is dedicated to research in design optimization, with a particular emphasis on design for additive manufacturing (DfAM), as well as data-driven design, design for mobility components, and optimization algorithms for artificial neural networks. Our research develops analytical and computational methods to solve practical engineering problems in smart factory systems and related applications.   
   
**We are currently seeking highly motivated graduate and undergraduate students to join CODE Lab. If you are interested, feel free to reach out at [hansukim@gachon.ac.kr](mailto:hansukim@gachon.ac.kr)** 😊   
   
<div class="tags">
  <div class="tags-header">
    <h2 class="tags-header-title">{{ page.title }}</h2>
    <div class="tags-header-line"></div>
  </div>
  <div class="tags-clouds">
    {% for tag in site.tags %}
    <a href="#{{ tag[0] }}">{{ tag[0] }}</a>
    {% endfor %}
  </div>
  {% for tag in site.tags %}
  <div class="tags-item" id="{{ tag[0] }}">
    <svg
      class="tags-item-icon"
      xmlns="http://www.w3.org/2000/svg"
      width="20"
      height="20"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
      class="feather feather-tag"
    >
      <path
        d="M20.59 13.41l-7.17 7.17a2 2 0 0 1-2.83 0L2 12V2h10l8.59 8.59a2 2 0 0 1 0 2.82z"
      ></path>
      <line x1="7" y1="7" x2="7.01" y2="7"></line>
    </svg>
    <h2 class="tags-item-label">{{ tag[0] }}</h2>
    {% for post in tag[1] %}
    <a class="tags-post" href="{{ post.url | prepend: site.baseurl }}">
      <div>
        <span class="tags-post-title">{{ post.title }}</span>
        <div class="tags-post-line"></div>
      </div>
      <span class="tags-post-meta">
        <time datetime="{{ post.date }}">
          {{ post.date | date:"%Y-%m-%d" }}
        </time>
      </span>
