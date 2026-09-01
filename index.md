---
layout: default
---

<section class="home-intro">
  <p class="home-kicker">WEEKLY NOTES</p>
  <h1>留給自己的小小記事</h1>
  <p>這裡存放小林每週的學習、想法與生活。</p>
</section>

<section class="home-posts">
  <h2>最新週記</h2>

  <ul class="home-post-list">
    {% for post in site.posts %}
      <li>
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y.%m.%d" }}</time>
        <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </li>
    {% endfor %}
  </ul>
</section>
