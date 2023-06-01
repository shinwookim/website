---
layout: page
---

<img alt="Shinwoo Kim" src="./assets/img/hero-bg.webp" class="figure-img img-fluid rounded" />

##### What's New?
{% for item in site.data.news %}

{% if forloop.index < 4 %}   
<div class="row">
<div class="col-2">
<p markdown="1" class="fw-bolder"> {{item.when}}</p>
</div>
<div class="col-10">
<p markdown="1">{{item.what}}</p>
</div>
</div>

{% elsif forloop.index == 4 %}
<div class="text-center">
<a id="news-btn" data-bs-toggle="collapse" href="#news-content" role="button"
aria-expanded="false" aria-controls="news-content" style="font-size: 0.85rem;"
onclick="document.getElementById('news-btn').style.display = 'none';">More News</a>
</div>
<div class="collapse">
<div class="row">
<div class="col-2">
<p markdown="1" class="fw-bolder"> {{item.when}}</p>
</div>
<div class="col-10">
<p markdown="1">{{item.what}}</p>
</div>
</div>
</div>
<div class="collapse" id="news-content">
{% else %}
<div class="row">
<div class="col-2 " markdown="1">
<p markdown="1" class="fw-bolder"> {{item.when}}</p>
</div>
<div class="col-10">
<p markdown="1">{{item.what}}</p>
</div>
</div>
{% endif %}
{% endfor %}
</div>

<style>
    p{
        font-size: 1rem !important;
    }
</style>
