# Hello World!
aqui vai um

## Páginas do Site

<ul>
  {% for page in site.pages %}
    {% if page.path contains 'paginas/' and page.title %}
      <li>
        <a href="{{ page.url | relative_url }}">{{ page.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
