---
layout: default
title: Blog Posts by Tag
permalink: /tag/

---

<div id="content" class="site-content">


	<div id="primary" class="content-area">
		<main id="main" class="site-main clearfix" role="main">


<article id="post-21" class="post-21 page type-page status-publish hentry" itemscope itemtype="http://schema.org/WebPage">


Click on a tag to see relevant list of posts.

<ul class="tags">
{% for tag in site.tags %}
  {% assign t = tag | first %}
  <li><a href="/tag/#{{t | downcase | replace:" ","-" }}">{{ t | downcase }}</a></li>
{% endfor %}
</ul>

<!--"{{ site.baseurl }}/tag/#{{ tag | first | slugify }}"-->

---

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}

<h4><a name="{{t | downcase | replace:" ","-" }}"></a><a class="internal" href="/tag/#{{t | downcase | replace:" ","-" }}">{{ t | downcase }}</a></h4>
<ul>
{% for post in posts %}
  {% if post.tags contains t %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>

---

{% endfor %}


		</main><!-- /#main -->
	</div><!-- /#primary -->
</div><!-- /#content -->
