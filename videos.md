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
          <a href="{{ video.url }}" style="all: unset; cursor: pointer;">
            <div class="video-prev" style="background-image: url({{ video.image }})">
                <div class="video-synopsis">
                    <h1>{{ video.topic | markdownify }}</h1>
                    <p>{{ video.synopsis | markdownify }}</p>
                </div>
            </div>
          </a>
	      {% endfor %}
      </div>
	  
    </div>
  </section>
<!-- End Videos -->
