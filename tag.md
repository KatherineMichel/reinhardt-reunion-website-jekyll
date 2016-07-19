---
layout: default
title: Blog Posts by Tag
permalink: /tag/

---

<div id="content" class="site-content">

	<div id="primary" class="content-area">
		<main id="main" class="site-main clearfix" role="main">

<article id="post-2" class="post-2 page type-page status-publish hentry" itemscope itemtype="http://schema.org/WebPage">




<ul class="tags">
{% for tag in site.tags %}
  {% assign t = tag | first %}
  <li><a href="{{ site.baseurl }}/tag/#{{t | downcase | replace:" ","-" }}">{{ t | downcase }}</a></li>
{% endfor %}
</ul>

<!--"{{ site.baseurl }}/tag/#{{ tag | first | slugify }}"-->

---

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}

<h4><a name="{{t | downcase | replace:" ","-" }}"></a><a class="internal" href="{{ site.baseurl }}/tag/#{{t | downcase | replace:" ","-" }}">{{ t | downcase }}</a></h4>
<ul>
{% for post in posts %}
  {% if post.tags contains t %}
  <li>
    <a href="{{ site.baseurl }}/{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>

---

{% endfor %}





	<div class="entry-inner"><header class="entry-header"><h1 itemprop="name">Click on a tag to see relevant list of posts.</h1></header><div class="entry-content" itemprop="description"><p>The Reinhardt</p> 
	
	<p><a class="button" title="Portfolio" href="{{ "/gallery/" | prepend: site.baseurl }}">Visit Gallery</a> or <a class="button" title="Blog" href="{{ "/blog/" | prepend: site.baseurl }}">Visit Blog</a></p>
</div></div>
</article>

		</main><!-- /#main -->
	</div><!-- /#primary -->
</div><!-- /#content -->
