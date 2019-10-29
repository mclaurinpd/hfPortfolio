---
title: Portfolio
layout: blog
permalink: /portfolio/
description: This is Hannah Fell's portfolio.
author: Hannah Fell
---

<main class="main  container">

  <div class="content">

    <article class="article  article--page  typeset">
      <h2>Clips</h2>
    </article>

    <ul>
      {% for clip in site.clips %}
        <li style="margin-bottom: 20px" class="list  list--posts" margin="0 0 10px 0">
          <article class="article  article--post">
            <h5><a href="{{ clip.url }}">{{ clip.title }}</a></h5>
          </article>
        </li>
        {% endfor %}
    </ul>

   	 <article class="article  article--page  typeset">
    	<h2>Fiction</h2>
   	 </article>

    <ul>
    	{% for story in site.stories %}
    		<li style="margin-bottom: 20px" class="list  list--posts">
    			<article class="article  article--post">
    				<h5><a href="{{ story.url }}">{{ story.title }}</a></h5>
    			</article>
    		</li>
  	  	{% endfor %}
  	</ul>

  </div>

  {% if page.aside == true %}{% include site-aside.html %}{% endif %}

</main>
