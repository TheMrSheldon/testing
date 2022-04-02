---
layout: page
title: Videos
---
<!-- Videos -->
  <section class="page-section" id="videos">
    <div class="container">
	
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Lehrvideos</h2>
          {% if site.data.sitetext[site.locale].videos.text %}
		        <h3 class="section-subheading text-muted">{{ site.data.sitetext[site.locale].videos.text }}</h3>
		      {% endif %}
        </div>
      </div>
	  
      <div class="row text-center">
	      {% for video in site.videos %}
          <div class="col-md-4">
            <h4 class="service-heading">{{ video.chapter &ndash; video.topic | markdownify }}</h4>
            {% if video.synopsis %}<div class="text-muted">{{ video.synopsis | markdownify }}</div>{% endif %}
          </div>
	      {% endfor %}
      </div>
	  
    </div>
  </section>
<!-- End Videos -->
