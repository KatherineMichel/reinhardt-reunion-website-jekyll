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




<div id="content" class="site-content">

	<div id="primary" class="content-area">

		<main id="main" class="site-main clearfix" role="main">

	<section class="archives-listing">

		<header class="page-header">

			<h1 class="page-title">Tags</h1></header>

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




			<section class="blog-posts front-page-section">

				<header class="page-header">

					<h1 class="page-title"><a href="{{ "/blog/" | prepend: site.baseurl }}">Blog</a></h1>

<div class="posts posts-list clearfix" itemscope itemtype="http://schema.org/ItemList"><ul class="taxonomy-links taxonomy-jetpack-portfolio-type">

				</header>

				<div class="posts posts-list clearfix" itemscope itemtype="http://schema.org/ItemList">

{% for post in site.posts %}

<article id="post-160" class="post-160 jetpack-portfolio type-jetpack-portfolio status-publish format-standard has-post-thumbnail hentry jetpack-portfolio-type-movies jetpack-portfolio-tag-films jetpack-portfolio-tag-movies-2" itemscope itemprop="blogPost" itemtype="http://schema.org/BlogPosting">

		<div class="entry-media">

			<figure class="post-thumbnail" itemprop="image">

				<!--<img src="{{ post.image | prepend: site.baseurl  }}">-->

			</figure>

		</div>
		
		<div class="entry-inner"><header class="entry-header"><h1 class="entry-title" itemprop="name"><a href="{{ post.url | prepend: site.baseurl }}" rel="bookmark">{{ post.title }}</a></h1></header>
		
		<div class="entry-content" itemprop="description"><p class="post-excerpt">{{ post.excerpt | truncatewords:20 }}</p>

<div class="tags">
Tags
<!--{% for tag in post.tags %} <div class='tag'><a href='/tag/#{{tag}}'>{{tag}}</a></div> {% endfor %}-->
{% for tag in post.tags %} <div class='tag'><a href="{{ site.baseurl }}/tag/#{{tag}}" }}">{{tag}}</a></div> {% endfor %}
</div></br>

		<div class="link-more"><a href="{{ post.url | prepend: site.baseurl }}">Continue reading<span class="screen-reader-text"> "Style guide"</span></a>
		</div>
		</div>
	
		<div class="entry-meta"><p>Published: {{ post.date | date: "%b %-d, %Y" }}</p> 
		</div>

		</div>

</article>
			
{% endfor %}

 </div>

			</section>





			<section class="blog-posts front-page-section">

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}

				<header class="page-header">

<!--{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}-->

<!--
<h4><a name="{{t | downcase | replace:" ","-" }}"></a><a class="internal" href="{{ site.baseurl }}/tag/#{{t | downcase | replace:" ","-" }}">{{ t | downcase }}</a></h4>-->

					<h1 class="page-title"><a name="{{t | downcase | replace:" ","-" }}"></a><a href="{{ site.baseurl }}/tag/#{{t | downcase | replace:" ","-" }}">{{ t | downcase }}</a></h1>

<!--{% for post in posts %}
  {% if post.tags contains t %}-->

<div class="posts posts-list clearfix" itemscope itemtype="http://schema.org/ItemList"><ul class="taxonomy-links taxonomy-jetpack-portfolio-type">

				</header>

				<div class="posts posts-list clearfix" itemscope itemtype="http://schema.org/ItemList">



<ul>

  <!--<li>
    <a href="{{ site.baseurl }}/{{ post.url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y"  }}</span>
  </li>-->




{% for post in posts %}
  {% if post.tags contains t %}
  
<article id="post-160" class="post-160 jetpack-portfolio type-jetpack-portfolio status-publish format-standard has-post-thumbnail hentry jetpack-portfolio-type-movies jetpack-portfolio-tag-films jetpack-portfolio-tag-movies-2" itemscope itemprop="blogPost" itemtype="http://schema.org/BlogPosting">

		<div class="entry-media">

			<figure class="post-thumbnail" itemprop="image">

				<!--<img src="{{ post.image | prepend: site.baseurl }}">-->

			</figure>

		</div>
		
		<div class="entry-inner"><header class="entry-header"><h1 class="entry-title" itemprop="name"><a href="{{ post.url | prepend: site.baseurl }}" rel="bookmark">{{ post.title }}</a></h1></header>
		
		<div class="entry-content" itemprop="description"><p class="post-excerpt">{{ post.excerpt | truncatewords:20 }}</p>

<div class="tags">
Tags
<!--{% for tag in page.tags %} <div class='tag'><a href='/tag/#{{tag}}'>{{tag}}</a></div> {% endfor %}-->
{% for tag in post.tags %} <div class='tag'><a href="{{ site.baseurl }}/tag/#{{tag}}" }}">{{tag}}</a></div> {% endfor %}
</div></br>

		<div class="link-more"><a href="{{ post.url | prepend: site.baseurl }}">Continue reading<span class="screen-reader-text"> "Style guide"</span></a>
		</div>
		</div>
	
		<div class="entry-meta"><p>Published: {{ post.date | date: "%b %-d, %Y" }}</p> 
		</div>
		</div>


  {% endif %}
{% endfor %}
</ul>


</article>

 </div>

{% endfor %}

			</section>







			<section class="blog-posts front-page-section">

				<header class="page-header">

					<h1 class="page-title"><a href="{{ "/blog/" | prepend: site.baseurl }}">Blog</a></h1>

<div class="posts posts-list clearfix" itemscope itemtype="http://schema.org/ItemList"><ul class="taxonomy-links taxonomy-jetpack-portfolio-type">

				</header>

				<div class="posts posts-list clearfix" itemscope itemtype="http://schema.org/ItemList">

{% for post in site.posts %}

<article id="post-160" class="post-160 jetpack-portfolio type-jetpack-portfolio status-publish format-standard has-post-thumbnail hentry jetpack-portfolio-type-movies jetpack-portfolio-tag-films jetpack-portfolio-tag-movies-2" itemscope itemprop="blogPost" itemtype="http://schema.org/BlogPosting">

		<div class="entry-media">

			<figure class="post-thumbnail" itemprop="image">

				<!--<img src="{{ post.image | prepend: site.baseurl  }}">-->

			</figure>

		</div>
		
		<div class="entry-inner"><header class="entry-header"><h1 class="entry-title" itemprop="name"><a href="{{ post.url | prepend: site.baseurl }}" rel="bookmark">{{ post.title }}</a></h1></header>
		
		<div class="entry-content" itemprop="description"><p class="post-excerpt">{{ post.excerpt | truncatewords:20 }}</p>

<div class="tags">
Tags
<!--{% for tag in post.tags %} <div class='tag'><a href='/tag/#{{tag}}'>{{tag}}</a></div> {% endfor %}-->
{% for tag in post.tags %} <div class='tag'><a href="{{ site.baseurl }}/tag/#{{tag}}" }}">{{tag}}</a></div> {% endfor %}
</div></br>

		<div class="link-more"><a href="{{ post.url | prepend: site.baseurl }}">Continue reading<span class="screen-reader-text"> "Style guide"</span></a>
		</div>
		</div>
	
		<div class="entry-meta"><p>Published: {{ post.date | date: "%b %-d, %Y" }}</p> 
		</div>

		</div>

</article>
			
{% endfor %}

 </div>

			</section>
