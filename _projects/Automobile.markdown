---
layout: page
title: Automobile
description: All of my automobile photos.
img: /assets/img/2.jpg 
importance: 1
category: work
---

<div class="container">

<div class="row p-2">
{% for image in site.static_files %}
    {% if image.path contains 'img/Automobile/CBR/' %}
            <div class="col-md mt-3 mt-md-0">
                <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}{{ image.path | relative_url }}" alt="" title="Eyestocker"/>
            </div>
    {% endif %}
{% endfor %}
</div>

<div class="caption">
    CBR
</div>

{% for image in site.static_files %}
    {% if image.path contains 'img/Automobile/KTM/' %}
        <div class="row p-1">  
            <div class="col-md">
                <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}{{ image.path | relative_url }}" alt="" title="Eyestocker"/>
            </div>
        </div>

    {% endif %}
{% endfor %}
<div class="caption">
    KTM
</div>


{% for image in site.static_files %}
    {% if image.path contains 'img/Automobile/Royal Enfield/' %}
        <div class="row p-2">
            <div class="col-sm mt-3 mt-md-0">
                <img class="img-fluid rounded z-depth-1" src="{{ site.baseurl }}{{ image.path | relative_url }}" alt="" title="Eyestocker"/>
            </div>
        </div>
    {% endif %}
{% endfor %}
<div class="caption">
    Royal Enfield
</div>

</div>