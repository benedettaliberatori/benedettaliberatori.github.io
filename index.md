---
layout: home
title: Home
---

<div id="intro-wrapper" class="l-text">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="/images/myportrait.jpg"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Benedetta Liberatori</h1>
			<div id="intro-subtitle">PhD student @ University of Trento</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<!-- <hr class="l-middle home-hr"> -->
	<div id="everything-else" class="l-middle">
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<!--<a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a> -->
		<a href="{{ site.url }}/everything-else"><div><i class="fa fa-list-ul icon icon-right-space"></i>Everything Else</div></a>
	</div>
	<div>
		Hi! I am Benedetta Liberatori. I am a second year PhD student at the <a href="https://mhug.disi.unitn.it/#/">Multimedia Human Understanding Group</a> (<a href="https://www.disi.unitn.it/">University of Trento</a>, Italy), where I am supervised by <a href="https://eliricci.eu/">Prof. Elisa Ricci</a>. 

	</div>
	<div style="height: 1rem"></div>
	<div>
		My research interests focus on vision and language models for video understanding. 
	</div>
	<div style="height: 1rem"></div>
	
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title">Selected <a href="/cv/#publications"> Publications</a></h2>

<p class="feature-text">
</p>

<div class="cover-wrapper cover-wrapper-2-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>



