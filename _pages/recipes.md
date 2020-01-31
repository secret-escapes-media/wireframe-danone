---
layout: standard
id: recipes
title: Recipes
permalink: /recipes/
nav: true
nav-order: 4
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
        {% assign site-recipes = site.html_pages | where: 'layout', 'recipe' | sort: 'nav-order' %}
        {% for item in site-recipes %}
          <div class="col">
            <div class="bg-img bg-img--3-2" style="background-image: url('{{site.img}}/img.jpg')">
              <a class="bg-img__link" href="{{site.baseurl}}{{item.url}}"></a>
              <div class="bg-img__bg-overlay"></div>
            </div>
            <div class="bg--white boxpad--lg">
              <div class="title title--xs"><a href="{{site.baseurl}}{{item.url}}">{{item.title}}</a></div>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore quia ex doloremque dolorum deleniti vel maiores laudantium aliquam, odio quod labore, nostrum nam, explicabo a. Eaque sed neque hic repellendus...</p>
              <div class="space--sm"></div>
              <div class="row row--valign-center">
                <div class="col col--7">
                  <p>{{item.stats}}</p>
                </div>
                <div class="col col--5">
                  <div class="text--right">
                    <a href="{{site.baseurl}}{{item.url}}" class="btn btn--sm btn--outline btn--outline-orange">See Recipe</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        {% endfor %}
      </div>
    </div>
  </div>
</div>