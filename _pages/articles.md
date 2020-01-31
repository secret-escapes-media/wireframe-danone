---
layout: standard
id: articles
title: Articles
permalink: /articles/
nav: true
nav-order: 5
content-page: true
---

<div class="container vpad--xl">
  <div class="width width--lg text--center">
    <p class="text--xxl">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta voluptatibus eius itaque sequi cumque aliquid temporibus a adipisci voluptates atque, eveniet odio rem ullam, iure, qui incidunt! Totam magni adipisci harum quia possimus tenetur temporibus quae? Similique consequuntur ut architecto voluptatibus. Deserunt assumenda eveniet temporibus numquam, voluptatem officiis. Natus, molestiae.</p>
  </div>
</div>

<div class="bg--light">
  <div class="container">
    <div class="vpad--xxl">
      <div class="row row--6-6 row--gutters-lg">
        {% assign site-articles = site.html_pages | where: 'layout', 'article' | sort: 'nav-order' %}
        {% for item in site-articles %}
          <div class="col">
            <div class="bg-img bg-img--4-3" style="background-image: url('{{site.img}}/img.jpg')">
              <a class="bg-img__link" href="{{site.baseurl}}{{item.url}}"></a>
              <div class="bg-img__bg-overlay"></div>
            </div>
            <div class="space--sm"></div>
            <div class="title title--sm"><a href="{{site.baseurl}}{{item.url}}">{{item.title}}</a></div>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore quia ex doloremque dolorum deleniti vel maiores laudantium aliquam, odio quod labore, nostrum nam, explicabo a. Eaque sed neque hic repellendus...</p>
            <div class="space--sm"></div>
            <a href="{{site.baseurl}}{{item.url}}" class="btn btn--sm btn--outline btn--outline-orange">Read More</a>
            <div class="space--sm"></div>
          </div>
        {% endfor %}
      </div>
    </div>
  </div>
</div>