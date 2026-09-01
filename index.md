---
layout: default
---

<section class="home-intro">
  <p class="home-kicker">這裡存放小林的學習、想法與生活。</p>
 
</section>

<section class="home-posts">
  <h4>Post</h4>

  <ul class="home-post-list">
    {% for post in site.posts %}
      <li>
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y.%m.%d" }}</time>
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </li>
    {% endfor %}
  </ul>
</section>
