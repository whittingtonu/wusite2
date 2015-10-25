---
layout: page
permalink: /about/index.html
title: About Whittington U
tags: [Jon Weiler, Whittington U, NRA Whittington Center, Firearm Training, Precision Shooting,]
imagefeature: fourseasons.jpg
chart: true
---
<figure>
  <img src="{{ site.url }}/images/whittingtonu.jpg" alt="Whittington U">
  <figcaption>Whittington U - Training Division of the NRA Whittington Center</figcaption>
</figure>

{% assign total_words = 0 %}
{% assign total_readtime = 0 %}
{% assign featuredcount = 0 %}
{% assign statuscount = 0 %}

{% for post in site.posts %}
    {% assign post_words = post.content | strip_html | number_of_words %}
    {% assign readtime = post_words | append: '.0' | divided_by:200 %}
    {% assign total_words = total_words | plus: post_words %}
    {% assign total_readtime = total_readtime | plus: readtime %}
    {% if post.featured %}
    {% assign featuredcount = featuredcount | plus: 1 %}
    {% endif %}
{% endfor %}


This is the info site for Whittington U, the training division of the NRA Whittington Center.  Located at the foothills of the Sangre de Cristo Mountains in NE New Mexico, the NRA Whittington Center is a 52 square mile world class outdoor facility.  The Whittington U is the instructional division of the NRA Whittington Center that utilizes an educational model in the approach to firearms instruction. Broken down into Academies that are applicable to the firearm or method of instruction, the Whittington U strives to assist all students in building both confidence and a holistic understanding of all the firearm platforms.

Broken down into the Defensive Academy and Precision Academy, Whittington U focuses on the Everday Implementation of the firearm tool into our everyday lives.The Whittington U also focuses on the real world implementation of the firearm platform, regardless if it is a technical, precision long range or defensive oriented curriculum. Each course is designed to educate students in a manner that is both easily understandable and retainable. Our course sizes are such to ensure a good Instructor:Student ratio to assist every individual who attends our courses.

<iframe width="560" height="315" src="https://www.youtube.com/embed/KTlHyVqSIM8" frameborder="0" allowfullscreen></iframe>


