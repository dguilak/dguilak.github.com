---
layout: page
title: Main
tagline: Supporting tagline
group: navigation
---
    
# A wild Daniel Guilak approaches!
    
Just kidding, I'm domesticated. Since I'm currently tinkering around with HTML and CSS (I haven't really designed a website since well before puberty), content will be coming soon! Expect to experience a wide range of emotions such as elation, inspiration, and carboxylation. Wait, that last one doesn't sound right.

## About

I'm a double-major in Computer Science and Chemistry at the University of Puget Sound, and I'll be graduating in May. I love solving challenging problems via computation and learning new concepts and tools! Currently, I'm seeking software-engineering employment at a startup where I can do so in a collaborative and close-knit environment.

If you're interested in contacting me, please feel free to reach out through [Twitter](http://twitter.com/dguilak/), [LinkedIn](http://www.linkedin.com/pub/daniel-guilak/3a/22/145/145), or [GitHub](http://github.com/dguilak/).

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
