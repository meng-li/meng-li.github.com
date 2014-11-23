---
layout: page
title: meng-li's blog
---
{% include JB/setup %}


<dl class="posts">
  {% for post in site.posts %}
    <dd name="display"> 
      <h3>{{ post.title }}</h3>
      <span>{{ post.date | date_to_string }}</span> &raquo;<br/><hr style="height:3px;color:red;"/>
      <div name="lion">{{ post.content }}</div><a href="{{ BASE_PATH }}{{ post.url }}">read more</a>
      <hr/>
    </dd>
  {% endfor %}
</dl>
