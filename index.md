---
layout: home
title: Home
---

<div id="intro-wrapper" class="l-text">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="images/headshot.png"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Hi, I'm Zhonghao Shi</h1>
			<div id="intro-subtitle">I'm an Incoming Postdoc Fellow at<br>Harvard University</div>
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
	<div id="everything-else" class="l-middle" style="display: grid; grid-template-columns: repeat(2, 1fr); max-width: 24rem; margin-left: auto; margin-right: auto;">
		<a href="{{ site.url }}/cv.pdf"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a>
		<!-- <a href="{{ site.url }}/everything-else"><div><i class="fa fa-list-ul icon icon-right-space"></i>Everything Else</div></a> -->
	</div>
	<div>
		My research focuses on developing <b>personalized, human-centered AI and robots</b>. More specifically, I design and evaluate <b>machine learning models, AI agents, and socially assistive robots</b> that adapt to users’ individual needs to support learning, health, and overall quality of life.
	</div>
	<div style="height: 1rem"></div>
	<div>
		I am fortunate to be joining Prof. <a href="https://ying-xu.com/">Ying Xu</a>'s lab at <a href="https://www.harvard.edu/">Harvard University</a> as an incoming postdoc fellow to work on AI for education. I defended my PhD at the <a href="https://www.usc.edu/">University of Southern California (USC)</a> where I was fortunate to be advised by Prof. <a href="https://maja-mataric.web.app/">Maja Matarić</a>. Previously I worked on trustworthy machine learning at <a href="https://www.jpmorganchase.com/about/technology/research/applied-research">JPMorganChase</a> and studied at <a href="https://www.ucl.ac.uk/">University College London (UCL)</a>.
	</div>
	<div style="height: 1rem"></div>
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title">Featured <a href="{{ site.url }}/projects">Publications</a></h2>

<p class="feature-text">
	My latest research on human-centered AI and machine learning.
</p>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>
