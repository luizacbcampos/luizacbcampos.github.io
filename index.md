---
title: Main
layout: default
---

<div class="container-fluid p-0">
    {% for section in site.sections %}
        {%- if section.enabled -%}
        <section class="resume-section" id="{{section.name | downcase}}">
        {% include {{section.name | downcase}}.html %}
        </section>
        <hr class="m-0" />
        {%- endif -%}
    {% endfor %}
</div>


<!--
You can use HTML elements in Markdown, such as the comment element, and they won't
be affected by a markdown parser. However, if you create an HTML element in your
markdown file, you cannot use markdown syntax within that element's contents.
-->
