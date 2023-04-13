---
layout: default
permalink: /cv/
title: cv
nav: true
nav_order: 4
cv_pdf: cv.pdf
---
Test
<div class="post">
	<header class="post-header">
		<h1 class="post-title">{{ page.title }} {% if page.cv_pdf %}<a href="{{ page.cv_pdf | prepend: 'assets/pdf/' | relative_url}}" target="_blank" rel="noopener noreferrer" class="float-right"><i class="fas fa-file-pdf"></i></a>{% endif %}</h1>
		<p class="post-description">{{ page.description }}</p>
	</header>

	<article>
		<iframe class="cv-display" src="/assets/pdf/cv.pdf" width="100%" height="1000px"></iframe>	
	</article>
</div>
