---
layout: page
title: Course
---
On this page, I will put some links to the homepage of the course, containing my understanding of the course and my own notes, I hope it will be helpful.
The course red and black list is [here](https://table.nju.edu.cn/external-apps/7aded834-74a2-43cc-b515-fb8e01656ef2/?page_id=zI1D).
Some useful resourse about CS you can find at [here](https://github.com/NijikaIjichi/njucs-past-exam).
{: .message }

<style>
  .semester-column { text-align: center; }
</style>

{% for section in site.data.courses %}
<table>
  <thead>
    <tr>
      {% if section.show_semester %}
      <th colspan="3">{{ section.title }}</th>
      {% else %}
      <th colspan="2">{{ section.title }}</th>
      {% endif %}
    </tr>
    {% if section.show_semester %}
    <tr>
      <th class="semester-column">Semester</th>
      <th>Course Name</th>
      <th>HomePage</th>
    </tr>
    {% endif %}
  </thead>
  <tbody>
    {% for row in section.rows %}
    <tr>
      {% if section.show_semester %}
      <td class="semester-column">{{ row.semester }}</td>
      {% endif %}

      <td>
        {% if row.course_emphasis %}
        <em>{{ row.course }}</em>
        {% else %}
        {{ row.course }}
        {% endif %}
      </td>

      <td>
        {% if row.homepage_text %}
        {{ row.homepage_text }}
        {% else %}
        {% if row.homepage_prefix %}{{ row.homepage_prefix }}{% endif %}
        {% for link in row.links %}
          {% if link.internal %}
            <a href="{{ link.url | relative_url }}">{{ link.label }}</a>
          {% else %}
            <a href="{{ link.url }}">{{ link.label }}</a>
          {% endif %}
          {% unless forloop.last %} & {% endunless %}
        {% endfor %}
        {% endif %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
{% endfor %}

<p>Note: <mark><em>Ongoing Course</em></mark></p>
<em>Prof.</em> means that this page is provided by the professor, please modify the website according to the academic year and semester.
