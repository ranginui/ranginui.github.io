<center>
   {% for item in site.data.nav.docs %}
      <span> | <a href="{{ item.url }}" alt="{{ item.title }}">{{ item.title }}</a> | </span>
   {% endfor %}
</center>
