---
layout: page
title: Blog
permalink: blog/
order: 3
---


This blog will cover a variety of topics that come to mind, including tech, transportation, cities, government, design, geography, and education.

<br>

## All posts

<ul class="post-list">
{% for post in site.posts %}
    <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h2>
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
    </li>
{% endfor %}
</ul>

<p class="rss-subscribe">Subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a>
</p>

<br>

## Post queue

This is a list of posts I'm planning to write. It was inspired by the [post queue](https://pedestrianobservations.wordpress.com/post-queue/) on Alon Levy's blog, Pedestrian Observations.

Transportation, cities, and regions:

* A follow-up to [my post](/2015/08/18/problem-gtfs-modes/) about the limitations of GTFS transit mode classifications. Specifically, this post will propose a new way of describing transit services that focuses on service instead of technology.
* Why I think the key to the future of national rail service in the United States is medium-speed unreserved trains, in contrast to high-speed rail, which is what most discussions center on.
* A potential vision for rail service on the Northeast Corridor, integrating everything from high-speed and long-distance rail to short-distance commuter services.
* Why the "last mile" problem in urban transit isn't nearly as much of a problem as people think, and can actually be a good thing. (Basically, elaborating on [this post](http://urbankchoze.blogspot.com/2014/11/how-i-learned-to-stop-worrying-and-love.html).)
* My categorization of the three primary non-industrial land uses, and how their spatial distribution can best be matched to transit service. (An elaboration on both [this post](http://urbankchoze.blogspot.com/2015/06/in-defense-of-use-separation.html) and [this one](https://pedestrianobservations.wordpress.com/2012/05/24/destination-centralization/).)

Education and math:

* My observations about math education and number sense, after having been a math tutor for 10 months.
* Some of the techniques I show my students about doing arithmetic in ways that rely on dealing with the actual quantities, especially ones that are helpful for doing mental math, in contrast to some traditional pencil-and-paper methods like long division. 
* How I came to love 0-indexing of numbering, and why I think being concious of the usage of 0-indexing vs. 1-indexing in everyday life (and incorporating more 0-indexing) can be very helpful. Also included in this discussion are closed, half-closed, and open intervals, and discrete vs. continuous data.
* Philosophy of science, and how I see the different fields of science relating to each other in different ways. (A modified version of [this diagram](https://commons.wikimedia.org/wiki/File:Partial_ordering_of_the_sciences_Balaban_Klein_Scientometrics2006_615-637.svg).)
* What topics I think are over- and under-emphasized in high school curricula.
* How different academic disciplines (particularly in universities) have much more in common than people realize.

Other:

* Equal representation in legislative bodies based on population makes a lot of sense. But, it does have a major challenge that is rarely discussed, and this post will explain what it is.
* Examples from my life (and my observations) of how more choice can be a bad thing, inspired by [this book](https://en.wikipedia.org/wiki/The_Paradox_of_Choice).

<br>

## Links

Some blogs I follow:

* [Human Transit](http://www.humantransit.org/) (Jarrett Walker)
* [Pedestrian Observations](http://pedestrianobservations.wordpress.com/) (Alon Levy)
* [Urban Kchoze](http://urbankchoze.blogspot.com/)
* [Streetsblog](http://www.streetsblog.org/)