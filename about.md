---
layout: page
title: About
permalink: /about/
---

![Me!](/images/me-portrait.png)

I am an investor and operator living in Brooklyn, NY.  I am from Buffalo, NY, and came to the great city of New York after spending time in the Bay Area, Seattle and at Cornell University. For a little more info about what I've done, click on the "Work" link above or take a look at my quite outdated [resume](/JohnMorrowResume.pdf). For any inquiries about freelance work or consulting, feel free to contact me via the information below.

<div>

I advise and invest in a handful of start-ups across tech, with a focus on crypto. If you are an early stage start-up focusing on an area I'm passionate about, I'd love to help. A few of the companies I work with are
    {% for investment in site.investments %}
    {% if forloop.last == true %} and {% endif %}
    <a  href="{{ investment.url | prepend: site.baseurl }}">{{investment.name}}</a>
    {% if forloop.last != true %},
    {% else %}.
    {% endif %}
    {% endfor %}
</div>

<p></p>

You can find the source code for this website [on my github](https://github.com/jmomx/mrjohnmorrow.github.io). See if you can figure out how to fix the whitespace issue with template-generated investment list above.
