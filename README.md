
## Recent posts

<ul>
  {% for post in site.posts %}
  <li class="mb-3">
    <a href="{{ post.url }}"><h4>{{ post.title }}</h4></a>
    <p class="blockquote">{{ post.excerpt | default: '' }}</p>
    <p class="m-1">published {{ post.date | date_to_string }} by {{ post.author }}</p>
    {% for category in post.categories %}
      <p class="badge badge-warning">{{category}}</p>
    {% endfor %}
  </li>
  {% endfor %}
</ul>
