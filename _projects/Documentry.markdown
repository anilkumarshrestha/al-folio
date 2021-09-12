---
layout: page
title: Documentry
description: All of my Documentry photos.
img: /assets/img/Documentry/Buddha/Eyestocker (1).jpg
importance: 1
category: work
---

<div class="container">


{% for image in site.static_files %}
    {% if image.path contains 'img/Documentry/Buddha/' %}
        <div class="row p-1">  
            <div class="col-md">
                <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}{{ image.path | relative_url }}" alt="" title="Eyestocker"/>
            </div>
        </div>

    {% endif %}
{% endfor %}
<div class="caption">
    Buddha
</div>


{% for image in site.static_files %}
    {% if image.path contains 'img/Documentry/Story/' %}
        <div class="row p-2">
            <div class="col-sm mt-3 mt-md-0">
                <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}{{ image.path | relative_url }}" alt="" title="Eyestocker"/>
            </div>
        </div>
    {% endif %}
{% endfor %}
<div class="caption">
    Story
</div>

</div>