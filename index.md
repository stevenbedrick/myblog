---
layout: page
title: More Organs → More Human
tagline: Stupid stuff I've figured out so you don't have to.
---
{% include JB/setup %}

  {% assign page = site.posts.first %}
<div class="blog-index">  
  <div class="page-header">
    <h1>{{ page.title }}</h1>
	{% if page.tagline %}<small>{{page.tagline}}</small>{% endif %}
  </div>
	
  <div class="row-fluid post-full">
    <div class="span12">
      <div class="date">
        <span>{{ page.date | date_to_long_string }}</span>
      </div>
      <div class="content">
        {{ page.content }}
      </div>

      <hr>
      <div class="pagination">
        <ul>
        {% if page.previous %}
          <li class="prev"><a href="{{ BASE_PATH }}{{ page.previous.url }}" title="{{ page.previous.title }}">&larr; Previous</a></li>
        {% else %}
          <li class="prev disabled"><a>&larr; Previous</a></li>
        {% endif %}
        </ul>
      </div>
      <hr>
    </div>
  </div>
  
	

</div>


