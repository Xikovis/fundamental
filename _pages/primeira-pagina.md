---
layout: default
title: "Meu Primeiro Post"
---

# Lista
1. Item 1
2. Item 2
3. Item 3

## Tabela
<table>
  {% for row in site.data.tabela %}
    {% if forloop.first %}
      <tr>
        {% for pair in row %}
          <th>{{ pair[0] }}</th>
        {% endfor %}
      </tr>
    {% endif %}
    <tr>
      {% for pair in row %}
        <td>{{ pair[1] }}</td>
      {% endfor %}
    </tr>
  {% endfor %}
</table>
