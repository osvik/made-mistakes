---
layout: archive
title: "Mastering Paper by FiftyThree"
excerpt: "Tutorials and techniques to help learn Paper."
modified: 2014-12-08T12:25:40-05:00
image: 
  feature: mastering-paper-feature.jpg
  thumb: paper-by-fiftythree-icon175x175.png
---

In the spirit of openness I've decided to compile everything I've learned using [*Paper by FiftyThree*](http://www.fiftythree.com), into a series of tutorials and guides titled --- Mastering Paper.
{:.shorten}

<nav class="toc toc-left">
  <ul>
    <li><h6>Getting Started with Paper</h6></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2013-07-31-introduction-tool-guide %}">Introduction and Tool Guide</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2014-07-03-moving-the-loupe %}">Moving the Zoom Loupe</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2014-02-09-basics %}">Drawing and Painting Basics</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2014-10-25-erasing %}">Erasing and Correcting Mistakes</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2013-11-08-moleskine-book %}">Printing a Moleskine Book</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2014-11-25-mix %}">Mastering Mix</a></li>
    <li><h6>Step by Step Paper Tutorials</h6></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2013-08-31-drawing-trees %}">How to Draw Trees and Grass</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2013-09-05-drawing-clouds %}">How to Draw Skies and Clouds</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2013-09-29-drawing-water %}">How to Draw Water and Waves</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2013-11-25-drawing-textures %}">How to Draw Textures</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2014-04-21-drawing-faces %}">How to Draw Skin and Faces</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2013-05-10-drawing-hair %}">How to Draw Hair</a></li>
    <li><h6>Advanced Paper Techniques</h6></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2014-07-06-grid-method %}">The Grid Method</a></li>
    <li><a href="{{ site.url }}{% post_url /mastering-paper/2014-01-13-contour-drawing %}">Contour Line Drawing</a></li>
  </ul>
</nav><!-- /.toc-left -->

<div class="tiles tiles-right">
{% for post in site.categories.mastering-paper %}
  <article class="tile" itemscope itemtype="http://schema.org/Article">
    <a href="{{ post.url }}" title="{{ post.title }}" class="post-teaser">
      <img src="{{ site.url }}/images/preload-400.png" data-original="/images/{% if post.image.teaser %}{{ post.image.teaser }}{% else %}{{ site.teaser }}{% endif %}" class="load" alt="teaser" itemprop="image">
      <noscript><img src="/images/{% if post.image.teaser %}{{ post.image.teaser }}{% else %}{{ site.teaser }}{% endif %}" alt="teaser" itemprop="image"></noscript>
    </a>
    <h2 class="post-title" itemprop="name"><a href="{{ post.url }}">{{ post.title | remove: 'Mastering Paper by FiftyThree: ' | remove: 'Mastering Paper by 53: ' | remove: ' with Paper by 53' }}</a></h2>
    {% if post.date %}<p class="entry-date date published"><time datetime="{{ post.date | date: "%Y-%m-%d" }}" itemprop="datePublished">{{ post.date | date: "%B %d, %Y" }}</time></p>{% endif %}
    <p class="post-excerpt" itemprop="description">{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </article><!-- /.tile -->
{% endfor %}
</div><!-- /.tiles-right -->