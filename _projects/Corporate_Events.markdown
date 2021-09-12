---
layout: page
title: Corporate Events
description: Corporate Events photos
img: /assets/img/Corporate Event/Eyestocker (13).jpg
importance: 1
category: work
---
<div class="container">


{% for image in site.static_files %}
    {% if image.path contains 'img/Corporate Event/' %}
        <div class="row p-1">  
            <div class="col-md">
                <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}{{ image.path | relative_url }}" alt="" title="Eyestocker"/>
            </div>
        </div>

    {% endif %}
{% endfor %}

</div>