This is our information hub about the training points, equipment and readiness thoughts that we see at the Whittington U.  This site currently has {{ site.posts | size }} posts in {{ site.categories | size }} categories which combinedly have {{ total_words }} words, which will take an average reader ({{ site.wpm }} WPM) approximately <span class="time">{{ total_readtime }}</span> minutes to read. {% if featuredcount != 0 %}There are <a href="{{ site.url }}/featured">{{ featuredcount }} featured posts</a>, you should definitely check those out.{% endif %} The most recent post is {% for post in site.posts limit:1 %}{% if post.description %}<a href="{{ site.url }}{{ post.url }}" title="{{ post.description }}">"{{ post.title }}"</a>{% else %}<a href="{{ site.url }}{{ post.url }}" title="{{ post.description }}" title="Read more about {{ post.title }}">"{{ post.title }}"</a>{% endif %}{% endfor %} which was published on {% for post in site.posts limit:1 %}{% assign modifiedtime = post.modified | date: "%Y%m%d" %}{% assign posttime = post.date | date: "%Y%m%d" %}<time datetime="{{ post.date | date_to_xmlschema }}" class="post-time">{{ post.date | date: "%d %b %Y" }}</time>{% if post.modified %}{% if modifiedtime != posttime %} and last modified on <time datetime="{{ post.modified | date: "%Y-%m-%d" }}" itemprop="dateModified">{{ post.modified | date: "%d %b %Y" }}</time>{% endif %}{% endif %}{% endfor %}. The last post was on {{ site.time | date: "%A, %d %b %Y" }} at {{ site.time | date: "%I:%M %p" }} [UTC](http://en.wikipedia.org/wiki/Coordinated_Universal_Time "Temps Universel Coordonné").


<figure>
	<img src="{{ site.url }}/images/about/WUpcitable.jpg" alt="WU Practical Carbine">
	<figcaption>Day 1: Practical Carbine I</figcaption>
</figure>

Whittington U offers some of the best firearm instruction in the world!

<figure class="third">
	<a href="{{ site.url }}/images/about/highangle1.jpg"><img src="{{ site.url }}/images/about/highangle1-1.jpg"></a>
	<a href="{{ site.url }}/images/about/highangle2.jpg"><img src="{{ site.url }}/images/about/highangle1-2.jpg"></a>
	<a href="{{ site.url }}/images/about/highangle3.jpg"><img src="{{ site.url }}/images/about/highangle1-3.jpg"></a>
</figure>
<figure class="half">
	<a href="{{ site.url }}/images/about/highangle1-7.jpg"><img src="{{ site.url }}/images/about/highangle7.jpg"></a>
	<a href="{{ site.url }}/images/about/highangle1-8.jpg"><img src="{{ site.url }}/images/about/highangle8.jpg"></a>
</figure>
<figure class="third">
	<a href="{{ site.url }}/images/about/highangle4.jpg"><img src="{{ site.url }}/images/about/highangle1-4.jpg"></a>
	<a href="{{ site.url }}/images/about/highangle5.jpg"><img src="{{ site.url }}/images/about/highangle1-5.jpg"></a>
	<a href="{{ site.url }}/images/about/highangle6.jpg"><img src="{{ site.url }}/images/about/highangle1-6.jpg"></a>
	<figcaption>Photos from WU Courses</figcaption>
</figure>


<figure>
	<img src="{{ site.url }}/images/about/Defensive-Academy3.jpg" alt="WU Defensive Academy">
	<figcaption>WU Defensive Academy Courses</figcaption>
</figure>

<a href="http://nrawc.goemerchant-stores.com/Defensive-Academy_c_28.html" class="button">Register</a>

**WU Defensive Academy**

The Whittington U Defensive Academy focuses on the real world implementation on the defensive use of the Pistol and Carbine Platforms. The Defensive Academy's goals are to instill a strong fundamental base of interaction with the firearm platform, to help further the knowledge of the responsible gun owner.

<figure class="third">
	<a href="{{ site.url }}/images/about/pp.jpg"><img src="{{ site.url }}/images/about/pp-1.png"></a>
	<a href="{{ site.url }}/images/about/pc.jpg"><img src="{{ site.url }}/images/about/pc-1.jpg"></a>
	<a href="{{ site.url }}/images/about/ps.jpg"><img src="{{ site.url }}/images/about/ps-1.jpg"></a>
</figure>

The Defensive Academy offers a progressive course lineup that begins with the Fundamentals of Defensive Marksmanship and leads up to a series of Masters Courses that will be the conditioning response for the respective platforms. Training is key to success in every endeavor and the Whittington U Defensive Academy give students the opportunity to test themselves, both mentally and physically in a controlled environment. 

<figure>
	<img src="{{ site.url }}/images/about/Precision-Academy3.jpg" alt="WU Precision Academy">
	<figcaption>Click above for info on the WU Precision Academy</figcaption>
</figure>

**WU Precision Academy**

The Whittington U Precision Academy offers courses specifically oriented towards 1000 Yard and Extreme Long Range Engagements, allowing for all centerfire cartridges and rifle platforms to be used. The School of 1000 Yards focuses on the caliber/cartridges and rifle platforms that are designed for engagements between 100 – 1200 yards, with the School of Extreme Long Range emphasizing the cartridge/calibers that are designed for 2000 yard and beyond engagements.

The Whittington U Precision Academy courses take place in the beautiful NRA Whittington Center's Backcountry Training Area that is equipped with a Known Distance, High Angle and Unknown Distance Range to maximize each course to its fullest potential.

<figure class="third">
	<a href="{{ site.url }}/images/about/1000.jpg"><img src="{{ site.url }}/images/about/1000-1.jpg"></a>
	<a href="{{ site.url }}/images/about/elr.jpg"><img src="{{ site.url }}/images/about/elr-1.jpg"></a>
</figure>

Both the School of 1000 Yards and School of ELR offer various Masters Courses that are designed to challenge each graduate by putting them in an environment that forces them to employ the skills taught in previous courses. Our Precision Academy Masters Courses are extremely progressive and the Level I-III Courses are a requirement to participate.


