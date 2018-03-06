<h2>{{ site.data.nav.docs_list_title }}</h2>
<ul>
   {% for item in site.data.nav.docs %}
      <li><a href="{{ item.url }}" alt="{{ item.title }}">{{ item.title }}</a></li>
   {% endfor %}
</ul>

![Site logo](images/pttf.png)

[Testimonials](testimonials.html)

