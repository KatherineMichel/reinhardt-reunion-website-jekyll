---
layout: default
title: Blog Posts by Tag
permalink: /tag/
---


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




<body id="top" class="downscroll-enabled home is-singular page page-id-2 page-template page-template-_front page-template-page-template page-template-page-template_front-php">

<div id="page" class="hfeed site">
	<div class="site-inner">

<header id="masthead" class="site-header" role="banner" itemscope itemtype="http://schema.org/WPHeader">

<nav id="site-navigation" class="main-navigation" role="navigation" itemscope itemtype="http://schema.org/SiteNavigationElement"><span class="screen-reader-text">Modern site navigation</span><a class="skip-link screen-reader-text" href="#content">Skip to content</a><div class="main-navigation-inner"><div class="menu"><ul><li id="menu-item-14" class="menu-item menu-item-type-post_type menu-item-object-page current-menu-item page_item page-item-2 current_page_item menu-item-14 active-menu-item"><a href="/reinhardt-reunion-website-jekyll/">Home</a></li>
<li id="menu-item-15" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-15"><a href="/reinhardt-reunion-website-jekyll/gallery/">Gallery</a></li>
<li id="menu-item-15" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-15"><a href="/reinhardt-reunion-website-jekyll/blog/">Blog</span></a></li>
<li id="menu-item-15" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-15"><a href="https://www.facebook.com/groups/1671389859766863" target="_blank">Facebook</span></a></li>
<!--<li id="menu-item-15" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-15"><a href="/admin" target="_blank">Admin</a></li>-->
</ul></div>

<!--<div id="nav-search-form" class="nav-search-form"><a href="#" id="search-toggle" class="search-toggle"><span class="screen-reader-text">Search</span></a>
<form method="get" class="form-search" action="http://themedemos.webmandesign.eu/modern/">
	<label for="search-field" class="screen-reader-text">Search</label>
	<input type="search" value="" placeholder="Search field: type and press enter" name="s" class="search-field" id="search-field" />
</form></div>-->

</div>

<button id="menu-toggle" class="menu-toggle" aria-controls="site-navigation" aria-expanded="false">Menu</button></nav><div class="site-branding"><h1 class="site-title logo type-text"><a href="/reinhardt-reunion-website-jekyll/" title="Modern | WordPress Theme by WebMan"><span class="text-logo">Welcome</span></a></h1><h2 class="site-description"> </h2></div><div class="social-links"><ul id="menu-social-links" class="social-links-items"><li id="menu-item-8" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-8"><a href="https://www.facebook.com/groups/1671389859766863" target="_blank" onclick="_gaq.push(['_trackEvent', 'outbound-widget', 'https://www.facebook.com/groups/1671389859766863', 'WebMan on Facebook']);" ><span class="screen-reader-text">Reinhardt Reunion on Facebook</span></a></li>
</ul></div>


    <div id="site-banner" class="site-banner no-slider">

	<div class="site-banner-inner">
		
<div class="site-banner-content">
	
	<div class="site-banner-media">

		<figure class="site-banner-thumbnail">

			<img src="../images/header.png"" width="1920" height="1080" alt="" />

		</figure>

	</div>
	
</div>
	</div>

</div>

</header>

<div id="content" class="site-content">

	<div id="primary" class="content-area">

		<main id="main" class="site-main clearfix" role="main">

	<section class="archives-listing">

		<header class="page-header">

			<h1 class="page-title">Blog</h1></header>

				<div id="posts" class="posts posts-list clearfix" itemscope itemtype="http://schema.org/ItemList"><ul class="taxonomy-links taxonomy-jetpack-portfolio-type"><li class="link-all">
		
				</ul>


<article id="post-160" class="post-160 jetpack-portfolio type-jetpack-portfolio status-publish format-standard has-post-thumbnail hentry jetpack-portfolio-type-movies jetpack-portfolio-tag-films jetpack-portfolio-tag-movies-2" itemscope itemprop="blogPost" itemtype="http://schema.org/BlogPosting">

		<div class="entry-media">

			<figure class="post-thumbnail" itemprop="image">

				<!--<img src="/reinhardt-reunion-website-jekyll">-->

			</figure>

		</div>
		
		<div class="entry-inner"><header class="entry-header"><h1 class="entry-title" itemprop="name"><a href="/reinhardt-reunion-website-jekyll/post/2016/07/14/welcome-to-reinhardt-reunion-website.html" rel="bookmark">Welcome to Reinhardt Reunion Website!</a></h1></header>
		
		<div class="entry-content" itemprop="description"><p class="post-excerpt"><p>The Reinhardt Reunion website is the companion to the <a href="https://www.facebook.com/groups/1671389859766863" target="_blank">Reinhardt Reunion Facebook group</a>, created for the descendants of...</p>

		<div class="link-more"><a href="/reinhardt-reunion-website-jekyll/post/2016/07/14/welcome-to-reinhardt-reunion-website.html">Continue reading<span class="screen-reader-text"> "Style guide"</span></a>
		</div>
		</div>
	
		<div class="entry-meta"><p>Published: Jul 14, 2016</p> 
		</div>
		</div>

</article>
			


		</main><!-- /#main -->
	</div><!-- /#primary -->
</div><!-- /#content -->

	</div><!-- /.site-inner -->
</div><!-- /#page -->
