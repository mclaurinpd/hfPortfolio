---
title: Portfolio
layout: blog
permalink: /portfolio/
---

<main class="main  container">

  <div class="content">

   	 <article class="article  article--page  typeset">
    	<h2>Stories</h2>
   	 </article>

    <ul>
    	{% for story in site.stories %}
    		<li class="list  list--posts">
    			<article class="article  article--post">
    				<h4><a href="{{ story.url }}">{{ story.title }}</a></h4>
    			</article>
    		</li>
  	  	{% endfor %}
  	</ul>

  	<article class="article  article--page  typeset">
    	<h2>Clips</h2>
   	 </article>

    <ul>
    	{% for clip in site.clips %}
    		<li class="list  list--posts">
    			<article class="article  article--post">
    				<h4><a href="{{ clip.url }}">{{ clip.title }}</a></h4>
    			</article>
    		</li>
  	  	{% endfor %}
  	</ul>

  </div>

  {% if page.aside == true %}{% include site-aside.html %}{% endif %}

</main>
