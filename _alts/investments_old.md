<!-- # ---
layout: page
title: Investments
permalink: /investments/
--- -->

I advise and invest in a handful of start-ups across tech, with a focus on crypto. If you are an early stage start-up focusing on an area I'm passionate about, I'd love to help. Here are a few of the companies I am working with:

<div class="home">

  <ul class="post-list">
    {% for investment in site.investments %}
      <li>

        <h2>
          <a class="post-link" href="{{ investment.url | prepend: site.baseurl }}">
          
          <img src="{{ investment.logo | prepend: site.invimagebase }}" class="logo-image">
          
          </a>
        </h2>
      </li>
    {% endfor %}
  </ul>

</div>

