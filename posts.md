---
layout: page
# title: All Posts
permalink: /posts/
layout: default
---

<div class="home" style="min-width: 55%;">
  {%- if page.title -%}
    <p class="post-title">{{ page.title }}</p>
  {%- endif -%}

  {%- if site.posts.size > 0 -%}
    <ul class="post-list">
      {%- for post in site.posts -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        
        <h3>

          <a class="post" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a> &nbsp; &nbsp;
          <span class="post-meta" style="float:right;">{{ post.date | date: date_format }}</span>
        </h3>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
      {%- endfor -%}
    </ul>

    <p class="feed-subscribe">
      <a href="{{ 'feed.xml' | relative_url }}">
        <svg class="svg-icon orange"><use xlink:href="{{ 'assets/minima-social-icons.svg#rss' | relative_url }}"></use></svg><span>Subscribe via RSS</span>
      </a>
    </p>
  {%- endif -%}

</div>