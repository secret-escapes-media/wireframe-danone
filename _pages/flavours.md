---
layout: standard
id: flavours
title: Flavours
permalink: /flavours/
nav: true
nav-order: 3
content-page: true

flavours:

  - title: Blueberry
    description: Play to win hearts with this mouth watering taste sensation. Enjoy the fab fruity zing of Light & Free Blueberry!
    link: http://www.lightandfree.com/product/four-pack-blueberry

  - title: Vanilla
    description: Smooth as silk, a timeless classic! Enjoy the laid-back taste of Light & Free Vanilla!
    link: http://www.lightandfree.com/product/four-pack-vanilla

  - title: Peach Passion Fruit
    description: Wakey wakey, let your senses shine with this taste of the tropics. Enjoy the exciting fruit combination of Light & Free Peach Passion Fruit!
    link: http://www.lightandfree.com/product/four-pack-peach-passion-fruit

  - title: Lemon
    description: Its zesty style will awaken your senses. Enjoy the refreshing taste of Light & Free Lemon!
    link: http://www.lightandfree.com/product/four-pack-lemon

  - title: Cherry
    description: Take a ride on the luscious side. Enjoy the sunkissed taste of Light & Free Cherry!
    link: http://www.lightandfree.com/product/four-pack-cherry

  - title: Strawberry
    description: Great taste, great style, you’re simply made for each other. Enjoy the irresistible taste of Light & Free Strawberry!
    link: http://www.lightandfree.com/product/four-pack-strawberry

  - title: Coconut
    description: Its coconut bits will tingle your taste buds. Enjoy the fresh taste of Light & Free Coconut!
    link: http://www.lightandfree.com/product/four-pack-coconut

  - title: Raspberry
    description: Enjoy the delicious taste of Light* & Free Raspberry!
    link: http://www.lightandfree.com/product/four-pack-raspberry
---

<div class="container vpad--xl">
  <div class="width width--lg text--center">
    <p class="text--xxl">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta voluptatibus eius itaque sequi cumque aliquid temporibus a adipisci voluptates atque, eveniet odio rem ullam, iure, qui incidunt! Totam magni adipisci harum quia possimus tenetur temporibus quae? Similique consequuntur ut architecto voluptatibus. Deserunt assumenda eveniet temporibus numquam, voluptatem officiis. Natus, molestiae.</p>
  </div>
</div>

<div class="bg--light">
  <div class="container">
    <div class="vpad--xxl">
      <div class="row row--4-4-4 row--gutters-lg">
        {% for item in page.flavours %}
        <div class="col">
          <div class="bg-img bg-img--1-1" style="background-image: url('{{site.img}}/img.jpg')">
            <a class="bg-img__link" href="{{item.link}}"></a>
            <div class="bg-img__bg-overlay"></div>
          </div>
          <div class="bg--white boxpad--md text--center">
            <div class="space--xs"></div>
            <div class="title title--sm"><a href="{{item.link}}">{{item.title}}</a></div>
            <p>{{item.description}}</p>
            <div class="space--sm"></div>
            <a href="{{item.link}}" class="btn btn--sm btn--outline btn--outline-orange">Find out more</a>
            <div class="space--xs"></div>
          </div>
        </div>
        {% endfor %}
      </div>
    </div>
  </div>
</div>

