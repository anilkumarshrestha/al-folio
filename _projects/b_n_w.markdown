---
layout: page
title: Black and White
description: All of my Black and White photos.
img: /assets/img/BW/Eyestocker (8).jpg
importance: 1
category: work
---

<div class="container">


{% for image in site.static_files %}
    {% if image.path contains 'img/BW' %}
        <div class="row p-1">  
            <div class="col-md">
                <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}{{ image.path | relative_url }}" alt="" title="Eyestocker"/>
            </div>
        </div>

    {% endif %}
{% endfor %}

</div>