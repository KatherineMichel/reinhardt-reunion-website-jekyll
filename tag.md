---
layout: default
title: Blog Posts by Tag
permalink: /tag/

---

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





<div id="content" class="site-content">


	<div id="primary" class="content-area">
		<main id="main" class="site-main clearfix" role="main">


<article id="post-21" class="post-21 page type-page status-publish hentry" itemscope itemtype="http://schema.org/WebPage">

	<div class="entry-inner"><header class="entry-header"><h1 class="entry-title" itemprop="name">Contact</h1></header><div class="entry-content" itemprop="description"><p class="uppercase">Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna aliquam erat volutpat.</p>
<p>Ut wisi enim ad minim veniam, quis nostrud exerci tation ullamcorper suscipit lobortis nisl ut aliquip ex ea commodo consequat. Eodem modo typi, qui nunc nobis videntur parum clari, fiant sollemnes in futurum.</p>
<div id='contact-form-21'>
<form action='http://themedemos.webmandesign.eu/modern/contact/#contact-form-21' method='post' class='contact-form commentsblock'>

<div>
		<label for='g21-name' class='grunion-field-label name'>Name<span>(required)</span></label>
		<input type='text' name='g21-name' id='g21-name' value='' class='name'  required aria-required='true'/>
	</div>

<div>
		<label for='g21-email' class='grunion-field-label email'>Email<span>(required)</span></label>
		<input type='email' name='g21-email' id='g21-email' value='' class='email'  required aria-required='true'/>
	</div>

<div>
		<label for='g21-website' class='grunion-field-label url'>Website</label>
		<input type='text' name='g21-website' id='g21-website' value='' class='url'  />
	</div>



</div>
	</div>

	

		</main><!-- /#main -->
	</div><!-- /#primary -->
</div><!-- /#content -->
